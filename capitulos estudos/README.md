# Capítulos de Estudos

Esta pasta é o centro de formação técnica do projeto, responsável por estruturar, documentar e desenvolver os **capítulos de estudos**.

Os capítulos constituem um percurso técnico autônomo voltado à formação do **Engenheiro Agêntico**. Ensinam fundamentos de computação, engenharia de software e práticas de orquestração e auditoria de IA com rigor conceitual e exemplos verificáveis, sem exigir que o leitor conheça a vida do autor ou leia a narrativa pessoal da [Jornada do Herói](<../jornada do heroi/README.md>).

---

## 1. Visão Geral das 7 Partes e Temas Transversais

A trilha de formação organiza-se em sete partes técnicas estruturantes e um eixo transversal que acompanha todo o percurso:

| Parte | Foco de Estudo | Competência do Engenheiro Agêntico |
| :--- | :--- | :--- |
| **I — Computação e Runtime** | Execução física, stack, heap, ciclo de vida de objetos, processos, threads e latência de I/O. | Entender como o código gerado consome memória e CPU; evitar vazamentos, contenção e bloqueios de I/O. |
| **II — Qualidade, Métricas e Auditoria** | Design por Contrato, complexidade ciclomática, acoplamento, SAST e profiling. | Aplicar os 5 Filtros Visuais de auditoria rápida; rejeitar código hipercomplexo e frágil antes da execução. |
| **III — Requisitos, Domínio e SDD** | Requisitos não funcionais (NFRs), cenários de qualidade, DDD (Bounded Contexts) e SDD. | Fornecer contexto inequívoco e contratos formais aos agentes; manter rastreabilidade ponta a ponta. |
| **IV — Modularidade e Arquitetura** | Information Hiding (Parnas), acoplamento/coesão, SOLID, arquitetura hexagonal e Conway. | Isolar o núcleo de negócio contra mudanças em bibliotecas ou frameworks externos gerados por IA. |
| **V — Verificação, Validação e Testes** | V&V, pirâmide/troféu de testes, BDD, testes baseados em propriedades e testes de mutação. | Auditar testes tautológicos ("placebos verdes"); garantir que a suíte realmente capture falhas e mutantes. |
| **VI — Dados, Concorrência e Distribuição** | Propriedades ACID, isolamento, locks, Teorema CAP, PACELC, Saga, idempotência e offline-first. | Evitar anomalias concorrentes (Lost Updates), desenhar operações idempotentes e lidar com falhas de rede. |
| **VII — Evolução e Resiliência em Produção** | Leis de Lehman, débito técnico, SemVer, Expand & Contract, Circuit Breakers e OpenTelemetry. | Sustentar sistemas vivos, migrar contratos sem quebrar clientes e diagnosticar incidentes via telemetria. |
| **Transversal — Orquestração e Governança** | Engenharia de contexto, harnesses de agentes (MCP), pipelines de avaliação (*evals*) e auditoria contínua. | Liderar múltiplos agentes com governança, testar prompts/specs e manter a soberania de engenharia. |

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

* **[MAPA_DE_ESTUDOS.md](MAPA_DE_ESTUDOS.md):** Tabela central com a sequência de pré-requisitos dos 18 capítulos (CAP-01 a CAP-18), links diretos para cada base e acompanhamento de status.
* **Pastas Dedicadas (`01` a `18`):** Cada capítulo conta com sua pasta própria e seu respectivo `documento-base.md`, onde são detalhados a pergunta central, os conceitos formais, os filtros diagnósticos aplicados e a evidência esperada:
  * `01-execucao-runtime-e-memoria/`
  * `02-processos-threads-e-io/`
  * `03-contratos-e-leitura-diagnostica/`
  * `04-qualidade-metricas-e-profiling/`
  * `05-problema-requisitos-e-atributos-de-qualidade/`
  * `06-linguagem-e-fronteiras-de-dominio/`
  * `07-sdd-e-rastreabilidade-no-desenvolvimento/`
  * `08-modularidade-e-dependencias/`
  * `09-escolhas-arquiteturais/`
  * `10-verificacao-validacao-e-aceitacao/`
  * `11-propriedades-mutacao-e-eficacia-dos-testes/`
  * `12-dados-transacoes-e-isolamento/`
  * `13-distribuicao-e-consistencia/`
  * `14-mensageria-apis-e-sincronizacao/`
  * `15-evolucao-e-compatibilidade/`
  * `16-resiliencia-e-observabilidade/`
  * `17-seguranca-aplicada-e-julgamento-economico/`
  * `18-orquestracao-contexto-e-governanca-de-agentes/`

---

## 4. Notas sobre Fontes Históricas

As transcrições literais e os registros de conversas que serviram de subsídio à montagem inicial da grade estão preservados de forma imutável nos anexos da jornada ([`06-texto-anexo.md`](<../jornada do heroi/06-texto-anexo.md>) e [`10-texto-anexo.md`](<../jornada do heroi/10-texto-anexo.md>)). Toda a base conceitual ativa e as diretrizes editoriais estão unificadas neste README e no mapa de estudos.
