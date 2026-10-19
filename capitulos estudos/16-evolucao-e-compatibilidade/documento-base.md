# Documento Base — CAP-16: Evolução e compatibilidade

**ID:** CAP-16  
**Parte:** VII — Produção e Soberania  
**Estado:** Planejado — aguardando conclusão de CAP-06 e CAP-09  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Por que sistemas de software se degradam com o tempo se nÃ£o forem ativamente adaptados (Leis de Lehman), e como modernizar cÃ³digo legado sem paralisar a produÃ§Ã£o nem quebrar contratos existentes?
* **Objetivo de estudo:** Compreender as Leis de EvoluÃ§Ã£o de Software de Manny Lehman, a gestÃ£o formal do DÃ©bito TÃ©cnico (Ward Cunningham), Versionamento SemÃ¢ntico (SemVer) e padrÃµes de migraÃ§Ã£o progressiva (*Strangler Fig* e *Expand and Contract*).

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes adoram sugerir "vamos reescrever o sistema do zero em uma nova linguagem/framework", o que quase sempre termina em desastre comercial e operacional. AlÃ©m disso, a IA gera breaking changes com frequÃªncia por nÃ£o considerar clientes antigos da API ou esquemas de banco de dados prÃ©-existentes.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Rejeitar reescritas cegas e planejar migraÃ§Ãµes incrementais seguras (*Strangler Fig*).
  * Aplicar a tÃ©cnica *Expand and Contract* (adicionar suporte ao novo formato sem remover imediatamente o antigo) em bancos de dados e APIs.
  * Gerenciar a dÃ­vida tÃ©cnica com critÃ©rios econÃ´micos, priorizando o que trava a evoluÃ§Ã£o do negÃ³cio.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-09: Escolhas arquiteturais](../09-escolhas-arquiteturais/documento-base.md) e [CAP-10: VerificaÃ§Ã£o, validaÃ§Ã£o e aceitaÃ§Ã£o](../10-verificacao-validacao-e-aceitacao/documento-base.md).
* **TÃ³picos essenciais:**
  * As 8 Leis de Lehman de EvoluÃ§Ã£o de Software (MudanÃ§a ContÃ­nua, Complexidade Crescente, DeclÃ­nio de Qualidade).
  * A metÃ¡fora da DÃ­vida TÃ©cnica (Ward Cunningham) e a Matriz de DÃ©bito TÃ©cnico (Martin Fowler).
  * Versionamento SemÃ¢ntico (SemVer 2.0.0: MAJOR.MINOR.PATCH) e compatibilidade retroativa.
  * PadrÃ£o Strangler Fig (Martin Fowler): substituiÃ§Ã£o gradual de mÃ³dulos legados por novas implementaÃ§Ãµes.
  * PadrÃ£o Expand and Contract (Parallel Change) para migraÃ§Ã£o de esquemas e contratos de dados.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** Planejamento e execuÃ§Ã£o de uma mudanÃ§a de contrato de API e de modelo de dados usando o padrÃ£o Expand and Contract com um agente de IA.
* **EvidÃªncia esperada:** Documento de plano de migraÃ§Ã£o em 3 etapas demonstrando que tanto a versÃ£o antiga quanto a nova funcionam simultaneamente durante o perÃ­odo de transiÃ§Ã£o sem quebra para nenhum cliente.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 1 (Contratos)* e *Filtro 4 (Testes de RegressÃ£o)*.
* **Pergunta de auditoria rÃ¡pida:** "Esta alteraÃ§Ã£o removeu ou renomeou algum campo existente em produÃ§Ã£o? Os clientes que ainda enviam a versÃ£o anterior continuarÃ£o funcionando durante a migraÃ§Ã£o?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Programs, Life Cycles, and Laws of Software Evolution** (Proc. IEEE, 1980) â€” M. M. Lehman.
2. **Refactoring: Improving the Design of Existing Code** â€” Martin Fowler (tÃ©cnicas de refatoraÃ§Ã£o contÃ­nua e Strangler Fig).
3. **Semantic Versioning 2.0.0 Specification** ([semver.org](https://semver.org)).

