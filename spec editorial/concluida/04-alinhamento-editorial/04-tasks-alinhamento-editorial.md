# Tasks 04 — Alinhamento editorial

**ID:** TASKS-EDITORIAL-004  
**Versão:** 0.3 — 2026-10-16  
**Base:** [spec v0.2](04-spec-alinhamento-editorial.md) e [plano v0.2](04-plano-alinhamento-editorial.md).  
**Estado:** concluída no escopo documental.

## Tarefas e critérios

| ID | Entrega / dependência | Resultado e conferência necessária | Estado |
| --- | --- | --- | --- |
| T04-001 | ENT04-01; spec/plano conferidos | Regras e pontos de entrada alinhados às cinco responsabilidades; guia e ficha conectam o acervo ao SDD. | Concluída. |
| T04-002 | ENT04-02; decisão D04-03 | Mapa cobre as sete partes e temas transversais com IDs/dependências válidos, fontes locais, estados e limites; jornada aponta aos responsáveis corretos e não obriga emoções. | Concluída. |
| T04-003 | ENT04-03; decisão D04-02 | Índice das peças existentes, origens e estados; modelos conectados ao método; fontes preservadas e vínculos recíprocos pertinentes. | Concluída. |
| T04-004 | ENT04-04; decisão D04-01 | Decisões atuais em 02/03 reconciliadas sem repetir pendências resolvidas; histórico e critérios ainda pendentes preservados. | Concluída. |
| T04-005 | ENT04-05; T04-001 a T04-004 produzidas | Conferir os sete requisitos, links locais, alterações do recorte, fontes e staging; registrar artefatos, versões, limites e destino de cada pendência. | Concluída. |

## Preservação e registro inicial

Antes da edição dos artefatos, 97 Markdown fora de `historico/` foram copiados para `spec editorial/historico/2026-10-15-antes-do-alinhamento-do-projeto/`, mantendo caminhos relativos à raiz. Todos os hashes SHA-256 coincidiram. Manifesto: [PRESERVACAO.md](../../historico/2026-10-15-antes-do-alinhamento-do-projeto/PRESERVACAO.md).

Hash SHA-256 do índice Git no início: `8cd8b3b81f195eafdd34abe410630799a12eca0464a999d05d4175d0467e7d8d`. O índice contém trabalho anterior; sua composição não integra a edição autorizada desta rodada.

O parecer desta sessão foi aceito pelo autor para aplicação integral. A revisão e integração têm acesso ao histórico e aos pareceres das frentes; não constituem prova de independência. Publicação e estudo técnico não foram iniciados por este registro.

## Evidências da execução

Integração de 2026-10-16 executada sequencialmente pela IA responsável, usando o parecer anterior e o histórico disponível. Todos os sete grupos de achados foram acolhidos. A preservação protege fontes, ressalvas e contexto histórico; não houve redação do piloto nem nova pesquisa técnica.

| Tarefa / requisitos | Artefatos e versões | Critério e evidência | Resultado e limites |
| --- | --- | --- | --- |
| T04-001 / R04-01,02,06 | AGENTS, README, BASE_DO_LIVRO; guia v0.6; ficha v0.2; índice SDD. | Leitura cruzada das cinco responsabilidades e do contrato de destino; os pontos de entrada conduzem ao mapa, acervo e método. | Atende documentalmente. Não reabre a evidência histórica de 01 nem valida comportamento editorial novo. |
| T04-002 / R04-02,03,07 | Mapa de estudos v0.1, README/estrutura de estudos, páginas 06/07/14/15 e índice/universo da jornada. | CAP-01 a CAP-18 cobrem as sete partes e temas transversais; objetivos, fontes de origem, dependências, resultados, estados e pendências presentes. Jornada aponta aos responsáveis e trata emoções como possibilidades. | Atende à organização inicial. Bibliografia específica, diagnóstico, profundidade, aprendizagem e sumário final não foram validados. |
| T04-003 / R04-01,05,06 | PUBLICACOES v0.1; modelo público v0.2; README, método, canais, fichas 02/06/12/14/15; metadados PUB-000 r01. | Cinco peças disponíveis catalogadas: PUB-000 e AMO-01 a 04. Origem dupla, estados separados, referência SDD e vínculos aos registros existentes conferidos. Corpo de PUB-000 e fonte das amostras preservados. | Atende no acervo local disponível. Não comprova importação de toda produção externa nem versões/URLs publicadas das amostras. |
| T04-004 / R04-01,04 | Spec 02 v0.23, plano v0.6, tasks v0.18; spec 03 v0.4. | RA02-14 substitui destino de RA02-13; síntese vigente separa decisões recebidas de propostas históricas. Público, voz, fatos e canais mantidos; T02-004 e T02-005 a 007 conservam pendências reais. | Atende à reconciliação. Guia v0.6 e ficha v0.2 serão considerados na seleção de procedimentos T02-005. Sem passagem automática para 03. |

**Conferência intermediária:** 85 Markdown fora de snapshots/transcrições, 949 referências locais e 310 âncoras sem destinos ausentes. Dezoito fontes protegidas comparadas byte a byte com a preservação, todas intactas. Hash do índice Git inalterado. A conferência de whitespace encontrou duas linhas novas na ficha; corrigidas antes da rodada final. Estes números descrevem a rodada intermediária, antes da atualização do índice e do fechamento.

## Destino das pendências

| Pendência fora da correção documental | Destino explícito / próximo passo |
| --- | --- |
| Diagnóstico, ambiente/caso e fonte para começar estudo | MAPA_DE_ESTUDOS, CAP-01 e seção de pendências; definir antes da atividade. |
| Bibliografia específica, profundidade e ajustes da sequência | MAPA_DE_ESTUDOS por CAP; conferir antes de cada unidade dependente. |
| Conteúdo dos capítulos, evidências e ordem final do livro | Acompanhamento dos CAPs e BASE_DO_LIVRO; permanecem não produzidos. |
| Extensão e prontidão da primeira publicação | T02-004; condições ainda a fechar, sem perguntar novamente canais/destinos. |
| Percurso, cobertura e parecer de suficiência | T02-005/T02-006/T02-007, considerando guia v0.6 e ficha v0.2. |
| Texto e apreciação autoral do piloto | Spec 03; aguarda preparação suficiente de 02. |
| URLs e versões externas das amostras | PUBLICACOES, AMO-01 a AMO-04; conferir quando necessário ao uso, sem presumir envio. |

O fechamento desta iniciativa abrange correções de organização e mapa documental inicial, não execução das pendências acima.

## Histórico

| Versão | Alteração |
| --- | --- |
| 0.1 | Decomposição conferida contra plano v0.1; preservação realizada; execução iniciada. |
| 0.2 | 2026-10-16: T04-001 a 004 produzidas e conferidas; evidências, limites e destinos registrados. T04-005 aguarda conferência final do conjunto. |
| 0.3 | 2026-10-16: T04-005 conferida; encerramento documental e movimentação para concluida, com referências ajustadas. |

## T04-005 — conferência final e encerramento

**Artefatos conferidos:** [mapa v0.1](<../../../capitulos estudos/MAPA_DE_ESTUDOS.md>), [acervo v0.1](<../../../registro da autoridade/PUBLICACOES.md>), [guia v0.6](../../GUIA_DE_OPERACAO.md), [ficha v0.2](../../modelos/ficha-editorial.md), [spec 02 v0.23 e acompanhamento](../02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md), [spec 03 v0.4](../../backlog/03-piloto-editorial/03-piloto-editorial.md), regras, índices, modelos e páginas identificados nas entregas acima.

**Resultado:** R04-01 a R04-07 atendidos no escopo documental. Os 18 CAPs têm IDs únicos, dependências existentes e sem ciclos; todos permanecem pendentes quanto à aprendizagem. Cinco peças disponíveis inventariadas com seus limites; nenhuma publicação externa atribuída sem evidência. Corpo do rascunho PUB-000 preservado. Os 11 links antigos para Livro foram corrigidos nos documentos de orientação, mantendo referências históricas em seus contextos.

**Evidência de navegação antes do arquivamento:** 85 Markdown fora de snapshots/transcrições; 958 referências locais e 311 âncoras verificadas, nenhum destino ausente. A revisão de apresentação detectou uma linha de histórico separada da tabela nas tasks 04; integrada antes do fechamento. `git diff --check` passou após corrigir as duas linhas de whitespace da ficha. Dezoito fontes protegidas permaneceram byte a byte iguais à preservação; índice Git com SHA-256 inicial inalterado. Após a movimentação, reconferidos 85 documentos, 964 referências locais e 311 âncoras: nenhum destino ausente. Localização única de 04 em concluida confirmada; fontes protegidas e índice Git novamente intactos.

**Limites:** leitura documental silenciosa pela mesma IA integradora, com acesso aos pareceres anteriores. Não houve pesquisa técnica externa, execução do estudo, prova de eficácia nova das skills, redação do piloto ou apreciação humana presumida. A sequência dos capítulos é proposta operacional revisável. Não se alterou o staging nem se realizou commit.

**Retomada:** correções desta iniciativa concluídas; consultar T02-004 para a primeira publicação ou as pendências de CAP-01 quando houver seleção de estudo. Não reabrir escolhas já recebidas de leitor, voz, canais ou destino. Preservar o encaminhamento individual das demais pendências na tabela acima.
