# Documento Base — CAP-06: Linguagem e fronteiras de domínio

**ID:** CAP-06  
**Parte:** III — Requisitos, Atributos de Qualidade e SDD  
**Estado:** Planejado — aguardando conclusão de CAP-05  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como evitar que agentes de IA misturem conceitos de diferentes áreas de negócio em um modelo confuso e monolítico, mantendo termos inequívocos e fronteiras rígidas entre subsistemas?
* **Objetivo de estudo:** Aplicar os conceitos estratégicos do *Domain-Driven Design* (DDD) — Linguagem Ubíqua (*Ubiquitous Language*), Contextos Delimitados (*Bounded Contexts*) e Mapa de Contextos (*Context Mapping*) —, criando modelos semânticos claros para orientar a geração e modularização de código por agentes.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** LLMs sofrem de contaminação semântica: se o termo "Cliente" ou "Conta" tiver significados ligeiramente diferentes no módulo de Vendas e no módulo Fiscal, o agente unificará tudo em uma única classe gigante repleta de campos nulos e condicionais tortuosas.
* **Decisões sob responsabilidade do engenheiro:**
  * Fornecer ao agente um vocabulário rigoroso e sem ambiguidade (linguagem ubíqua do domínio).
  * Desenhar a linha que separa um contexto delimitado do outro.
  * Definir o relacionamento entre contextos (parceria, cliente-fornecedor, núcleo compartilhado ou camada anticorrupção - ACL).

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-05: Problema, requisitos e atributos de qualidade](../05-problema-requisitos-e-atributos-de-qualidade/documento-base.md).
* **Tópicos essenciais:**
  * Linguagem Ubíqua: alinhamento formal entre termos de negócio, código e prompts dos agentes.
  * Bounded Contexts: fronteiras explícitas onde um modelo conceitual específico se aplica e é estritamente válido.
  * Context Mapping: padrões de integração entre contextos (Shared Kernel, Customer-Supplier, Anti-Corruption Layer - ACL).
  * Entidades, Objetos de Valor (*Value Objects*) e Agregados (*Aggregates*) como fronteiras de consistência transacional.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Modelagem de um problema que envolva dois domínios conexos (ex.: Pedidos e Faturamento, ou Vagas e Candidaturas) onde um mesmo termo tem sentidos distintos.
* **Evidência esperada:** Mapa de contextos visual/documentado com a Linguagem Ubíqua de cada contexto delimitado e a definição explícita de um tradutor/camada anticorrupção (ACL) orientando os prompts do agente.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtro em destaque:** *Filtro 1 (Contratos e Tipagem)* e *Filtro 3 (Invariantes)*.
* **Pergunta de auditoria rápida:** "Os tipos manipulados neste módulo pertencem estritamente a este Bounded Context ou vazaram classes e estruturas internas de outro contexto sem passar por um adaptador/ACL?"

---

## 6. Fontes Primárias de Referência

1. **Domain-Driven Design: Tackling Complexity in the Heart of Software** — Eric Evans (Parte I e IV: Linguagem Ubíqua e Design Estratégico).
2. **Domain-Driven Design Distilled** — Vaughn Vernon (resumo essencial de Bounded Contexts e Context Mapping).
3. **Martin Fowler Bliki:** Bounded Context e Bounded Context Mapping ([martinfowler.com/bliki/BoundedContext.html](https://martinfowler.com/bliki/BoundedContext.html)).

