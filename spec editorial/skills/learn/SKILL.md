---
name: learn
description: Consolida aprendizados editoriais sobre fluxo, regras, skills e produção/revisão de textos, propondo melhorias e encaminhando conteúdo e pendências às fontes próprias. Use ao pedir learn, retrospectiva ou fechamento com lições; não substitui revisão de texto ou aprovação autoral.
metadata:
  version: "0.2"
---

# Aprender com a sessão editorial

Adaptação da skill `learn` de `C:/_Projetos/ERP PDV D+/.claude/skills/learn/SKILL.md`, consultada em 18/10/2026, SHA-256 `37e40913d5b9ad75b180ac877a661fe350e0f62a48096d44e3a02c07dc456245`. Reaproveita a separação entre regra, pendência e preferência; não importa caminhos operacionais, gates de software ou memória do Claude Code. Esta cópia é específica deste projeto e pode ser lida por qualquer agente, conforme o [AGENTS](../../../AGENTS.md).

## Escopo editorial

Examinar como o trabalho foi preparado, escrito, revisado, integrado e coordenado: decisões de leitura, qualidade dos textos, uso das skills, retorno autoral e retrabalho. Não exigir código, testes de aplicação, build, deploy ou gate do projeto-fonte. Git serve apenas para rastrear versões; o diagnóstico pode ocorrer sem commit. A validação estrutural de uma skill examina suas instruções, não transforma o acervo em projeto de software.

Distinguir aprendizado sobre o método de conhecimento adquirido no conteúdo. Não reescrever uma peça aprovada, inventar vivência, iniciar estudo técnico ou transformar um relato pessoal em regra por consequência do learn.

## Entrada e evidência

Receber pedido/foco, contexto disponível, artefatos e retornos do autor. Sem foco explícito, examinar a sessão até o escopo autorizado, sem carregar todo o acervo.

- Se a conversa identificar um commit, conferir essa referência com `git show <ref>` e os arquivos pertinentes. Não presumir que HEAD ou `git log -1` corresponde à sessão. Mensagem de commit não prova todos os resultados descritos.
- Confrontar as lições com o conteúdo efetivo, decisões e pareceres. Declarar perda de contexto ou versão não recuperável; não reconstruir comparação exata por lembrança.
- Consultar [guia](../../GUIA_DE_OPERACAO.md) e acompanhamento da iniciativa. Identificar causa, efeito observado, correção e limite; não confundir ausência de erro factual com qualidade de voz, interesse ou narrativa.

## Selecionar e encaminhar

| Tipo | Critério e destino |
| --- | --- |
| Regra reutilizável | Mudaria uma decisão numa tarefa futura semelhante? Conferir se já está atendida. Procedimento na skill da fase; passagem comum no guia; somente invariantes/roteamento no AGENTS. Propor refinamento da fonte existente, sem copiar a regra em vários lugares. |
| Conhecimento de conteúdo | Se houver relato ou fonte suficiente, encaminhar o conhecimento à jornada ou ao estudo pertinente, com origem e limites. Não guardar história, pesquisa ou capítulo dentro da skill; editar o conteúdo somente no escopo autorizado. |
| Pendência ou hipótese | Encaminhar à task/spec pertinente; uma hipótese não vira regra pela repetição. Usar backlog apenas para escopo novo, sem abrir iniciativa duplicada ou tarefa vazia. |
| Preferência ou decisão autoral | Distinguir escolha desta peça, orientação do projeto e preferência pessoal. A escolha editorial aceita pertence à ficha/spec; a preferência privada não vai para o repositório. Não escrever em memória externa ou no ambiente de outro agente sem autorização explícita e mecanismo disponível. |

Para mudança de regra, apresentar arquivo, trecho antes/depois, evidência da sessão, ganho e possível custo. **Propor antes de aplicar e aguardar confirmação**, salvo se o pedido já autorizar de forma explícita a aplicação da mudança identificada. Pedido de rodar `learn` autoriza diagnóstico e encaminhamento, não aprovação genérica de qualquer regra nova. Uma decisão autoral já recebida não precisa ser perguntada novamente; registrar o conflito exato e o alcance da autorização existente.

Usar o acompanhamento existente para os resultados autorizados. Sem edição autorizada, entregar o parecer no chat. Não criar diário de sessão, relatório paralelo de learn, pasta de snapshots ou lista de lições dentro da skill. Fontes, textos e histórias permanecem nas áreas próprias. Não exigir lição em todos os tipos; informar quando não houver achado.

## Conferir e encerrar

- Verificar duplicação, intenção, limites e vínculos dos documentos alterados. Para skill nova/alterada, executar o validador estrutural disponível e examinar o procedimento em casos pertinentes; estrutura válida não comprova qualidade editorial.
- Separar observado em peça real, hipótese de melhoria, instrução criada e comportamento ainda não exercitado. Retorno favorável às peças não valida o método inteiro. Não inventar métricas de tempo, esforço ou causalidade.
- Registrar aprendizado, evidência, destino, estado e próxima ação uma vez nas tasks quando a iniciativa as possuir. Se a avaliação formal do piloto exigir mais critérios, `learn` parcial não a conclui.
- Entregar ref/contexto usados, lições selecionadas, alterações aplicadas versus propostas, conferência e pendências. Não fazer commit, push, publicação ou delegação automaticamente.
