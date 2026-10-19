# Documento Base — CAP-03: Linguagem e fronteiras de domínio

**ID:** CAP-03  
**Parte:** II — Especificação e Domínio  
**Estado:** Planejado — aguardando conclusão de CAP-02  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como evitar que agentes de IA misturem conceitos de diferentes Ã¡reas de negÃ³cio em um modelo confuso e monolÃ­tico, mantendo termos inequÃ­vocos e fronteiras rÃ­gidas entre subsistemas?
* **Objetivo de estudo:** Aplicar os conceitos estratÃ©gicos do *Domain-Driven Design* (DDD) â€” Linguagem UbÃ­qua (*Ubiquitous Language*), Contextos Delimitados (*Bounded Contexts*) e Mapa de Contextos (*Context Mapping*) â€”, criando modelos semÃ¢nticos claros para orientar a geraÃ§Ã£o e modularizaÃ§Ã£o de cÃ³digo por agentes.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** LLMs sofrem de contaminaÃ§Ã£o semÃ¢ntica: se o termo "Cliente" ou "Conta" tiver significados ligeiramente diferentes no mÃ³dulo de Vendas e no mÃ³dulo Fiscal, o agente unificarÃ¡ tudo em uma Ãºnica classe gigante repleta de campos nulos e condicionais tortuosas.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Fornecer ao agente um vocabulÃ¡rio rigoroso e sem ambiguidade (linguagem ubÃ­qua do domÃ­nio).
  * Desenhar a linha que separa um contexto delimitado do outro.
  * Definir o relacionamento entre contextos (parceria, cliente-fornecedor, nÃºcleo compartilhado ou camada anticorrupÃ§Ã£o - ACL).

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-05: Problema, requisitos e atributos de qualidade](../05-problema-requisitos-e-atributos-de-qualidade/documento-base.md).
* **TÃ³picos essenciais:**
  * Linguagem UbÃ­qua: alinhamento formal entre termos de negÃ³cio, cÃ³digo e prompts dos agentes.
  * Bounded Contexts: fronteiras explÃ­citas onde um modelo conceitual especÃ­fico se aplica e Ã© estritamente vÃ¡lido.
  * Context Mapping: padrÃµes de integraÃ§Ã£o entre contextos (Shared Kernel, Customer-Supplier, Anti-Corruption Layer - ACL).
  * Entidades, Objetos de Valor (*Value Objects*) e Agregados (*Aggregates*) como fronteiras de consistÃªncia transacional.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** Modelagem de um problema que envolva dois domÃ­nios conexos (ex.: Pedidos e Faturamento, ou Vagas e Candidaturas) onde um mesmo termo tem sentidos distintos.
* **EvidÃªncia esperada:** Mapa de contextos visual/documentado com a Linguagem UbÃ­qua de cada contexto delimitado e a definiÃ§Ã£o explÃ­cita de um tradutor/camada anticorrupÃ§Ã£o (ACL) orientando os prompts do agente.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtro em destaque:** *Filtro 1 (Contratos e Tipagem)* e *Filtro 3 (Invariantes)*.
* **Pergunta de auditoria rÃ¡pida:** "Os tipos manipulados neste mÃ³dulo pertencem estritamente a este Bounded Context ou vazaram classes e estruturas internas de outro contexto sem passar por um adaptador/ACL?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Domain-Driven Design: Tackling Complexity in the Heart of Software** â€” Eric Evans (Parte I e IV: Linguagem UbÃ­qua e Design EstratÃ©gico).
2. **Domain-Driven Design Distilled** â€” Vaughn Vernon (resumo essencial de Bounded Contexts e Context Mapping).
3. **Martin Fowler Bliki:** Bounded Context e Bounded Context Mapping ([martinfowler.com/bliki/BoundedContext.html](https://martinfowler.com/bliki/BoundedContext.html)).

