# Documento Base — CAP-15: Evolução e compatibilidade

**ID:** CAP-15  
**Parte:** VII — Evolução, Manutenção e Resiliência em Produção  
**Estado:** Planejado — aguardando conclusão de CAP-09 e CAP-10  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Por que sistemas de software se degradam com o tempo se não forem ativamente adaptados (Leis de Lehman), e como modernizar código legado sem paralisar a produção nem quebrar contratos existentes?
* **Objetivo de estudo:** Compreender as Leis de Evolução de Software de Manny Lehman, a gestão formal do Débito Técnico (Ward Cunningham), Versionamento Semântico (SemVer) e padrões de migração progressiva (*Strangler Fig* e *Expand and Contract*).

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes adoram sugerir "vamos reescrever o sistema do zero em uma nova linguagem/framework", o que quase sempre termina em desastre comercial e operacional. Além disso, a IA gera breaking changes com frequência por não considerar clientes antigos da API ou esquemas de banco de dados pré-existentes.
* **Decisões sob responsabilidade do engenheiro:**
  * Rejeitar reescritas cegas e planejar migrações incrementais seguras (*Strangler Fig*).
  * Aplicar a técnica *Expand and Contract* (adicionar suporte ao novo formato sem remover imediatamente o antigo) em bancos de dados e APIs.
  * Gerenciar a dívida técnica com critérios econômicos, priorizando o que trava a evolução do negócio.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-09: Escolhas arquiteturais](../09-escolhas-arquiteturais/documento-base.md) e [CAP-10: Verificação, validação e aceitação](../10-verificacao-validacao-e-aceitacao/documento-base.md).
* **Tópicos essenciais:**
  * As 8 Leis de Lehman de Evolução de Software (Mudança Contínua, Complexidade Crescente, Declínio de Qualidade).
  * A metáfora da Dívida Técnica (Ward Cunningham) e a Matriz de Débito Técnico (Martin Fowler).
  * Versionamento Semântico (SemVer 2.0.0: MAJOR.MINOR.PATCH) e compatibilidade retroativa.
  * Padrão Strangler Fig (Martin Fowler): substituição gradual de módulos legados por novas implementações.
  * Padrão Expand and Contract (Parallel Change) para migração de esquemas e contratos de dados.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Planejamento e execução de uma mudança de contrato de API e de modelo de dados usando o padrão Expand and Contract com um agente de IA.
* **Evidência esperada:** Documento de plano de migração em 3 etapas demonstrando que tanto a versão antiga quanto a nova funcionam simultaneamente durante o período de transição sem quebra para nenhum cliente.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 1 (Contratos)* e *Filtro 4 (Testes de Regressão)*.
* **Pergunta de auditoria rápida:** "Esta alteração removeu ou renomeou algum campo existente em produção? Os clientes que ainda enviam a versão anterior continuarão funcionando durante a migração?"

---

## 6. Fontes Primárias de Referência

1. **Programs, Life Cycles, and Laws of Software Evolution** (Proc. IEEE, 1980) — M. M. Lehman.
2. **Refactoring: Improving the Design of Existing Code** — Martin Fowler (técnicas de refatoração contínua e Strangler Fig).
3. **Semantic Versioning 2.0.0 Specification** ([semver.org](https://semver.org)).

