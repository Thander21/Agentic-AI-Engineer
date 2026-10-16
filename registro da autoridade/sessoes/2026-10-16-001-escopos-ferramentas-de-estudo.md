# SS-2026-10-16-001 — Escopos das ferramentas de estudo

[Método de registro](../METODO_DE_REGISTRO.md) · [Mapa das ferramentas](<../../ferramentas de estudo/README.md>)

- Data: 2026-10-16.
- Revisão: r01.
- Pergunta inicial: como incluir os três projetos nas regras de leitura da IA e no contexto para preparar posts ou histórias?
- Estado: organização concluída e conferida documentalmente.
- Registro preparado pela IA a partir do pedido do autor nesta sessão; não é texto público nem relato de aprendizagem técnica.

## Decisões recebidas

| Fonte autoral | Decisão registrada | Limite |
| --- | --- | --- |
| Pedido de 16/10/2026 — FlutterGuard-AI | Somente uma ideia a desenvolver para estudo. | Documentação não comprova implementação. |
| Mesmo pedido — SDD-TDDkit e SpecSimpleKit | Kit em desenvolvimento e uso; o autor começa com SpecSimpleKit, testa e adapta em cada projeto e usa a experiência para evoluir o SDD-TDDkit. Este projeto editorial também foi personalizado a partir da base. | Não presumir que cada adaptação local voltou ao kit nem que houve instalação técnica do motor aqui. |
| Mesmo pedido — VagasAutomatizada | Fonte privada de informações pessoais/profissionais e projeto em uso na busca de vagas; consultar localmente, documentar apenas existência/finalidade e excluir do Git deste acervo. | Nome local: VagasAutomatizado. Conteúdo privado não deve ser copiado para o repositório editorial. |
| Mesmo pedido — Obsidian | Usar notas pertinentes como fontes e melhorar os vínculos entre dados depois. | Expansão dos vínculos permanece futura. |

Essas decisões complementam as fontes de consulta; não alteram intenção, voz ou prontidão do piloto 03. As iniciativas 01, 02 e 04 permanecem encerradas no escopo já conferido. A inclusão pontual foi registrada nesta sessão, sem criar uma nova cadeia spec/plano/tasks.

## Integração realizada

- Criado o mapa v0.1 com estados, pontos de entrada, limites de evidência e consulta privada.
- Incluídas regras no AGENTS e vínculos nos READMEs da raiz, dos estudos, da jornada e do acervo.
- Substituída a regra ineficaz `./VagasAutomatizado/` por `**/VagasAutomatizado/` no `.gitignore` principal, cobrindo o nome real em qualquer nível e preservando as demais exclusões. A regra adicional para a variante VagasAutomatizada foi retirada em edição concomitante; mantida a versão atual do arquivo, sem recriar uma pasta com essa grafia.
- Mantidos os documentos internos dos projetos e as configurações do Obsidian; nenhuma fonte privada foi transcrita ou copiada.

Aplicadas as skills locais `editorial-preparar` v0.2, para seleção de contexto, e `editorial-integrar` v0.1, para preservação e integração proporcional. A conferência auxiliar foi documental e somente leitura, com acesso ao histórico; não constitui revisão cega ou prova de funcionamento dos projetos.

## Preservação e fontes

As seis versões anteriores estão na [preservação desta rodada](<../../spec editorial/historico/2026-10-16-antes-dos-escopos-de-ferramentas/PRESERVACAO.md>), com SHA-256 conferido antes da edição e reconferido ao final. O índice permaneceu igual na conferência intermediária e recebeu uma atualização concomitante depois: os arquivos desta rodada passaram a constar no staging. Essa atualização foi preservada; o registro final desta conferência foi ajustado em seguida no arquivo de trabalho.

O [README do FlutterGuard-AI](<../../ferramentas de estudo/FlutterGuard-AI/README.md>) descreve capacidades no presente; o relato atual do autor prevalece como estado editorial. Os [pontos de entrada do SDD-TDDkit e SpecSimpleKit](<../../ferramentas de estudo/README.md#sdd-tddkit-e-specsimplekit-base-prática-e-evolução>) sustentam a distinção documental entre oficina e base. Não houve avaliação técnica dessas capacidades.

Para VagasAutomatizado, conferidos apenas existência/caminho, situação no índice principal e presença de `.git` próprio. Não foi encontrado `.git` nessa cópia local. Repositório privado no GitHub e sua visibilidade não foram verificados; nenhum remoto foi criado ou sincronizado.

## Conferência

| Critério / artefato | Evidência | Resultado |
| --- | --- | --- |
| Coerência do mapa v0.1, desta sessão r01 e dos cinco pontos de entrada ajustados | Leitura dirigida comparada com as seis versões preservadas; parecer auxiliar de fatos/fontes e continuidade usando `editorial-revisar` v0.2, com histórico disponível. | PASS documental: estados autorais preservados, destinos editoriais coerentes e vínculos ampliados do Obsidian mantidos como etapa futura. |
| Navegação dos sete Markdown vigentes alterados/criados e do manifesto | 230 referências locais e 8 âncoras conferidas em 8 documentos, sem destinos ausentes. | PASS. Caminho privado apresentado como texto; não foi criado link que dependa dele numa cópia pública. |
| Exclusão no `.gitignore` principal | `git check-ignore -v` confirmou o caminho real, arquivo oculto, eventual `.git/config` e cópia em subpasta histórica. | PASS para VagasAutomatizado; 0 arquivos privados rastreados e 0 elegíveis como não rastreados nessa pasta. Os três pontos de entrada públicos das ferramentas continuam disponíveis ao Git. A variante VagasAutomatizada não está coberta na versão final e não corresponde a uma pasta existente. |
| Preservação e staging | Seis cópias com SHA-256 iguais aos hashes do manifesto. Índice inicial/intermediário: `f5b5f98d8126b1574d98c7f2a5e7832dc9d2d9a6c7d0e963ed70996be38edb12`; última leitura após atualização concomitante: `9ae5737a649d7054ce3aa2b5438a6999b2e2eef063661866f921a0c81b987f8b`. | PASS das cópias; o índice final não é idêntico ao inicial. O agente não executou `git add`, reset, commit ou envio, nem reverteu a atualização concomitante. |
| Apresentação e índice do acervo | Deltas comparados às cópias; conferência de whitespace dos Markdown sem erros; 29 Markdown contados no acervo. | PASS no recorte documental. O `.gitignore` foi conferido pelo comportamento das regras, preservando sua edição concomitante. Não é validação de software, aprendizagem, comportamento das skills no piloto ou apreciação autoral. |

A existência e a privacidade de um remoto GitHub permanecem não verificadas. Essa limitação não altera a conferência da exclusão no Git principal.

## Limites e próximo passo

Não houve estudo técnico, desenvolvimento dos projetos, geração de post/história, execução de automações, publicação ou commit. Consulta privada autorizada não equivale a liberação de dados para o acervo público.

A inclusão dos escopos permite selecionar fontes para um pedido editorial futuro. A ampliação dos vínculos do Obsidian aguarda a seleção das notas e relações pelo autor. O piloto continua no acompanhamento próprio da iniciativa 03.
