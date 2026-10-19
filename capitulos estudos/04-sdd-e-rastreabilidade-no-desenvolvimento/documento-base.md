# Documento Base — CAP-04: SDD e rastreabilidade no desenvolvimento

**ID:** CAP-04  
**Parte:** II — Especificação e Domínio  
**Estado:** Planejado — aguardando conclusão de CAP-02 e CAP-03  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como estruturar um fluxo de Desenvolvimento Orientado por EspecificaÃ§Ã£o (SDD â€” *Spec-Driven Development*) que garanta rastreabilidade ponta a ponta desde o requisito atÃ© o teste automatizado, sem depender de "fÃ©" nas respostas do agente de IA?
* **Objetivo de estudo:** Dominar a disciplina de SDD e matrizes de rastreabilidade, construindo uma cadeia auditÃ¡vel que conecta cada declaraÃ§Ã£o de necessidade a uma especificaÃ§Ã£o formal, a um plano de execuÃ§Ã£o, a tarefas delimitadas e a verificaÃ§Ãµes automatizadas de aceitaÃ§Ã£o.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Quando um desenvolvedor pede tarefas soltas no chat, o agente gera soluÃ§Ãµes fragmentadas que desviam dos requisitos originais. Sem uma especificaÃ§Ã£o versionada que sirva como "contrato e fonte da verdade", o agente alucina requisitos nÃ£o solicitados e esquece restriÃ§Ãµes crÃ­ticas.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Autorizar a transiÃ§Ã£o entre fases (especificaÃ§Ã£o -> planejamento -> tarefas -> implementaÃ§Ã£o -> conferÃªncia).
  * Manter a rastreabilidade bidirecional (saber exatamente qual requisito gerou qual teste e vice-versa).
  * Auditar o fechamento de tarefas contra a evidÃªncia real produzida, rejeitando entregas incompletas.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-05: Problema, requisitos e atributos de qualidade](../05-problema-requisitos-e-atributos-de-qualidade/documento-base.md) e [CAP-06: Linguagem e fronteiras de domÃ­nio](../06-linguagem-e-fronteiras-de-dominio/documento-base.md).
* **TÃ³picos essenciais:**
  * O ciclo SDD: EspecificaÃ§Ã£o (*Spec*) -> Planejamento (*Plan*) -> Tarefas (*Tasks*) -> ExecuÃ§Ã£o com IA -> VerificaÃ§Ã£o (*Verification*).
  * Matriz de Rastreabilidade de Requisitos (RTM â€” *Requirements Traceability Matrix*).
  * Limites do SDD com agentes: por que a especificaÃ§Ã£o reduz drasticamente ambiguidades e retrabalho, mas nÃ£o elimina matematicamente a necessidade de leitura diagnÃ³stica e testes de cÃ³digo.
  * AutomaÃ§Ã£o de harness de contexto (como fornecer a spec ao agente de forma sustentÃ¡vel dentro do contexto da janela de atenÃ§Ã£o).

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** Uma funcionalidade pequena conduzida sob fluxo SDD rigoroso, desde a elaboraÃ§Ã£o da spec atÃ© a aprovaÃ§Ã£o da entrega.
* **EvidÃªncia esperada:** Matriz de rastreabilidade preenchida demonstrando a ligaÃ§Ã£o inequÃ­voca entre Requisito -> ID de Tarefa -> Arquivo de CÃ³digo -> CenÃ¡rio de Teste Automatizado correspondente, com registro das lacunas detectadas.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 3 (Invariante por HipÃ³tese com a Spec como Gabarito)* e *Filtro 4 (Auditoria do Teste)*.
* **Pergunta de auditoria rÃ¡pida:** "A entrega do agente responde estritamente ao contrato da tarefa ou introduziu cÃ³digo nÃ£o rastreado na especificaÃ§Ã£o?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Guia de OperaÃ§Ã£o SDD Editorial / SDD de Software** â€” [spec editorial/GUIA_DE_OPERACAO.md](../../spec%20editorial/GUIA_DE_OPERACAO.md).
2. **SWEBOK v3/v4** â€” IEEE Computer Society (tÃ³picos sobre Rastreabilidade de Software e Engenharia de Requisitos).
3. **Spec-Driven Development Principles** â€” PrÃ¡ticas contemporÃ¢neas de conduÃ§Ã£o de agentes com especificaÃ§Ãµes formais.

