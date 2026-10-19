# Documento Base — CAP-07: SDD e rastreabilidade no desenvolvimento

**ID:** CAP-07  
**Parte:** III — Requisitos, Atributos de Qualidade e SDD  
**Estado:** Planejado — aguardando conclusão de CAP-05 e CAP-06  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como estruturar um fluxo de Desenvolvimento Orientado por Especificação (SDD — *Spec-Driven Development*) que garanta rastreabilidade ponta a ponta desde o requisito até o teste automatizado, sem depender de "fé" nas respostas do agente de IA?
* **Objetivo de estudo:** Dominar a disciplina de SDD e matrizes de rastreabilidade, construindo uma cadeia auditável que conecta cada declaração de necessidade a uma especificação formal, a um plano de execução, a tarefas delimitadas e a verificações automatizadas de aceitação.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Quando um desenvolvedor pede tarefas soltas no chat, o agente gera soluções fragmentadas que desviam dos requisitos originais. Sem uma especificação versionada que sirva como "contrato e fonte da verdade", o agente alucina requisitos não solicitados e esquece restrições críticas.
* **Decisões sob responsabilidade do engenheiro:**
  * Autorizar a transição entre fases (especificação -> planejamento -> tarefas -> implementação -> conferência).
  * Manter a rastreabilidade bidirecional (saber exatamente qual requisito gerou qual teste e vice-versa).
  * Auditar o fechamento de tarefas contra a evidência real produzida, rejeitando entregas incompletas.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-05: Problema, requisitos e atributos de qualidade](../05-problema-requisitos-e-atributos-de-qualidade/documento-base.md) e [CAP-06: Linguagem e fronteiras de domínio](../06-linguagem-e-fronteiras-de-dominio/documento-base.md).
* **Tópicos essenciais:**
  * O ciclo SDD: Especificação (*Spec*) -> Planejamento (*Plan*) -> Tarefas (*Tasks*) -> Execução com IA -> Verificação (*Verification*).
  * Matriz de Rastreabilidade de Requisitos (RTM — *Requirements Traceability Matrix*).
  * Limites do SDD com agentes: por que a especificação reduz drasticamente ambiguidades e retrabalho, mas não elimina matematicamente a necessidade de leitura diagnóstica e testes de código.
  * Automação de harness de contexto (como fornecer a spec ao agente de forma sustentável dentro do contexto da janela de atenção).

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Uma funcionalidade pequena conduzida sob fluxo SDD rigoroso, desde a elaboração da spec até a aprovação da entrega.
* **Evidência esperada:** Matriz de rastreabilidade preenchida demonstrando a ligação inequívoca entre Requisito -> ID de Tarefa -> Arquivo de Código -> Cenário de Teste Automatizado correspondente, com registro das lacunas detectadas.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 3 (Invariante por Hipótese com a Spec como Gabarito)* e *Filtro 4 (Auditoria do Teste)*.
* **Pergunta de auditoria rápida:** "A entrega do agente responde estritamente ao contrato da tarefa ou introduziu código não rastreado na especificação?"

---

## 6. Fontes Primárias de Referência

1. **Guia de Operação SDD Editorial / SDD de Software** — [spec editorial/GUIA_DE_OPERACAO.md](../../spec%20editorial/GUIA_DE_OPERACAO.md).
2. **SWEBOK v3/v4** — IEEE Computer Society (tópicos sobre Rastreabilidade de Software e Engenharia de Requisitos).
3. **Spec-Driven Development Principles** — Práticas contemporâneas de condução de agentes com especificações formais.

