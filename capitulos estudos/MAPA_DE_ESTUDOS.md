# Mapa de estudos e capítulos

**Versão:** 1.0 — 19/10/2026. **Natureza:** Mapa de estudos da formação técnica e índice central dos capítulos de estudos.

[Índice de estudos](README.md) · [Acervo de publicações](<../registro da autoridade/PUBLICACOES.md>) · [Método editorial](<../spec editorial/GUIA_DE_OPERACAO.md>)

---

## Como usar

Este é o local de referência para a ordem de estudo e navegação pelos **capítulos de estudos**. Os IDs CAP-01 a CAP-18 identificam as unidades de trabalho e formação. Cada capítulo possui sua pasta dedicada e seu **documento base**, contendo objetivos pedagógicos, o papel do engenheiro agêntico, conceitos formais, aplicação dos filtros de leitura diagnóstica e evidências esperadas.

A sequência numérica serve como guia estruturado de pré-requisitos: dependência técnica significa compreensão necessária para a atividade proposta. O acompanhamento prático, as decisões e os experimentos realizados são registrados nas pastas de cada unidade.

---

## Sequência dos Capítulos de Estudos

Abaixo está a trilha completa dos 18 capítulos de estudos organizados em suas 7 partes fundamentais e eixo transversal:

| Ordem / ID | Parte e Capítulo de Estudo | Documento Base | Objetivo Central | Pré-requisitos | Estado |
| :---: | :--- | :---: | :--- | :--- | :--- |
| 01 / CAP-01 | I — Execução, runtime e memória | [Base CAP-01](01-execucao-runtime-e-memoria/documento-base.md) | Explicar stack, heap e gerenciamento de memória no ambiente escolhido (Dart desktop). | Ponto de partida delimitado; nenhum CAP anterior exigido. | Preparação conferida — estudo a iniciar |
| 02 / CAP-02 | I — Processos, threads e I/O | [Base CAP-02](02-processos-threads-e-io/documento-base.md) | Relacionar execução, concorrência, event loop, latência de I/O e descritores físicos. | CAP-01 | Planejado |
| 03 / CAP-03 | II — Contratos e leitura diagnóstica | [Base CAP-03](03-contratos-e-leitura-diagnostica/documento-base.md) | Dominar Design por Contrato e os 5 Filtros de Auditoria Visual rápida de código gerado por IA. | CAP-01 | Planejado |
| 04 / CAP-04 | II — Qualidade, métricas e profiling | [Base CAP-04](04-qualidade-metricas-e-profiling/documento-base.md) | Interpretar complexidade ciclomática, acoplamento, métricas de Halstead, SAST e profiling. | CAP-02 e CAP-03 | Planejado |
| 05 / CAP-05 | III — Problema, requisitos e atributos de qualidade | [Base CAP-05](05-problema-requisitos-e-atributos-de-qualidade/documento-base.md) | Formular requisitos inequívocos e cenários de atributos de qualidade (NFRs) mensuráveis. | CAP-03 | Planejado |
| 06 / CAP-06 | III — Linguagem e fronteiras de domínio | [Base CAP-06](06-linguagem-e-fronteiras-de-dominio/documento-base.md) | Aplicar Linguagem Ubíqua, Bounded Contexts e Context Mapping (DDD) para guiar agentes. | CAP-05 | Planejado |
| 07 / CAP-07 | III — SDD e rastreabilidade no desenvolvimento | [Base CAP-07](07-sdd-e-rastreabilidade-no-desenvolvimento/documento-base.md) | Estruturar cadeia ponta a ponta: Requisito -> Spec -> Tarefa -> Implementação -> Verificação. | CAP-05 e CAP-06 | Planejado |
| 08 / CAP-08 | IV — Modularidade e dependências | [Base CAP-08](08-modularidade-e-dependencias/documento-base.md) | Aplicar Information Hiding (Parnas), acoplamento/coesão (Stevens) e SOLID para estabilidade. | CAP-03 e CAP-06 | Planejado |
| 09 / CAP-09 | IV — Escolhas arquiteturais | [Base CAP-09](09-escolhas-arquiteturais/documento-base.md) | Comparar monolito modular, arquitetura hexagonal, microsserviços e Conway via ADRs. | CAP-05 e CAP-08 | Planejado |
| 10 / CAP-10 | V — Verificação, validação e aceitação | [Base CAP-10](10-verificacao-validacao-e-aceitacao/documento-base.md) | Distinguir V&V, pirâmide/troféu, BDD e auditar testes falsos/tautológicos gerados por IA. | CAP-03 e CAP-05 | Planejado |
| 11 / CAP-11 | V — Propriedades, mutação e eficácia dos testes | [Base CAP-11](11-propriedades-mutacao-e-eficacia-dos-testes/documento-base.md) | Avaliar escore de testes de mutação e criar testes baseados em propriedades (QuickCheck). | CAP-10 | Planejado |
| 12 / CAP-12 | VI — Dados, transações e isolamento | [Base CAP-12](12-dados-transacoes-e-isolamento/documento-base.md) | Controlar concorrência, propriedades ACID, anomalias de isolamento e travamento (OCC/PCC). | CAP-02 e CAP-03 | Planejado |
| 13 / CAP-13 | VI — Distribuição e consistência | [Base CAP-13](13-distribuicao-e-consistencia/documento-base.md) | Compreender falhas parciais de rede, Teorema CAP, modelo PACELC, 2PC e Padrão Saga. | CAP-09 e CAP-12 | Planejado |
| 14 / CAP-14 | VI — Mensageria, APIs e sincronização | [Base CAP-14](14-mensageria-apis-e-sincronizacao/documento-base.md) | Projetar idempotência, semântica de mensageria, outbox transacional e arquitetura offline-first. | CAP-10 e CAP-13 | Planejado |
| 15 / CAP-15 | VII — Evolução e compatibilidade | [Base CAP-15](15-evolucao-e-compatibilidade/documento-base.md) | Gerenciar débito técnico, Leis de Lehman, SemVer e migrações progressivas (Expand & Contract). | CAP-09 e CAP-10 | Planejado |
| 16 / CAP-16 | VII — Resiliência e observabilidade | [Base CAP-16](16-resiliencia-e-observabilidade/documento-base.md) | Implementar Circuit Breakers, Bulkheads, Retries com Jitter e rastreamento OpenTelemetry. | CAP-04 e CAP-14 | Planejado |
| 17 / CAP-17 | VII — Segurança aplicada e julgamento econômico | [Base CAP-17](17-seguranca-aplicada-e-julgamento-economico/documento-base.md) | Auditar riscos OWASP, criptografia e finanças de software (trade-offs de TCO e manutenção). | CAP-09 e CAP-14 | Planejado |
| 18 / CAP-18 | Transversal — Orquestração, contexto e governança | [Base CAP-18](18-orquestracao-contexto-e-governanca-de-agentes/documento-base.md) | Integrar engenharia de contexto, harnesses de agentes (MCP), suítes de Evals e governança. | CAP-07 e CAP-11 | Planejado |

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
| **CAP-01** | [FIC-CAP-01 r02](01-execucao-runtime-e-memoria/ficha-editorial.md) · [Base CAP-01](01-execucao-runtime-e-memoria/documento-base.md) | Dart Overview, DevTools Memory, Functions & Debugger | Ponto de partida autoral delimitado em Dart desktop; caso síncrono estruturado | Iniciar redação do esboço introdutório conceitual conforme autorizado |
| **CAP-02** a **CAP-18** | Pastas dedicadas `02` a `18` com seus respectivos `documento-base.md` | Obras primárias e documentações mapeadas nos documentos base | Aguardando avanço da sequência de estudos | Iniciar preparação da unidade ao atingir seus pré-requisitos |

---

## Pendências Concretas

1. **CAP-01:** Preparação conceitual concluída. Ao avançar para testes práticos no Dart SDK, fixar versão do SDK, ambiente operacional e fonte imutável da implementação.
2. **Atualização contínua:** Conforme cada capítulo avançar, atualizar o estado e registrar as evidências diretamente nas fichas e no acompanhamento da unidade.
