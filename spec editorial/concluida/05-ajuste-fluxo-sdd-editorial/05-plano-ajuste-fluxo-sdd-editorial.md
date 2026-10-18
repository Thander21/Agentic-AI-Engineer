# Plano 05 — Ajuste do fluxo SDD editorial

**ID:** PLANO-EDITORIAL-005  
**Versão:** 0.1 — 17/10/2026  
**Base:** [spec 05 v0.6](05-spec-ajuste-fluxo-sdd-editorial.md), parecer apto para planejamento.  
**Acompanhamento:** [tasks 05](05-tasks-ajuste-fluxo-sdd-editorial.md).

## Entregas e cobertura

Base dos caminhos: raiz do repositório. Nenhuma alteração do kit ou da prosa pública integra este plano.

| Entrega | Documentos afetados e resultado | Requisitos | Dependência / conferência |
| --- | --- | --- | --- |
| ENT05-01 | `AGENTS.md`, `spec editorial/README.md` e `GUIA_DE_OPERACAO.md`: entrada curta, autoridade, fases e sequência editorial vigente. | R05-01/02/03/04/05/08/10/11/12 | Spec conferida. Comparar instruções entre documentos e com 4.1–4.5 da spec. |
| ENT05-02 | Sete `spec editorial/skills/*/SKILL.md`, seis `spec editorial/modelos/*.md` e referência P09: interfaces proporcionais e sequência revisão → integração → reconferência → autor → ajustes → prova. | R05-02/03/04/05/08/10/11/12 | ENT05-01. Validar estrutura das skills e examinar a responsabilidade de cada passagem; modelos não são relatórios obrigatórios. |
| ENT05-03 | Spec/plano/tasks 03, índice de publicações e metadados de navegação da ficha: estado único, reutilização do produzido, prova final depois do autor. Notas de vigência em 01/04 quando pertinentes. | R05-01/02/06/07/08/10/11/12 | ENT05-01/02. Preservar IDs e resultados de T03-007/008 como ocorridos; não duplicar suas execuções. Corpo de PUB-000/PUB-001, estudos e jornada fora da edição. |
| ENT05-04 | Conferência V05-01–08, referências e prontidão nas próprias tasks; atualização da dependência de 03. | R05-01–12, especialmente R05-09/10 | ENT05-01–03. Conferir os contratos com material existente e individualizar cobertura não exercitada. Sem eficácia editorial ou apreciação humana presumidas. |

## Decisões de execução

- Manter spec/plano/tasks separados para esta correção do método. A sequência editorial aplica-se às peças dentro das iniciativas e não exige uma nova cadeia documental por texto pequeno.
- Reduzir modelos e repetição nas skills; manter a referência dos nove perfis como consulta seletiva. Guia é o procedimento comum, skills descrevem a ação de cada papel.
- D05-01: solicitar commit apenas quando uma versão de publicação, jornada ou estudo precisar ser preservada e não estiver no Git. Nesta execução, preservar integralmente os corpos dos textos; navegação e acompanhamento não iniciam revisão da prosa. Se a edição revelar necessidade de mudar conteúdo, interromper essa parte antes de sobrescrever.
- A evolução é implementada em 05; 01/04 conservam a evidência histórica. Reabrir aceitação apenas se uma conclusão anterior for invalidada, identificando o aspecto. Não reabrir pela simples atualização do procedimento.
- Uma mesma IA planeja, implementa e confere com histórico disponível, sem independência alegada. Não executar motor, testes ou scripts do SpecSimpleKit. A referência SDD orienta requisito → entrega → tarefa → evidência.

## Parecer pré-execução

**Apto para tasks e execução no escopo autorizado pelo autor.** As quatro entregas cobrem os doze requisitos, dependências são sequenciais e não exigem retorno do piloto para conferir o método. V05-01–08 estão definidos antes das mudanças. Plano e tasks serão conferidos entre si antes da implementação; nenhum resultado futuro está marcado concluído neste documento.

Mudança de requisito volta à spec; mudança de estratégia atualiza este plano; resultado fica nas tasks. Conclusão desta correção libera a dependência de método de 03, sem escrever chamada ou publicar.
