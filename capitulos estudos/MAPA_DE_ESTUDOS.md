# Mapa de estudos e capítulos

**Versão:** 2.0 — 19/10/2026. **Natureza:** Mapa de estudos da formação técnica e índice central dos capítulos de estudos.

[Índice de estudos](README.md) · [Acervo de publicações](<../registro da autoridade/PUBLICACOES.md>) · [Método editorial](<../spec editorial/GUIA_DE_OPERACAO.md>)

---

## Como usar

Este é o local de referência para a ordem de estudo e navegação pelos **capítulos de estudos**. Os IDs CAP-00 a CAP-19 identificam as unidades de trabalho e formação do Engenheiro Agêntico. Cada capítulo possui sua pasta dedicada e seu **documento base**, contendo objetivos pedagógicos, o papel do engenheiro agêntico, conceitos formais, aplicação dos filtros de leitura diagnóstica e evidências esperadas.

A sequência numérica reflete a rampa pedagógica *Outside-In* (da governança ao silício), permitindo que o profissional domine primeiro a infraestrutura de agentes e o campo de força de auditoria externa antes de mergulhar nos fundamentos clássicos de computação e runtime.

---

## Sequência dos Capítulos de Estudos

Abaixo está a trilha completa dos 20 capítulos de estudos organizados em suas 8 partes fundamentais:

| Ordem / ID | Parte e Capítulo de Estudo | Documento Base | Objetivo Central | Pré-requisitos | Estado |
| :---: | :--- | :---: | :--- | :--- | :--- |
| 00 / CAP-00 | 0 — Setup, IDE, harness, git e loops | [Base CAP-00](00-setup-ide-harness-e-loops/documento-base.md) | Estruturar ambiente profissional com MCP, rules, skills, subagentes e git worktrees. | Ponto de partida; nenhum CAP anterior exigido. | Planejado — ponto de entrada inicial |
| 01 / CAP-01 | I — Campo de força, validações e governança | [Base CAP-01](01-campo-de-forca-validacoes-e-governanca/documento-base.md) | Construir guardrails (linter/pre-commit), validação caixa-preta e validar sem ler código (caso PDV D+). | CAP-00 | Planejado — novo ponto de entrada prático |
| 02 / CAP-02 | II — Problema, requisitos e atributos de qualidade | [Base CAP-02](02-problema-requisitos-e-atributos-de-qualidade/documento-base.md) | Formular requisitos inequívocos e cenários de atributos de qualidade (NFRs) mensuráveis. | CAP-01 | Planejado |
| 03 / CAP-03 | II — Linguagem e fronteiras de domínio | [Base CAP-03](03-linguagem-e-fronteiras-de-dominio/documento-base.md) | Aplicar Linguagem Ubíqua, Bounded Contexts e Context Mapping (DDD) para guiar agentes. | CAP-02 | Planejado |
| 04 / CAP-04 | II — SDD e rastreabilidade no desenvolvimento | [Base CAP-04](04-sdd-e-rastreabilidade-no-desenvolvimento/documento-base.md) | Estruturar cadeia ponta a ponta: Requisito -> Spec -> Tarefa -> Implementação -> Verificação. | CAP-02 e CAP-03 | Planejado |
| 05 / CAP-05 | III — Contratos e leitura diagnóstica | [Base CAP-05](05-contratos-e-leitura-diagnostica/documento-base.md) | Dominar Design por Contrato e os 5 Filtros de Auditoria Visual rápida de código gerado por IA. | CAP-01 e CAP-04 | Planejado |
| 06 / CAP-06 | III — Verificação, validação e aceitação | [Base CAP-06](06-verificacao-validacao-e-aceitacao/documento-base.md) | Distinguir V&V, pirâmide/troféu, BDD e auditar testes falsos/tautológicos ("placebos verdes"). | CAP-02 e CAP-05 | Planejado |
| 07 / CAP-07 | III — Propriedades, mutação e eficácia dos testes | [Base CAP-07](07-propriedades-mutacao-e-eficacia-dos-testes/documento-base.md) | Avaliar escore de testes de mutação e criar testes baseados em propriedades (QuickCheck). | CAP-06 | Planejado |
| 08 / CAP-08 | IV — Modularidade e dependências | [Base CAP-08](08-modularidade-e-dependencias/documento-base.md) | Aplicar Information Hiding (Parnas), acoplamento/coesão e SOLID para estabilidade de contexto. | CAP-03 e CAP-05 | Planejado |
| 09 / CAP-09 | IV — Escolhas arquiteturais | [Base CAP-09](09-escolhas-arquiteturais/documento-base.md) | Comparar monolito modular, arquitetura hexagonal, microsserviços e Conway via ADRs. | CAP-02 e CAP-08 | Planejado |
| 10 / CAP-10 | V — Execução, runtime e memória | [Base CAP-10](10-execucao-runtime-e-memoria/documento-base.md) | Explicar stack, heap e gerenciamento de memória no ambiente escolhido (Dart desktop). | CAP-05 e CAP-08 | Preparação conferida — estudo a iniciar |
| 11 / CAP-11 | V — Processos, threads e I/O | [Base CAP-11](11-processos-threads-e-io/documento-base.md) | Relacionar execução, concorrência, event loop, latência de I/O e descritores físicos. | CAP-10 | Planejado |
| 12 / CAP-12 | V — Qualidade, métricas e profiling | [Base CAP-12](12-qualidade-metricas-e-profiling/documento-base.md) | Interpretar complexidade ciclomática, acoplamento, métricas de Halstead, SAST e profiling. | CAP-10 e CAP-11 | Planejado |
| 13 / CAP-13 | VI — Dados, transações e isolamento | [Base CAP-13](13-dados-transacoes-e-isolamento/documento-base.md) | Controlar concorrência, propriedades ACID, anomalias de isolamento e travamento (OCC/PCC). | CAP-05 e CAP-11 | Planejado |
| 14 / CAP-14 | VI — Distribuição e consistência | [Base CAP-14](14-distribuicao-e-consistencia/documento-base.md) | Compreender falhas parciais de rede, Teorema CAP, modelo PACELC, 2PC e Padrão Saga. | CAP-09 e CAP-13 | Planejado |
| 15 / CAP-15 | VI — Mensageria, APIs e sincronização | [Base CAP-15](15-mensageria-apis-e-sincronizacao/documento-base.md) | Projetar idempotência, semântica de mensageria, outbox transacional e arquitetura offline-first. | CAP-06 e CAP-14 | Planejado |
| 16 / CAP-16 | VII — Evolução e compatibilidade | [Base CAP-16](16-evolucao-e-compatibilidade/documento-base.md) | Gerenciar débito técnico, Leis de Lehman, SemVer e migrações progressivas (Expand & Contract). | CAP-06 e CAP-09 | Planejado |
| 17 / CAP-17 | VII — Resiliência e observabilidade | [Base CAP-17](17-resiliencia-e-observabilidade/documento-base.md) | Implementar Circuit Breakers, Bulkheads, Retries com Jitter e rastreamento OpenTelemetry. | CAP-12 e CAP-15 | Planejado |
| 18 / CAP-18 | VII — Segurança aplicada e julgamento econômico | [Base CAP-18](18-seguranca-aplicada-e-julgamento-economico/documento-base.md) | Auditar riscos OWASP, criptografia e finanças de software (trade-offs de TCO e manutenção). | CAP-09 e CAP-15 | Planejado |
| 19 / CAP-19 | VII — Orquestração avançada, evals e governança | [Base CAP-19](19-orquestracao-avancada-evals-e-governanca/documento-base.md) | Integrar engenharia de contexto, harnesses de agentes (MCP), suítes de Evals e governança contínua. | CAP-04, CAP-07 e CAP-17 | Planejado |

---

## Práticas que acompanham os capítulos

* **Leitura diagnóstica e auditoria de código:** Praticadas continuamente em todas as unidades com foco nos 5 Filtros Visuais.
* **Orquestração e liderança de agentes:** Praticadas desde o primeiro capítulo ao utilizar IA sob especificações e restrições formais.
* **Julgamento de engenharia e economia:** Avaliação constante de trade-offs, limites de ferramentas e custos operacionais.
* **Ciclo de estudo e registro:** Pergunta norteadora, consulta a fontes primárias, aplicação prática e registro objetivo da evidência produzida.

---

## Acompanhamento e Vínculos

| Capítulo | Documentos de Trabalho | Fontes Selecionadas | Registro / Evidência | Próxima Ação |
| :--- | :--- | :--- | :--- | :--- |
| **CAP-00** | [Base CAP-00](00-setup-ide-harness-e-loops/documento-base.md) | Anthropic MCP, Git Worktrees, Harness Engineering | Ponto de partida de infraestrutura definido | Iniciar preparação técnica da unidade |
| **CAP-01** | [Base CAP-01](01-campo-de-forca-validacoes-e-governanca/documento-base.md) | Clean Architecture, MOC/SEFAZ (XSD), Evolutionary Architectures | Caso prático delimitado no PDV D+ fiscal | Iniciar preparação técnica da unidade |
| **CAP-10** | [FIC-CAP-10 r03](10-execucao-runtime-e-memoria/ficha-editorial.md) · [Base CAP-10](10-execucao-runtime-e-memoria/documento-base.md) | Dart Overview, DevTools Memory, Functions & Debugger | Ponto de partida autoral delimitado em Dart desktop; caso síncrono estruturado | Preparação conferida; aguarda pré-requisitos pedagógicos |
| **Demais CAPs** | Pastas dedicadas com seus respectivos `documento-base.md` | Obras primárias e documentações mapeadas nos documentos base | Aguardando avanço da sequência de estudos | Iniciar preparação da unidade ao atingir seus pré-requisitos |

---

## Pendências Concretas

1. **CAP-00 e CAP-01:** Novos pontos de entrada criados. Podem ter suas fichas editoriais preparadas quando autorizado o início da escrita.
2. **CAP-10 (antigo CAP-01):** Preparação conceitual em Dart desktop preservada de forma íntegra; agora posicionada pedagogicamente na Parte V (O Chão da Máquina).
