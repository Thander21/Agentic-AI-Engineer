# Capítulos de Estudos

Esta pasta é o centro de formação técnica do projeto, responsável por estruturar, documentar e desenvolver os **capítulos de estudos**.

Os capítulos constituem um percurso técnico autônomo voltado à formação do **Engenheiro Agêntico**. Ensinam desde a infraestrutura prática e governança de agentes (harness, guardrails, validação sem ler código) até os fundamentos profundos de computação, arquitetura, testes e resiliência com rigor conceitual e exemplos verificáveis, sem exigir que o leitor conheça a vida do autor ou leia a narrativa pessoal da [Jornada do Herói](<../jornada do heroi/README.md>).

---

## 1. Visão Geral das 8 Partes Estruturantes

A trilha de formação organiza-se em uma rampa pedagógica *Outside-In* (da governança ao silício), distribuída em 8 partes e 20 capítulos:

| Parte | Foco de Estudo | Competência do Engenheiro Agêntico |
| :--- | :--- | :--- |
| **0 — Setup do Engenheiro Agêntico** | LLMs, IDE, Harness, MCP, Skills, Subagentes, Git Worktrees e Loops de Feedback. | Estruturar o ecossistema e ambiente de desenvolvimento isolado para agentes atuarem com segurança. |
| **I — Governança Prática e Guardrails** | Campo de força (linters, pre-commit), auditoria caixa-preta, oráculos e validação sem ler código. | Garantir a corretude externa do produto (caso PDV D+ / NFC-e) contendo danos e rejeitando alucinações. |
| **II — Especificação e Domínio** | Requisitos não funcionais (NFRs), Bounded Contexts (DDD) e SDD ponta a ponta. | Fornecer contexto inequívoco e especificações executáveis para alimentar os agentes de IA. |
| **III — Auditoria, Contratos e Verificação** | Design por Contrato, os 5 Filtros Visuais, testes "placebo", testes de mutação e propriedades. | Auditar código gerado em segundos e provar matematicamente se a suíte de testes realmente captura falhas. |
| **IV — Modularidade e Arquitetura** | Information Hiding (Parnas), acoplamento/coesão, SOLID, arquitetura hexagonal e ADRs. | Isolar o núcleo de negócio para que módulos caibam nas janelas de contexto (*context windows*) dos modelos. |
| **V — Computação e o Chão da Máquina** | Execução física, stack, heap, GC (Dart desktop), event loop, concorrência, I/O e profiling. | Diagnosticar onde o código gerado consome memória e CPU; evitar vazamentos e travamentos de interface. |
| **VI — Dados, Concorrência e Distribuição** | Propriedades ACID, isolamento, locks, Teorema CAP, PACELC, Saga, idempotência e offline-first. | Evitar anomalias concorrentes (Lost Updates), desenhar operações idempotentes e lidar com falhas de rede. |
| **VII — Produção e Soberania Agêntica** | Leis de Lehman, SemVer, Expand & Contract, Circuit Breakers, OpenTelemetry, Evals e Governança. | Sustentar sistemas vivos, migrar contratos sem quebrar clientes e liderar frotas de agentes com soberania. |

---

## 2. Ciclo de Vida e Maturidade Editorial dos Capítulos

Para garantir que o conteúdo não seja apenas teoria abstrata nem cópia sem verificação, cada capítulo passa por estados explícitos de trabalho:

1. **Nota de estudo:** Registro inicial de uma dúvida, pergunta norteadora ou formulação de hipótese conceitual.
2. **Caso documentado:** Delimitação de um cenário prático ou problema real, registrando contexto, código didático e resultado observado.
3. **Caso conferido:** Verificação objetiva das afirmações contra fontes primárias e evidências de execução (profiler, testes de mutação, logs).
4. **Texto para leitura (esboço):** Estruturação didática e redação orientada ao leitor técnico, com explicações claras e sem necessidade de autobiografia.
5. **Capítulo revisado:** Integração de retorno editorial, revisão técnica dos exemplos e conferência de sua capacidade de ensinar com autonomia.

---

## 3. Estrutura das Pastas e Navegação

* **[MAPA_DE_ESTUDOS.md](MAPA_DE_ESTUDOS.md):** Tabela central com a sequência de pré-requisitos dos 20 capítulos (CAP-00 a CAP-19), links diretos para cada base e acompanhamento de status.
* **Pastas Dedicadas (`00` a `19`):** Cada capítulo conta com sua pasta própria e seu respectivo `documento-base.md`, onde são detalhados a pergunta central, os conceitos formais, os filtros diagnósticos aplicados e a evidência esperada:
  * `00-setup-ide-harness-e-loops/`
  * `01-campo-de-forca-validacoes-e-governanca/`
  * `02-problema-requisitos-e-atributos-de-qualidade/`
  * `03-linguagem-e-fronteiras-de-dominio/`
  * `04-sdd-e-rastreabilidade-no-desenvolvimento/`
  * `05-contratos-e-leitura-diagnostica/`
  * `06-verificacao-validacao-e-aceitacao/`
  * `07-propriedades-mutacao-e-eficacia-dos-testes/`
  * `08-modularidade-e-dependencias/`
  * `09-escolhas-arquiteturais/`
  * `10-execucao-runtime-e-memoria/`
  * `11-processos-threads-e-io/`
  * `12-qualidade-metricas-e-profiling/`
  * `13-dados-transacoes-e-isolamento/`
  * `14-distribuicao-e-consistencia/`
  * `15-mensageria-apis-e-sincronizacao/`
  * `16-evolucao-e-compatibilidade/`
  * `17-resiliencia-e-observabilidade/`
  * `18-seguranca-aplicada-e-julgamento-economico/`
  * `19-orquestracao-avancada-evals-e-governanca/`

---

## 4. Notas sobre Fontes Históricas

As transcrições literais e os registros de conversas que serviram de subsídio à montagem inicial da grade estão preservados de forma imutável nos anexos da jornada ([`06-texto-anexo.md`](<../jornada do heroi/06-texto-anexo.md>) e [`10-texto-anexo.md`](<../jornada do heroi/10-texto-anexo.md>)). Toda a base conceitual ativa e as diretrizes editoriais estão unificadas neste README e no mapa de estudos.
