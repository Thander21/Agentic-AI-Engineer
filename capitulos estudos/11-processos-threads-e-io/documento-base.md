# Documento Base — CAP-11: Processos, threads e I/O

**ID:** CAP-11  
**Parte:** V — Computação e Runtime  
**Estado:** Planejado — aguardando conclusão de CAP-10  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Quando o cÃ³digo gerado executa uma operaÃ§Ã£o assÃ­ncrona, abre um arquivo ou se comunica pela rede, como o sistema operacional e o runtime gerenciam processos, threads, descritores de arquivo e portas sem travar a CPU?
* **Objetivo de estudo:** Relacionar a execuÃ§Ã£o lÃ³gica do software Ã  concorrÃªncia fÃ­sica, sistemas operacionais e latÃªncia de I/O, compreendendo modelos de concorrÃªncia (preempÃ§Ã£o vs. cooperativo/event loop), multiplexaÃ§Ã£o de conexÃµes e limites de recursos fÃ­sicos.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** IAs frequentemente misturam cÃ³digo bloqueante com laÃ§os de eventos nÃ£o-bloqueantes (ex.: realizar leitura sÃ­ncrona de arquivo ou chamada externa de rede dentro da thread principal de interface/API), ou geram milhares de threads sem pool, exaurindo descritores de arquivo do sistema operacional.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Avaliar se uma operaÃ§Ã£o de entrada e saÃ­da (I/O) Ã© bloqueante ou assÃ­ncrona/nÃ£o-bloqueante.
  * Identificar e mitigar condiÃ§Ãµes de corrida (*race conditions*) e sincronizaÃ§Ã£o de memÃ³ria entre threads.
  * Auditar o uso de sockets, descritores de arquivo (*file descriptors*) e portas de rede, garantindo fechamento e reuso seguro de conexÃµes.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-01: ExecuÃ§Ã£o, runtime e memÃ³ria](../01-execucao-runtime-e-memoria/documento-base.md).
* **TÃ³picos essenciais:**
  * Processos vs. Threads: isolamento de espaÃ§o de endereÃ§amento versus memÃ³ria compartilhada.
  * Modelos de concorrÃªncia: threads do sistema operacional (*kernel threads*), threads leves (*green threads* / *goroutines* / *isolates*) e Event Loop com I/O multiplexado (`epoll`/`kqueue`/`IOCP`).
  * LatÃªncia fÃ­sica de I/O: a disparidade de tempo entre registradores, cache L1/L2, RAM, SSD/NVMe e chamadas de rede.
  * Descritores de arquivos, sockets TCP/UDP e vazamento de recursos (*file descriptor exhaustion*).

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Ambiente sugerido:** Dart no desktop (usando `Isolate`, `Stream` ou manipulaÃ§Ã£o de arquivos) ou runtime similar.
* **Caso didÃ¡tico:** ComparaÃ§Ã£o entre uma rotina que bloqueia a thread de execuÃ§Ã£o e uma rotina concorrente/nÃ£o-bloqueante que despacha tarefas, monitorando tempo de resposta e estado da thread.
* **EvidÃªncia esperada:** Registro de um caso com mediÃ§Ã£o de latÃªncia observada, demonstraÃ§Ã£o do fluxo de escalonamento e relato dos limites de contenÃ§Ã£o de CPU vs. espera de I/O.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtro em destaque:** *Filtro 2 (Efeitos Colaterais, I/O e ConcorrÃªncia)* e *Filtro 5 (InspeÃ§Ã£o Viva)*.
* **Pergunta de auditoria rÃ¡pida:** "Existe alguma chamada de rede ou disco bloqueante no caminho crÃ­tico? Esse loop abre descritores de rede ou arquivos sem garantia explÃ­cita de fechamento em bloco seguro (`finally`/`try-with-resources`)?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Operating Systems: Three Easy Pieces (OSTEP)** â€” Remzi H. Arpaci-Dusseau e Andrea C. Arpaci-Dusseau (capÃ­tulos sobre ConcorrÃªncia, Threads, Locks e I/O).
2. **Dart Asynchrony & Isolates Support:** Event loop, microtasks, event queue e concorrÃªncia baseada em isolamento de memÃ³ria ([dart.dev/guides/language/concurrency](https://dart.dev/guides/language/concurrency)).
3. **The Linux Programming Interface / POSIX Standards:** Conceitos fundamentais de processos, file descriptors e sockets de rede.

