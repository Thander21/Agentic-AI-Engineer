# Documento Base — CAP-15: Mensageria, APIs e sincronização

**ID:** CAP-15  
**Parte:** VI — Dados, Concorrência e Distribuição  
**Estado:** Planejado — aguardando conclusão de CAP-06 e CAP-14  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** O que garante que uma mensagem reenviada apÃ³s uma queda de conexÃ£o nÃ£o cobre o cliente duas vezes, e como estruturar sincronizaÃ§Ã£o confiÃ¡vel entre aplicaÃ§Ãµes locais e a nuvem (arquitetura *offline-first*)?
* **Objetivo de estudo:** Dominar a semÃ¢ntica de entrega de mensagens (at-most-once, at-least-once, effectively-once), projetar operaÃ§Ãµes rigorosamente idempotentes (*Idempotency Keys*) e compreender estratÃ©gias de sincronizaÃ§Ã£o bidirecional e resoluÃ§Ã£o de conflitos em clientes desacoplados (*offline-first* / CRDTs).

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Redes falham e reenviam requisiÃ§Ãµes (*retries*). Se o agente implementar uma API de pagamento ou atualizaÃ§Ã£o sem chaves de idempotÃªncia ou controle de duplicidade, o sistema processarÃ¡ a mesma operaÃ§Ã£o mÃºltiplas vezes. Da mesma forma, IAs tendem a assumir conectividade contÃ­nua em aplicaÃ§Ãµes desktop ou mobile.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Exigir e auditar chaves de idempotÃªncia em todas as operaÃ§Ãµes de mutaÃ§Ã£o (POST / mensagens).
  * Projetar filas de mensageria com suporte a Dead Letter Queues (DLQ) e reprocessamento seguro.
  * Escolher estratÃ©gias de resoluÃ§Ã£o de conflitos na sincronizaÃ§Ã£o (Last-Write-Wins vs. CRDTs / controle por versÃ£o).

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-10: VerificaÃ§Ã£o, validaÃ§Ã£o e aceitaÃ§Ã£o](../10-verificacao-validacao-e-aceitacao/documento-base.md) e [CAP-13: DistribuiÃ§Ã£o e consistÃªncia](../13-distribuicao-e-consistencia/documento-base.md).
* **TÃ³picos essenciais:**
  * SemÃ¢nticas de mensageria: Pelo menos uma vez (*At-least-once*) vs. No mÃ¡ximo uma vez (*At-most-once*).
  * IdempotÃªncia matemÃ¡tica e prÃ¡tica: *Idempotency Keys*, tabelas de deduplicaÃ§Ã£o e operaÃ§Ãµes comutativas.
  * PadrÃ£o Transacional Outbox (*Transactional Outbox Pattern*) para evitar perda de mensagens.
  * Arquiteturas *Offline-First* e sincronizaÃ§Ã£o de dados locais com a nuvem (Local-First Web).
  * ResoluÃ§Ã£o de conflitos em sincronizaÃ§Ã£o assÃ­ncrona.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** ImplementaÃ§Ã£o de um endpoint de processamento de cobranÃ§a ou atualizaÃ§Ã£o com fila que recebe mensagens duplicadas em decorrÃªncia de reenvios forÃ§ados.
* **EvidÃªncia esperada:** DemonstraÃ§Ã£o prÃ¡tica do uso de chave de idempotÃªncia impedindo duplicidade de processamento e assegurando o mesmo resultado sem reexecutar efeitos colaterais de pagamento.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 1 (Contratos / Headers)* e *Filtro 2 (Efeitos Colaterais)*.
* **Pergunta de auditoria rÃ¡pida:** "Se esta requisiÃ§Ã£o ou mensagem for entregue 3 vezes seguidas com a mesma chave, ela executarÃ¡ o dÃ©bito 3 vezes ou rejeitarÃ¡ as duplicatas de forma idempotente?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Enterprise Integration Patterns** â€” Gregor Hohpe e Bobby Woolf (padrÃµes de mensageria assÃ­ncrona e deduplicaÃ§Ã£o).
2. **IETF RFC 9110 â€” HTTP Semantics:** DefiniÃ§Ã£o formal de mÃ©todos seguros e mÃ©todos idempotentes.
3. **Local-First Software: You own your data, in spite of the cloud** (Onward! 2019) â€” Martin Kleppmann, Adam Wiggins et al. ([localfirstweb.dev](https://localfirstweb.dev)).

