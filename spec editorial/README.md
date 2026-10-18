# Organização do SDD editorial

[Guia de operação](GUIA_DE_OPERACAO.md) · [Regras de entrada](../AGENTS.md) · [Modelos](modelos) · [Skills](skills)

## Fluxo e localização

**Spec → plano → tasks → artefatos.** O SDD organiza a iniciativa; a [sequência editorial do guia](GUIA_DE_OPERACAO.md#4-sequência-editorial-do-texto) conduz a peça dentro dela. Não criar uma nova cadeia documental para cada texto pequeno ou etapa.

| Pasta | Uso e passagem |
| --- | --- |
| `backlog/` | Ideia/refinamento: análise, decisões, lacunas e parecer na mesma spec. Analisar não seleciona nem implementa. |
| `changes/` | Iniciativa selecionada pelo autor para uma fase de trabalho. Mover a mesma pasta com IDs/links; não duplicar. Planejamento não autoriza produção além do pedido. |
| `concluida/` | Escopo encerrado e conferido. Evolução de regra é tratada em iniciativa própria, com vínculo; aceitação anterior invalidada exige motivo, aspecto e reabertura/movimentação. Navegação não reabre conteúdo. |

A pasta não substitui o estado das tasks. Sem tasks, a próxima ação fica na spec. Com tasks, sua tabela é a fonte atual do progresso. “Continue” retoma o escopo autorizado até a entrega ou dependência real, sem nova confirmação por arquivo e sem inventar autorização de outra fase.

## Iniciativas

| ID | Documentos | Finalidade |
| --- | --- | --- |
| 01 — Construção do método | [Spec](concluida/01-sdd-editorial/01-especificacao-sdd-editorial.md) | Construção e avaliação inicial do método; procedimento de uso no guia. |
| 02 — Preparação do piloto | [Spec](concluida/02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md) | Fontes e decisões específicas do piloto; não configuração universal de novas peças. |
| 03 — Piloto | [Spec](concluida/03-piloto-editorial/03-piloto-editorial.md), [plano](concluida/03-piloto-editorial/03-plano-piloto-editorial.md), [tasks](concluida/03-piloto-editorial/03-tasks-piloto-editorial.md) | Aplicação do método a artigo e chamada, apreciação autoral e avaliação do percurso. |
| 04 — Alinhamento e mapa de estudos | [Spec](concluida/04-alinhamento-editorial/04-spec-alinhamento-editorial.md) | Responsabilidades das áreas, navegação e organização do mapa de estudos. |
| 05 — Correção do fluxo | [Spec](<concluida/05-ajuste-fluxo-sdd-editorial/05-spec-ajuste-fluxo-sdd-editorial.md>), [plano](<concluida/05-ajuste-fluxo-sdd-editorial/05-plano-ajuste-fluxo-sdd-editorial.md>), [tasks](<concluida/05-ajuste-fluxo-sdd-editorial/05-tasks-ajuste-fluxo-sdd-editorial.md>) | Ajuste das fases, passagens, preservação e interfaces do método. |

## Consultar por necessidade

- [Guia](GUIA_DE_OPERACAO.md): fases, sequência, contexto e limites comuns. Ler a skill da fase; não carregar as sete de uma vez.
- [Modelos](modelos): campos proporcionais; não são formulários integrais obrigatórios nem entregas preenchidas.
- [Avaliações T01-016](avaliacoes/T01-016/README.md): exercícios sintéticos E01–E07 com limites de cobertura, consultados quando o modo realmente exigir. Não são piloto ou relato autoral.
- [Complementos T02](avaliacoes/T02/02-complementos-voz-e-artigo/03-pareceres-e-integracao.md): cenário sintético de preparação/voz/artigo/chamada; não eficácia geral. A [entrada operacional T02](avaliacoes/T02/01-complemento-registro-operacional.md) documenta o cenário de registro operacional; resultados e cobertura devem ser consultados no acompanhamento correspondente.
- [Jornada](<../jornada do heroi/README.md>), [estudos](<../capitulos estudos/MAPA_DE_ESTUDOS.md>) e [publicações](<../registro da autoridade/PUBLICACOES.md>): conteúdo e fontes em suas áreas, vinculados pelo acompanhamento pertinente.

Decisões e evidências antigas permanecem nas iniciativas de origem e no Git. Este índice não mantém diário de alterações, histórico de aprovações ou uma segunda lista de tarefas.
