# Documento Base — CAP-14: Mensageria, APIs e sincronização

**ID:** CAP-14  
**Parte:** VI — Dados, Concorrência e Distribuição  
**Estado:** Planejado — aguardando conclusão de CAP-10 e CAP-13  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** O que garante que uma mensagem reenviada após uma queda de conexão não cobre o cliente duas vezes, e como estruturar sincronização confiável entre aplicações locais e a nuvem (arquitetura *offline-first*)?
* **Objetivo de estudo:** Dominar a semântica de entrega de mensagens (at-most-once, at-least-once, effectively-once), projetar operações rigorosamente idempotentes (*Idempotency Keys*) e compreender estratégias de sincronização bidirecional e resolução de conflitos em clientes desacoplados (*offline-first* / CRDTs).

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Redes falham e reenviam requisições (*retries*). Se o agente implementar uma API de pagamento ou atualização sem chaves de idempotência ou controle de duplicidade, o sistema processará a mesma operação múltiplas vezes. Da mesma forma, IAs tendem a assumir conectividade contínua em aplicações desktop ou mobile.
* **Decisões sob responsabilidade do engenheiro:**
  * Exigir e auditar chaves de idempotência em todas as operações de mutação (POST / mensagens).
  * Projetar filas de mensageria com suporte a Dead Letter Queues (DLQ) e reprocessamento seguro.
  * Escolher estratégias de resolução de conflitos na sincronização (Last-Write-Wins vs. CRDTs / controle por versão).

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-10: Verificação, validação e aceitação](../10-verificacao-validacao-e-aceitacao/documento-base.md) e [CAP-13: Distribuição e consistência](../13-distribuicao-e-consistencia/documento-base.md).
* **Tópicos essenciais:**
  * Semânticas de mensageria: Pelo menos uma vez (*At-least-once*) vs. No máximo uma vez (*At-most-once*).
  * Idempotência matemática e prática: *Idempotency Keys*, tabelas de deduplicação e operações comutativas.
  * Padrão Transacional Outbox (*Transactional Outbox Pattern*) para evitar perda de mensagens.
  * Arquiteturas *Offline-First* e sincronização de dados locais com a nuvem (Local-First Web).
  * Resolução de conflitos em sincronização assíncrona.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Implementação de um endpoint de processamento de cobrança ou atualização com fila que recebe mensagens duplicadas em decorrência de reenvios forçados.
* **Evidência esperada:** Demonstração prática do uso de chave de idempotência impedindo duplicidade de processamento e assegurando o mesmo resultado sem reexecutar efeitos colaterais de pagamento.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 1 (Contratos / Headers)* e *Filtro 2 (Efeitos Colaterais)*.
* **Pergunta de auditoria rápida:** "Se esta requisição ou mensagem for entregue 3 vezes seguidas com a mesma chave, ela executará o débito 3 vezes ou rejeitará as duplicatas de forma idempotente?"

---

## 6. Fontes Primárias de Referência

1. **Enterprise Integration Patterns** — Gregor Hohpe e Bobby Woolf (padrões de mensageria assíncrona e deduplicação).
2. **IETF RFC 9110 — HTTP Semantics:** Definição formal de métodos seguros e métodos idempotentes.
3. **Local-First Software: You own your data, in spite of the cloud** (Onward! 2019) — Martin Kleppmann, Adam Wiggins et al. ([localfirstweb.dev](https://localfirstweb.dev)).

