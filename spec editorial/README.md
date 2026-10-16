# Organização das iniciativas editoriais

As iniciativas seguem o fluxo **backlog → changes → concluida**. Cada iniciativa tem uma pasta própria; spec, plano e tasks ficam juntos quando esses documentos existirem. Não criar plano ou tasks vazios só para completar a pasta.

| Pasta | Finalidade | Condição de passagem |
| --- | --- | --- |
| `backlog/` | Iniciativas previstas, ainda não selecionadas para trabalho ativo. Podem conter análise preliminar e dependências. | Ao escolher a próxima iniciativa para análise ou execução, mover sua pasta para `changes/`. |
| `changes/` | Iniciativa em análise, especificação, planejamento ou execução. | Mover para `concluida/` após conferir o escopo, corrigir impeditivos e registrar evidências e destino explícito de eventuais transferências autorizadas. |
| `concluida/` | Iniciativas encerradas, com spec, plano, tasks e histórico de decisões consultáveis. | Se um defeito exigir reabertura, registrar motivo e aspecto afetado e devolver a iniciativa a `changes/`; correção de link não reabre o conteúdo. |

A pasta indica a situação da iniciativa, não substitui o estado de cada tarefa ou a versão dos documentos. Estar em `changes/` não autoriza automaticamente escrever, publicar ou executar todas as fases. Preservar IDs e evidências ao mover e atualizar os links de entrada e saída. Não manter cópias concorrentes da mesma spec em backlog e changes.

## Localização atual

| Iniciativa | Localização | Próximo encaminhamento |
| --- | --- | --- |
| 01 — Método SDD editorial | [Concluída](concluida/01-sdd-editorial/01-especificacao-sdd-editorial.md) | Referência do método; resultados e limites nas tasks arquivadas. |
| 02 — Preparação editorial | [Concluída: spec](concluida/02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md), [plano](concluida/02-preparacao-editorial/02-plano-preparacao-editorial.md) e [tasks](concluida/02-preparacao-editorial/02-tasks-preparacao-editorial.md) | Preparação encerrada; parecer suficiente para planejar 03. Voz real e publicação não avaliadas. |
| 03 — Piloto | [Backlog](backlog/03-piloto-editorial/03-piloto-editorial.md) | Preparação 02 recebida; selecionar 03 para elaborar plano/tasks antes de produzir ficha e textos. |
| 04 — Alinhamento editorial e mapa de estudos | [Concluída: spec](concluida/04-alinhamento-editorial/04-spec-alinhamento-editorial.md), [plano](concluida/04-alinhamento-editorial/04-plano-alinhamento-editorial.md) e [tasks](concluida/04-alinhamento-editorial/04-tasks-alinhamento-editorial.md) | Organização e mapa inicial conferidos; estudo técnico e preparação/piloto mantêm seus acompanhamentos próprios. |

Este índice serve à navegação. Decisões e pareceres ficam na spec; execução e evidências ficam nas tasks quando existentes. Consulte esses documentos para o progresso detalhado.

## Responsabilidades fora da metodologia

A metodologia e o acompanhamento ficam aqui. O [mapa de estudos](<../capitulos estudos/MAPA_DE_ESTUDOS.md>) organiza a formação e os capítulos; a [jornada](<../jornada do heroi/README.md>) fornece contexto narrativo; o [registro da autoridade](<../registro da autoridade/PUBLICACOES.md>) concentra posts/artigos e suas origens. As [regras](../AGENTS.md) orientam a atuação das IAs. O [guia](GUIA_DE_OPERACAO.md#contrato-de-localização-e-passagem-ao-acervo) define a passagem entre essas áreas.

## Pastas de apoio

| Pasta / arquivo | O que guarda |
| --- | --- |
| `avaliacoes/` | Evidências dos exercícios de avaliação dos procedimentos: pedidos e critérios, entradas, saídas, pareceres, integração e limites observados. |
| `modelos/` | Estruturas reutilizáveis para specs, planos, tasks, fichas, pareceres e integração. |
| `skills/` | Instruções locais dos procedimentos editoriais. |
| [Guia de operação](GUIA_DE_OPERACAO.md) | Regras de uso, papéis, passagens e encerramento. |

### O que existe em avaliacoes

[T02 — entrada operacional](avaliacoes/T02/01-complemento-registro-operacional.md) é um caso preparado em um recorte depois substituído, sem saída nem conferência. Não conta como exercício executado nem como conclusão de T02-006 da primeira publicação.


Atualmente, [T01-016](avaliacoes/T01-016/README.md) guarda os exercícios sintéticos E01–E07 usados na construção do método. São situações fictícias para observar decisões das skills, como preservar uma ressalva, distinguir pendência de bloqueio ou recusar uma conclusão sem fonte. Inclui a correção dirigida de E03 e seus limites.

Esses arquivos não são relatos do autor, texto do piloto ou comprovação de eficácia geral. A pasta permanece acessível porque as iniciativas seguintes precisam consultar a cobertura já exercitada. Arquivar a spec 01 não elimina suas evidências nem transfere esses exercícios para o backlog.

## Registro de organização — 2026-10-14

Por solicitação do autor, adotadas as pastas de situação. As iniciativas 02 e 03 compõem o trabalho pendente; 02 foi selecionada como próxima análise e ficou em `changes/`, enquanto 03 permaneceu em `backlog/`. A iniciativa 01 permanece em `concluida/`. Nenhuma decisão de voz, história ou execução do piloto foi tomada por essa movimentação.

Versões anteriores de 02 e 03 preservadas no histórico do Git. Links recalculados após a movimentação, inclusive os usados por modelos, skills e documentos concluídos; alterações de navegação não representam nova avaliação de comportamento.

**Conferência:** índice inicial, guia v0.5, spec 02 v0.5 e spec 03 v0.3; 26 documentos ativos examinados, com 154 referências locais válidas e nenhuma âncora sem destino. Confirmada uma única localização vigente para cada iniciativa. `git diff --check` sem erros nos arquivos rastreados. Conferência documental pela mesma IA responsável pela organização; conteúdo editorial do piloto e preferências do autor permanecem pendentes.

## Abertura do change 02 — 2026-10-14

Spec 02 avaliada e atualizada para v0.6, apta para planejar a preparação editorial; plano e tasks v0.1 criados na pasta já existente em `changes/`. Não houve nova movimentação ou duplicação da iniciativa. Parecer e limites estão na spec; acompanhamento e próxima tarefa estão nas tasks. As dez decisões editoriais permanecem abertas. Versões anteriores da spec e deste índice preservadas no histórico do Git.

## Alinhamento do projeto — 2026-10-16

Iniciativa 04 encerrada após correção das interfaces, acervo, mapa inicial e decisões vigentes. Evidências e pendências individuais nas tasks 04. A iniciativa 02 segue em preparação da primeira publicação e 03 permanece em backlog; o encerramento de 04 não executa essas entregas.

## Fechamento da preparação 02 — 2026-10-16

T02-001 a T02-007 conferidas; RA02-16 recebeu extensão livre, EX02-A/B complementaram procedimentos e parecer final delimitou a passagem. Iniciativa 02 arquivada em concluida. Próximo trabalho: planejar 03, sem execução automática do piloto.
