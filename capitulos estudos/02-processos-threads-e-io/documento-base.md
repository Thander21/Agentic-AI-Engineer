# Documento Base — CAP-02: Processos, threads e I/O

**ID:** CAP-02  
**Parte:** I — Computação e Runtime  
**Estado:** Planejado — aguardando conclusão de CAP-01  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Quando o código gerado executa uma operação assíncrona, abre um arquivo ou se comunica pela rede, como o sistema operacional e o runtime gerenciam processos, threads, descritores de arquivo e portas sem travar a CPU?
* **Objetivo de estudo:** Relacionar a execução lógica do software à concorrência física, sistemas operacionais e latência de I/O, compreendendo modelos de concorrência (preempção vs. cooperativo/event loop), multiplexação de conexões e limites de recursos físicos.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** IAs frequentemente misturam código bloqueante com laços de eventos não-bloqueantes (ex.: realizar leitura síncrona de arquivo ou chamada externa de rede dentro da thread principal de interface/API), ou geram milhares de threads sem pool, exaurindo descritores de arquivo do sistema operacional.
* **Decisões sob responsabilidade do engenheiro:**
  * Avaliar se uma operação de entrada e saída (I/O) é bloqueante ou assíncrona/não-bloqueante.
  * Identificar e mitigar condições de corrida (*race conditions*) e sincronização de memória entre threads.
  * Auditar o uso de sockets, descritores de arquivo (*file descriptors*) e portas de rede, garantindo fechamento e reuso seguro de conexões.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-01: Execução, runtime e memória](../01-execucao-runtime-e-memoria/documento-base.md).
* **Tópicos essenciais:**
  * Processos vs. Threads: isolamento de espaço de endereçamento versus memória compartilhada.
  * Modelos de concorrência: threads do sistema operacional (*kernel threads*), threads leves (*green threads* / *goroutines* / *isolates*) e Event Loop com I/O multiplexado (`epoll`/`kqueue`/`IOCP`).
  * Latência física de I/O: a disparidade de tempo entre registradores, cache L1/L2, RAM, SSD/NVMe e chamadas de rede.
  * Descritores de arquivos, sockets TCP/UDP e vazamento de recursos (*file descriptor exhaustion*).

---

## 4. Prática e Evidência Esperada

* **Ambiente sugerido:** Dart no desktop (usando `Isolate`, `Stream` ou manipulação de arquivos) ou runtime similar.
* **Caso didático:** Comparação entre uma rotina que bloqueia a thread de execução e uma rotina concorrente/não-bloqueante que despacha tarefas, monitorando tempo de resposta e estado da thread.
* **Evidência esperada:** Registro de um caso com medição de latência observada, demonstração do fluxo de escalonamento e relato dos limites de contenção de CPU vs. espera de I/O.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtro em destaque:** *Filtro 2 (Efeitos Colaterais, I/O e Concorrência)* e *Filtro 5 (Inspeção Viva)*.
* **Pergunta de auditoria rápida:** "Existe alguma chamada de rede ou disco bloqueante no caminho crítico? Esse loop abre descritores de rede ou arquivos sem garantia explícita de fechamento em bloco seguro (`finally`/`try-with-resources`)?"

---

## 6. Fontes Primárias de Referência

1. **Operating Systems: Three Easy Pieces (OSTEP)** — Remzi H. Arpaci-Dusseau e Andrea C. Arpaci-Dusseau (capítulos sobre Concorrência, Threads, Locks e I/O).
2. **Dart Asynchrony & Isolates Support:** Event loop, microtasks, event queue e concorrência baseada em isolamento de memória ([dart.dev/guides/language/concurrency](https://dart.dev/guides/language/concurrency)).
3. **The Linux Programming Interface / POSIX Standards:** Conceitos fundamentais de processos, file descriptors e sockets de rede.

