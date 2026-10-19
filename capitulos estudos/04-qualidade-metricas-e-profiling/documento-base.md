# Documento Base — CAP-04: Qualidade, métricas e profiling

**ID:** CAP-04  
**Parte:** II — Garantia da Qualidade, Métricas e Auditoria  
**Estado:** Planejado — aguardando conclusão de CAP-02 e CAP-03  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como utilizar ferramentas automatizadas de análise estática (SAST, linters) e métricas formais de código para rejeitar código defeituoso gerado pela IA antes mesmo de executá-lo, e como usar profiling para diagnosticar gargalos reais?
* **Objetivo de estudo:** Interpretar métricas quantitativas de engenharia de software (complexidade ciclomática, acoplamento aferente/eferente, métricas de Halstead) e aplicar profiling de runtime (tempo de CPU, gráficos de memória, traços de execução), compreendendo o que cada sinal prova e quais são seus limites.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes tendem a resolver problemas aninhando múltiplos blocos condicionais, criando "funções monstro" com alta complexidade ciclomática e acoplamento descontrolado. Sem ferramentas objetivas de controle de qualidade (*quality gates*), o repositório se degrada rapidamente em débito técnico.
* **Decisões sob responsabilidade do engenheiro:**
  * Estabelecer regras e limiares estáticos no pipeline de IA (ex.: rejeitar funções com complexidade ciclomática acima de 10).
  * Interpretar relatórios de SAST (segurança estática) sem se perder em falsos positivos ou falsos negativos.
  * Analisar dados de profiler de CPU e memória para distinguir problemas reais de lentidão de micro-otimizações prematuras.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-02: Processos, threads e I/O](../02-processos-threads-e-io/documento-base.md) e [CAP-03: Contratos e leitura diagnóstica](../03-contratos-e-leitura-diagnostica/documento-base.md).
* **Tópicos essenciais:**
  * Complexidade Ciclomática (Thomas McCabe): contagem de caminhos de execução linearmente independentes e propensão a defeitos.
  * Acoplamento Aferente ($Ca$) e Eferente ($Ce$), Instabilidade ($I$) e Distância da Sequência Principal (Robert Martin).
  * Métricas de Halstead: operadores, operandos, volume e esforço mental.
  * Análise Estática de Segurança (SAST) e Linters: regras de qualidade automatizadas.
  * Profiling: flame graphs, amostragem de chamadas (*sampling*), alocações por tipo e detecção de pontos quentes (*hotspots*).

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Submissão de um módulo gerado por IA contendo alta complexidade oculta e um hotspot de processamento a um linter/analisador estático e a uma ferramenta de profiling (ex.: Dart DevTools Profiler).
* **Evidência esperada:** Relatório de auditoria técnica contrastando a medição estática (complexidade calculada) e o comportamento dinâmico (tempo no flame graph), fundamentando a decisão de refatoração pelo agente.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtro em destaque:** *Filtro 5 (Inspeção Viva / Telemetria)* e *Filtro 2 (Efeitos Colaterais)*.
* **Pergunta de auditoria rápida:** "Qual é a profundidade de aninhamento e o número de bifurcações desta função? O que a ferramenta de análise estática ou o profiler revelam sobre o consumo de ciclos nessa rotina?"

---

## 6. Fontes Primárias de Referência

1. **A Complexity Measure** (IEEE Transactions on Software Engineering, 1976) — Thomas J. McCabe.
2. **Agile Software Development: Principles, Patterns, and Practices** — Robert C. Martin (capítulo sobre Métricas de Pacotes e Acoplamento).
3. **Dart/Flutter DevTools CPU Profiler Guide:** Interpretação de flame graphs, call tree e bottom-up table ([docs.flutter.dev/tools/devtools/cpu-profiler](https://docs.flutter.dev/tools/devtools/cpu-profiler)).

