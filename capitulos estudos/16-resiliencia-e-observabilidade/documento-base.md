# Documento Base — CAP-16: Resiliência e observabilidade

**ID:** CAP-16  
**Parte:** VII — Evolução, Manutenção e Resiliência em Produção  
**Estado:** Planejado — aguardando conclusão de CAP-04 e CAP-14  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como evitar que uma falha em uma dependência externa derrube em efeito dominó todo o nosso sistema em produção, e como saber exatamente o que aconteceu quando um erro silencioso ocorre às 3h da manhã?
* **Objetivo de estudo:** Dominar padrões formais de estabilidade e resiliência (Circuit Breaker, Bulkhead, Retry com Exponential Backoff e Jitter, Timeouts rigorosos) e os três pilares da Observabilidade moderna (Métricas, Logs estruturados e Tracing distribuído com OpenTelemetry).

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** IAs costumam implementar retentativas simples (`while error: retry()`) que funcionam como um ataque de negação de serviço (DoS) autoinduzido contra o servidor que acabou de ficar instável (*Thundering Herd problem*). Além disso, IAs criam logs em texto livre desestruturados que são impossíveis de filtrar e correlacionar em escala.
* **Decisões sob responsabilidade do engenheiro:**
  * Exigir Circuit Breakers e Timeouts explícitos em todas as fronteiras externas.
  * Configurar políticas de reintento seguras com crescimento exponencial e jitter aleatório.
  * Padronizar telemetria com IDs de correlação (*TraceID* / *SpanID*) em conformidade com o OpenTelemetry.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-04: Qualidade, métricas e profiling](../04-qualidade-metricas-e-profiling/documento-base.md) e [CAP-14: Mensageria, APIs e sincronização](../14-mensageria-apis-e-sincronizacao/documento-base.md).
* **Tópicos essenciais:**
  * Padrões de Estabilidade (Michael Nygard): Circuit Breaker (estados Fechado, Aberto e Meio-Aberto), Bulkheads (isolamento de pools de recursos) e Timeouts compulsórios.
  * Políticas de Retry: Backoff Exponencial e Jitter (adicionar aleatoriedade para dispersar picos de tráfego).
  * Os Três Pilares da Observabilidade: Logs Estruturados (JSON), Métricas (RED / USE metrics) e Rastreamento Distribuído (*Distributed Tracing*).
  * O padrão OpenTelemetry (OTel): Traces, Spans, Context Propagation e instrumentos de telemetria.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Uma chamada de serviço instável submetida a um Circuit Breaker com Retry e Jitter, instrumentada com tracing OpenTelemetry para diagnosticar a contenção.
* **Evidência esperada:** Demonstração do Circuit Breaker abrindo após falhas consecutivas, impedindo novas requisições de sobrecarregar o serviço externo, acompanhada pelo rastreamento do Span identificando o gargalo de latência.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 2 (Efeitos Colaterais / Rede)* e *Filtro 5 (Inspeção Viva e Telemetria)*.
* **Pergunta de auditoria rápida:** "Esta chamada externa possui timeout configurado? Se ela falhar repetidamente, ela entra em loop imediato ou usa backoff exponencial com jitter?"

---

## 6. Fontes Primárias de Referência

1. **Release It!: Design and Deploy Production-Ready Software** — Michael T. Nygard (capítulos sobre Circuit Breaker, Bulkheads e Falhas em Cascata).
2. **Exponential Backoff And Jitter** — Marc Brooker (AWS Architecture Blog).
3. **OpenTelemetry Documentation & Specifications** ([opentelemetry.io](https://opentelemetry.io)).

