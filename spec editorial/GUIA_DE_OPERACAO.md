# Guia de operação do SDD editorial

**Versão:** 1.1 — 17/10/2026. **Base vigente:** [spec 05](<concluida/05-ajuste-fluxo-sdd-editorial/05-spec-ajuste-fluxo-sdd-editorial.md>), D05-01/02 e R05-01–12. Evidências em [tasks 05](<concluida/05-ajuste-fluxo-sdd-editorial/05-tasks-ajuste-fluxo-sdd-editorial.md>). A construção inicial permanece na [spec 01](concluida/01-sdd-editorial/01-especificacao-sdd-editorial.md); pareceres antigos não validam automaticamente esta versão.

## 1. Começar pelo escopo autorizado

Localizar o pedido atual e a iniciativa no [índice](README.md). Se houver tasks, ler sua tabela atual; sem tasks, consultar parecer e próxima ação na spec. Ler explicitamente a skill da fase. Consultar somente a peça/ficha e fontes necessárias; não carregar todas as iniciativas, quinze etapas, modelos ou avaliações.

A entrada mínima é: objetivo/limite autorizado, fase e tarefa quando houver, artefato/revisão, decisões pertinentes, fontes selecionadas, lacuna e próxima ação. Um documento operacional pode usar o contrato da tarefa sem ficha narrativa.

“Continue” retoma essa entrega autorizada até concluí-la ou encontrar dependência real. Não exige nova confirmação por tarefa/arquivo e não autoriza automaticamente outra fase. Decisão ou fato essencial, versão a preservar ou retorno do autor interrompe somente a parte dependente. Continuar as partes independentes e perguntar pelo ponto concreto, sem repetir decisões já recebidas.

## 2. Organização SDD da iniciativa

**Pedido/escopo → análise de contexto/fontes → esclarecimentos essenciais → spec revisada → plano conferido → tasks conferidas → consistência entre os três → execução/conferência → encerramento.**

| Situação | Local e passagem |
| --- | --- |
| Ideia ou refinamento | `backlog/`: análise, decisões, lacunas e parecer na mesma spec. Analisar não seleciona nem implementa. |
| Trabalho selecionado | Mover a mesma pasta para `changes/`, atualizando links e mantendo IDs. A seleção autoriza somente a fase pedida. Plano e tasks são separados quando necessários à iniciativa; não criá-los vazios. |
| Execução | Seguir entregas/dependências autorizadas. Antes de executar, verificar requisito sem entrega, entrega sem tarefa, conflito de escopo ou dependência sem destino. Não criar outro relatório para essa conferência. |
| Encerramento | Critérios atendidos, evidências suficientes e pendências individualizadas. Mover para `concluida/` após conferência; ausência de retorno humano mantém pendente a entrega que dele depende. |

Uma peça pequena dentro de iniciativa definida usa seu acompanhamento, sem nova spec/plano/tasks por rotina. Correção pontual pode usar contrato breve e conferência dirigida. A avaliação de todos os modos das skills é trabalho específico do método, não obrigação de cada texto.

## 3. Autoridade e localização dos documentos

| Documento/área | Responsabilidade |
| --- | --- |
| AGENTS | Invariantes do projeto e roteamento da leitura. |
| README do SDD | Localização e encaminhamento, por vínculo ao acompanhamento. |
| Este guia | Procedimento editorial vigente e passagens comuns. |
| Spec / plano / tasks | Intenção/requisitos e decisões / entregas e estratégia / estado, evidência e próxima ação. |
| Skills / modelos | Procedimento do papel / campos proporcionais, sem preenchimento mecânico. |
| `jornada do heroi/` | Contexto, relatos pessoais e acompanhamento nas próprias páginas. |
| `capitulos estudos/` | Ordem de estudo, fontes, explicações e capítulos que formarão o livro. |
| `registro da autoridade/publicacoes/` | Peças para leitores, suas fichas e revisões, inclusive rascunhos. |

Instruções explícitas do autor prevalecem sobre orientações locais, respeitadas as regras do ambiente. Uma proposta não ganha autoridade por ser mais recente. Em conflito relevante, conferir a última decisão efetivamente aceita e perguntar só se faltar definição essencial; não escolher por quantidade de documentos.

Registros encerrados conservam o contexto da época, não determinam um próximo passo atual. Evolução do método atualiza a orientação vigente com vínculo à decisão; se um defeito invalidar aceitação anterior, registrar evidência/aspecto e reabrir a iniciativa conforme o índice. Correção de navegação não reabre conteúdo. Não copiar o mesmo histórico para várias iniciativas.

### Contrato de localização e passagem ao acervo

Posts/artigos têm um único arquivo de trabalho em `publicacoes/`, catalogado no [índice](<../registro da autoridade/PUBLICACOES.md>). Cada peça tem ID PUB disponível, revisão, origem (`jornada`, `estudo` ou `ambas`), ficha/tarefa quando pertinentes e relação com fontes. Artigo e chamada recebem IDs distintos. Os capítulos têm seus próprios IDs CAP e permanecem na área de estudo.

Vincular uma experiência ou fonte sem duplicá-la como outro acontecimento. Não recriar pastas de sessões, episódios ou fichas de etapas paralelas no acervo. Identificadores históricos, como EP-000, permanecem recuperáveis e vinculados à jornada. Estado atual detalhado fica nas tasks; índice registra apenas revisão/estado editorial, retorno e publicação da peça, com vínculo ao acompanhamento.

## 4. Sequência editorial do texto

**Preparar → estruturar quando necessário → redigir → revisar → integrar → reconferir → leitura autoral → ajustes, se houver → prova final.**

| Etapa | Responsabilidade e saída | Papel/skill e passagem |
| --- | --- | --- |
| Preparar | Avaliar próximo conteúdo pelo pedido, material e pendências, situando jornada ou estudo. Definir leitor, contribuição, natureza, tom, formato, fontes e limites em ficha proporcional. | `editorial-preparar`: base suficiente ou rascunho com lacunas delimitadas. Não substituir conteúdo já escolhido pelo autor nem seguir automaticamente a numeração da jornada. |
| Estruturar, quando necessário | Organizar abertura, progressão e fechamento conforme a ficha; produzir esboço. | `editorial-redigir`, esboço. Peça breve/estável pode dispensar arquivo de esboço; manter sequência compreensível. |
| Redigir | Produzir rascunho identificado a partir da ficha/fontes. | `editorial-redigir`: leitura de entrega, sem alegar revisão especializada. |
| Revisar | Examinar foco/estrutura/fatos/sentido antes do acabamento; didática/continuidade/voz conforme a peça, depois fluidez/língua. | `editorial-revisar`: achados e preservações, sem editar silenciosamente. Mudança estrutural é integrada antes de leituras dependentes. |
| Integrar | Acolher, recusar com motivo ou manter pendente os achados relevantes; aplicar alterações autorizadas. | `editorial-integrar`: versão resultante e decisões, preservando fatos, ressalvas e voz. Sem alteração, manter a revisão existente. |
| Reconferir | Examinar resolução dos achados e efeitos das mudanças na versão resultante. | `editorial-revisar`, aspectos afetados. Voltar à integração se necessário; depois entregar para leitura autoral. |
| Leitura autoral | Autor avalia voz, sentido, clareza, exposição e experiência de leitura; IA registra retorno real. | Autor. Sem retorno: pronto para leitura autoral, sem aprovação presumida. |
| Ajustes, se houver | Aplicar decisões do autor e reconferir aspectos afetados. | Integrar/revisar. Mudança de intenção ou exposição além do retorno recebido exige esclarecimento. Sem ajustes, seguir à prova. |
| Prova final | Conferir língua, títulos, links, resíduos e integridade da versão posterior ao retorno/ajustes. | Revisar P09. Problema substancial volta à etapa responsável; alteração invalida a prova no aspecto afetado. |

Sem alterações necessárias, registrar a decisão de manter o texto no acompanhamento existente e conservar sua revisão. Não criar r02, edição ou commit apenas para representar uma passagem. Sem mudanças nem achados a reconferir, registrar que a reconferência foi dispensada por esse motivo e seguir à leitura autoral, se não houver pendências impeditivas. Decisões de recusar achados relevantes precisam de fundamento; não dispensar sua conferência quando ainda houver questão a resolver.

Etapas são funções, não um arquivo ou agente obrigatório por etapa. Podem ocorrer na mesma sessão. Reaproveitar etapas já atendidas com evidência; mudança de regra reabre somente o aspecto afetado. Uma leitura técnica anterior ao autor pode remover resíduos, mas não substitui a prova final posterior.

## 5. Profundidade e coordenação

O mínimo é fidelidade à intenção e fontes/ressalvas relevantes, coerência e legibilidade. Ficha breve atende escopo estável; ficha completa/esboço se justificam por múltiplas fontes, estrutura ou decisões complexas. Capítulo exige pré-requisitos e suficiência didática; relato respeita vivências/voz; chamada é fiel ao artigo. Escolher perfis por questão presente, sem exigir os nove ou justificar nove dispensas. Os [perfis P01–P09](skills/editorial-revisar/references/perfis.md) são referência seletiva.

Plano coordena entregas e dependências; tasks mantêm etapa, versão e próxima ação atuais; skills executam seus papéis. Cada passagem recebe objetivo/limite, ficha e versão quando existentes, fontes selecionadas, achados/lacunas e saída esperada. Entrega artefato/revisão, resultado, critério conferido e pendência. Não repetir a ficha inteira nas tasks nem criar logs de passagem.

Uma mesma IA pode assumir os papéis sequencialmente, declarando acesso ao histórico/pareceres sem alegar independência. Revisão entrega parecer; integração altera; apreciação é humana. Não delegar automaticamente nem usar consenso entre IAs como comprovação factual.

## 6. Preservação, voz e retorno de achados

D05-01: sempre que precisar preservar texto de publicação, jornada ou capítulo de estudo antes de alterar, verificar se a versão está recuperável no Git. Se não estiver, solicitar o commit do autor e aguardar a edição dependente; continuar partes independentes. Não fazer commit/push automaticamente, cópia paralela, backup, snapshot ou manifesto para simular versionamento. Revisão r01/r02 não garante recuperação por si só.

A jornada é pessoal, em primeira pessoa e português brasileiro, com humor e repertório conforme a escolha do autor. Família, furão e outros interesses podem entrar quando pertinentes e relatados, sem cenas, emoções ou falas inventadas. Capítulos devem ensinar independentemente da autobiografia. Precisão técnica não exige voz corporativa. Preferências da preparação 02 são entradas do piloto 03; outra peça usa as decisões de sua própria iniciativa/ficha e a direção geral vigente.

Achado relevante identifica trecho/versão, problema, fundamento, importância e encaminhamento; ganho e possível perda quando se propõe mudança expressiva. Pode recomendar manter o que funciona. Impeditivo impede concluir a entrega afetada; revisão necessária exige correção ou justificativa; sugestão pode ser recusada. Não há número mínimo de mudanças.

Mudança de intenção/requisito volta à spec; estratégia ao plano; execução/evidência às tasks. Lacuna factual volta à fonte/preparação; estrutura ao esboço/redação; achado persistente à integração; vivência ou posicionamento não definidos voltam ao autor. Reconferir somente o afetado, mantendo sentido, fontes e ressalvas.

## 7. Conferência e encerramento

Tasks registram ID, estado, resultado/versão, critério/evidência suficiente e pendência/próxima ação. Estados: pendente; em execução; produzida/aguardando conferência; concluída; bloqueada com motivo após tentativa impedida. Dependência futura não é bloqueio. A tabela atual é única; explicação extensa só quando necessária, sem diário de saves ou lista repetida de arquivos alterados. Quando houver iniciativa com tasks, elas são a fonte do progresso; ficha e peça vinculam esse acompanhamento, sem uma segunda lista de estado ou pendências. Trabalho pequeno que dispense iniciativa/tasks usa um único registro proporcional na própria peça ou ficha, sem criar documento só para isso.

Distinguir documento produzido, estrutura/links conferidos, procedimento exercitado, apreciação autoral e publicação. Validador de skill não demonstra qualidade de escrita, prazer de leitura ou voz reconhecida. Não inventar tempos, retorno humano, consulta a fonte ou leitura em voz alta. Cobertura não exercitada recebe destino; impeditivo não é transferido para aparentar conclusão.

Uma peça aguarda leitura autoral até receber retorno; ajustes são reconferidos e a prova final examina a versão resultante. Publicar é ação separada, com instrução explícita e registro de revisão exata, destino, data e URL. Preparar ou concluir revisão não envia conteúdo.
