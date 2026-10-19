# Documento Base — CAP-12: Qualidade, métricas e profiling

**ID:** CAP-12  
**Parte:** V — Computação e Runtime  
**Estado:** Planejado — aguardando conclusão de CAP-10 e CAP-11  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como utilizar ferramentas automatizadas de anÃ¡lise estÃ¡tica (SAST, linters) e mÃ©tricas formais de cÃ³digo para rejeitar cÃ³digo defeituoso gerado pela IA antes mesmo de executÃ¡-lo, e como usar profiling para diagnosticar gargalos reais?
* **Objetivo de estudo:** Interpretar mÃ©tricas quantitativas de engenharia de software (complexidade ciclomÃ¡tica, acoplamento aferente/eferente, mÃ©tricas de Halstead) e aplicar profiling de runtime (tempo de CPU, grÃ¡ficos de memÃ³ria, traÃ§os de execuÃ§Ã£o), compreendendo o que cada sinal prova e quais sÃ£o seus limites.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes tendem a resolver problemas aninhando mÃºltiplos blocos condicionais, criando "funÃ§Ãµes monstro" com alta complexidade ciclomÃ¡tica e acoplamento descontrolado. Sem ferramentas objetivas de controle de qualidade (*quality gates*), o repositÃ³rio se degrada rapidamente em dÃ©bito tÃ©cnico.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Estabelecer regras e limiares estÃ¡ticos no pipeline de IA (ex.: rejeitar funÃ§Ãµes com complexidade ciclomÃ¡tica acima de 10).
  * Interpretar relatÃ³rios de SAST (seguranÃ§a estÃ¡tica) sem se perder em falsos positivos ou falsos negativos.
  * Analisar dados de profiler de CPU e memÃ³ria para distinguir problemas reais de lentidÃ£o de micro-otimizaÃ§Ãµes prematuras.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-02: Processos, threads e I/O](../02-processos-threads-e-io/documento-base.md) e [CAP-03: Contratos e leitura diagnÃ³stica](../03-contratos-e-leitura-diagnostica/documento-base.md).
* **TÃ³picos essenciais:**
  * Complexidade CiclomÃ¡tica (Thomas McCabe): contagem de caminhos de execuÃ§Ã£o linearmente independentes e propensÃ£o a defeitos.
  * Acoplamento Aferente ($Ca$) e Eferente ($Ce$), Instabilidade ($I$) e DistÃ¢ncia da SequÃªncia Principal (Robert Martin).
  * MÃ©tricas de Halstead: operadores, operandos, volume e esforÃ§o mental.
  * AnÃ¡lise EstÃ¡tica de SeguranÃ§a (SAST) e Linters: regras de qualidade automatizadas.
  * Profiling: flame graphs, amostragem de chamadas (*sampling*), alocaÃ§Ãµes por tipo e detecÃ§Ã£o de pontos quentes (*hotspots*).

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** SubmissÃ£o de um mÃ³dulo gerado por IA contendo alta complexidade oculta e um hotspot de processamento a um linter/analisador estÃ¡tico e a uma ferramenta de profiling (ex.: Dart DevTools Profiler).
* **EvidÃªncia esperada:** RelatÃ³rio de auditoria tÃ©cnica contrastando a mediÃ§Ã£o estÃ¡tica (complexidade calculada) e o comportamento dinÃ¢mico (tempo no flame graph), fundamentando a decisÃ£o de refatoraÃ§Ã£o pelo agente.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtro em destaque:** *Filtro 5 (InspeÃ§Ã£o Viva / Telemetria)* e *Filtro 2 (Efeitos Colaterais)*.
* **Pergunta de auditoria rÃ¡pida:** "Qual Ã© a profundidade de aninhamento e o nÃºmero de bifurcaÃ§Ãµes desta funÃ§Ã£o? O que a ferramenta de anÃ¡lise estÃ¡tica ou o profiler revelam sobre o consumo de ciclos nessa rotina?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **A Complexity Measure** (IEEE Transactions on Software Engineering, 1976) â€” Thomas J. McCabe.
2. **Agile Software Development: Principles, Patterns, and Practices** â€” Robert C. Martin (capÃ­tulo sobre MÃ©tricas de Pacotes e Acoplamento).
3. **Dart/Flutter DevTools CPU Profiler Guide:** InterpretaÃ§Ã£o de flame graphs, call tree e bottom-up table ([docs.flutter.dev/tools/devtools/cpu-profiler](https://docs.flutter.dev/tools/devtools/cpu-profiler)).

