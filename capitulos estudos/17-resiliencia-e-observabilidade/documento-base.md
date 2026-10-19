# Documento Base — CAP-17: Resiliência e observabilidade

**ID:** CAP-17  
**Parte:** VII — Produção e Soberania  
**Estado:** Planejado — aguardando conclusão de CAP-12 e CAP-15  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como evitar que uma falha em uma dependÃªncia externa derrube em efeito dominÃ³ todo o nosso sistema em produÃ§Ã£o, e como saber exatamente o que aconteceu quando um erro silencioso ocorre Ã s 3h da manhÃ£?
* **Objetivo de estudo:** Dominar padrÃµes formais de estabilidade e resiliÃªncia (Circuit Breaker, Bulkhead, Retry com Exponential Backoff e Jitter, Timeouts rigorosos) e os trÃªs pilares da Observabilidade moderna (MÃ©tricas, Logs estruturados e Tracing distribuÃ­do com OpenTelemetry).

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** IAs costumam implementar retentativas simples (`while error: retry()`) que funcionam como um ataque de negaÃ§Ã£o de serviÃ§o (DoS) autoinduzido contra o servidor que acabou de ficar instÃ¡vel (*Thundering Herd problem*). AlÃ©m disso, IAs criam logs em texto livre desestruturados que sÃ£o impossÃ­veis de filtrar e correlacionar em escala.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Exigir Circuit Breakers e Timeouts explÃ­citos em todas as fronteiras externas.
  * Configurar polÃ­ticas de reintento seguras com crescimento exponencial e jitter aleatÃ³rio.
  * Padronizar telemetria com IDs de correlaÃ§Ã£o (*TraceID* / *SpanID*) em conformidade com o OpenTelemetry.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-04: Qualidade, mÃ©tricas e profiling](../04-qualidade-metricas-e-profiling/documento-base.md) e [CAP-14: Mensageria, APIs e sincronizaÃ§Ã£o](../14-mensageria-apis-e-sincronizacao/documento-base.md).
* **TÃ³picos essenciais:**
  * PadrÃµes de Estabilidade (Michael Nygard): Circuit Breaker (estados Fechado, Aberto e Meio-Aberto), Bulkheads (isolamento de pools de recursos) e Timeouts compulsÃ³rios.
  * PolÃ­ticas de Retry: Backoff Exponencial e Jitter (adicionar aleatoriedade para dispersar picos de trÃ¡fego).
  * Os TrÃªs Pilares da Observabilidade: Logs Estruturados (JSON), MÃ©tricas (RED / USE metrics) e Rastreamento DistribuÃ­do (*Distributed Tracing*).
  * O padrÃ£o OpenTelemetry (OTel): Traces, Spans, Context Propagation e instrumentos de telemetria.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** Uma chamada de serviÃ§o instÃ¡vel submetida a um Circuit Breaker com Retry e Jitter, instrumentada com tracing OpenTelemetry para diagnosticar a contenÃ§Ã£o.
* **EvidÃªncia esperada:** DemonstraÃ§Ã£o do Circuit Breaker abrindo apÃ³s falhas consecutivas, impedindo novas requisiÃ§Ãµes de sobrecarregar o serviÃ§o externo, acompanhada pelo rastreamento do Span identificando o gargalo de latÃªncia.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 2 (Efeitos Colaterais / Rede)* e *Filtro 5 (InspeÃ§Ã£o Viva e Telemetria)*.
* **Pergunta de auditoria rÃ¡pida:** "Esta chamada externa possui timeout configurado? Se ela falhar repetidamente, ela entra em loop imediato ou usa backoff exponencial com jitter?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Release It!: Design and Deploy Production-Ready Software** â€” Michael T. Nygard (capÃ­tulos sobre Circuit Breaker, Bulkheads e Falhas em Cascata).
2. **Exponential Backoff And Jitter** â€” Marc Brooker (AWS Architecture Blog).
3. **OpenTelemetry Documentation & Specifications** ([opentelemetry.io](https://opentelemetry.io)).

