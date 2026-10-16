# Orientações para IAs e IDEs

Este arquivo é o ponto de entrada para trabalhar neste repositório. Aplica-se à raiz e às subpastas. Se o ambiente não carregar `AGENTS.md` automaticamente, leia-o explicitamente antes de atuar. Não presuma instalação ou descoberta automática das skills locais.

## Natureza do projeto

O projeto documenta a jornada pessoal do autor e sua formação por autoestudo em engenharia com agentes. O conhecimento tem uso profissional pelo autor e por quem quiser aproveitá-lo; os próprios capítulos de estudo serão estruturados como livro. O trabalho principal é editorial: estudo, registros, fontes, escrita criativa e revisão. Não introduza código, aplicação, infraestrutura ou baterias de testes de software para organizar a escrita.

Comunique-se em português. A jornada é pessoal, narrada em primeira pessoa, com humor, retórica, cotidiano e referências escolhidas pelo autor. Família, seu pet (um furão), filmes, animes, livros e outros interesses podem participar conforme os relatos forem trazidos. Esses temas já estão autorizados como direção; nomes, cenas, diálogos, emoções e acontecimentos específicos precisam de fonte autoral. Nenhum tema precisa aparecer em todo texto.

Os capítulos de estudo são o percurso técnico autônomo e formarão o livro. Devem apresentar conceitos, pré-requisitos e fontes suficientes para quem não acompanha a história pessoal. Relatos podem ser vinculados como leitura complementar; compreender a jornada não é pré-requisito para aprender o conteúdo. Posts e artigos recebem voz conforme a finalidade: história pessoal, explicação técnica ou combinação explícita das duas.

A forma de trabalhar respeita a rotina, as escolhas e o ritmo pessoal do autor. O SDD apoia essa organização com clareza e rastreabilidade; documentos operacionais podem ser diretos e próximos, sem impor linguagem corporativa, fantasia ou humor a todos os registros. Não fabrique sofrimento, derrota ou superação para completar um arco narrativo.

## Como começar ou retomar uma sessão

A organização das iniciativas segue [backlog → changes → concluida](<spec editorial/README.md>). Consulte primeiro `spec editorial/changes/` para localizar o trabalho selecionado; `backlog/` reúne o que aguarda e `concluida/` preserva o que foi encerrado. Mover uma iniciativa exige atualizar links e manter seus IDs; não duplicar a spec nas pastas. A localização não autoriza avançar além da fase pedida.

1. Identifique o pedido atual e seu escopo. Um pedido de análise não autoriza executar todas as fases seguintes. Instruções explícitas do autor prevalecem sobre orientações locais, respeitadas as regras do ambiente.
2. Leia o [guia de operação](<spec editorial/GUIA_DE_OPERACAO.md>) e o acompanhamento da iniciativa pertinente, incluindo pendências e o último registro relevante. As [tasks 01](<spec editorial/concluida/01-sdd-editorial/01-tasks-sdd-editorial.md>) conservam as evidências do método; a [spec 02](<spec editorial/concluida/02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md>) conserva a preparação editorial concluída e a [spec 03](<spec editorial/backlog/03-piloto-editorial/03-piloto-editorial.md>) delimita o piloto. Enquanto uma iniciativa não tiver plano/tasks, consulte o parecer e a próxima ação na própria spec. Um “continue” deve partir dessas evidências.
3. Consulte as seções pertinentes da spec e do plano da iniciativa, se existente. A [spec 01](<spec editorial/concluida/01-sdd-editorial/01-especificacao-sdd-editorial.md>) e o [plano 01](<spec editorial/concluida/01-sdd-editorial/01-plano-sdd-editorial.md>) são a referência do método. Confirme versões, dependências e arquivos existentes antes de editar.
4. Leia o `SKILL.md` correspondente à fase na tabela abaixo. Consulte seus modelos e referências conforme a necessidade; não carregue todo o acervo indiscriminadamente.
5. Execute o trabalho autorizado que tenha contexto suficiente. Registre lacunas concretas e prossiga nas partes independentes. Não peça novamente decisões já fornecidas pelo autor.

As tasks são a fonte do progresso atual. Este arquivo não mantém uma segunda lista de tarefas concluídas. Registros antigos descrevem o estado na data em que foram escritos; não devem substituir o acompanhamento atual.

## Fontes de orientação e organização

| Documento ou pasta | Função |
| --- | --- |
| [Spec 01](<spec editorial/concluida/01-sdd-editorial/01-especificacao-sdd-editorial.md>) | Intenção, requisitos e regras do SDD editorial. |
| [Plano 01](<spec editorial/concluida/01-sdd-editorial/01-plano-sdd-editorial.md>) | Entregas, dependências, contratos das skills e critérios de avaliação. |
| [Tasks 01](<spec editorial/concluida/01-sdd-editorial/01-tasks-sdd-editorial.md>) | Execução, evidências, versões, pendências e reaberturas. |
| [Guia de operação](<spec editorial/GUIA_DE_OPERACAO.md>) | Aplicação do fluxo, papéis, percursos e encerramento. |
| [Spec 02 — preparação editorial](<spec editorial/concluida/02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md>) | Análise de história, contexto, referências de voz/tom, adequação das skills e definições de onde, como e quando antes do piloto. |
| [Spec 03 — piloto](<spec editorial/backlog/03-piloto-editorial/03-piloto-editorial.md>) | Aplicação do método, ficha final, redação, revisão, integração e avaliação autoral; recebe a preparação suficiente de 02. |
| [Jornada do herói](<jornada do heroi/README.md>) | Contexto narrativo para escrever: quinze etapas, universo, voz e fontes preservadas; não define o currículo nem o método SDD. |
| [Estrutura técnica e estudo](<capitulos estudos/README.md>) | Mapa da formação e ordem de estudo em capítulos, com objetivos, pré-requisitos, fontes e evidências. A ordem de ensino no livro pode diferir da ordem de estudo. |
| [Registro da autoridade](<registro da autoridade/README.md>) | Acervo central de todos os posts e artigos criados, da jornada, dos estudos ou de ambos; inclui registros de origem, versões e destinos de publicação. |
| [Base do livro](<capitulos estudos/BASE_DO_LIVRO.md>) | Relação entre experiências, maturidade dos registros e capítulos. |
| [Ferramentas de estudo](<ferramentas de estudo/README.md>) | Três projetos como fontes de contexto e conhecimento: ideia de estudo, método em desenvolvimento e consulta privada. O mapa distingue estados, evidências e limites de uso. |

Se houver divergência entre documentos, identifique-a e confira as decisões mais recentes. Não transforme proposta histórica em escolha aceita, nem sobrescreva silenciosamente regras para resolver o conflito. Use os caminhos reais do workspace; não recrie pastas antigas a partir de referências desatualizadas.

Posts e artigos têm sua versão de trabalho em `registro da autoridade/publicacoes/` e entrada no [índice de publicações](<registro da autoridade/PUBLICACOES.md>). Capítulos e seu mapa ficam em `capitulos estudos/`; contextos narrativos e fontes históricas permanecem na jornada. Vincule o conteúdo de origem em vez de criar duas versões vigentes do mesmo texto. Fontes antigas preservadas fora do acervo podem ser inventariadas por referência. O [guia de operação](<spec editorial/GUIA_DE_OPERACAO.md#contrato-de-localização-e-passagem-ao-acervo>) detalha a passagem entre as áreas.

**Obsidian:** a pasta [.obsidian/](.obsidian/), na raiz, guarda configurações de navegação e apresentação do projeto. Consulte apenas os arquivos pertinentes quando a tarefa envolver links, propriedades ou comportamento do Obsidian. Para leitura editorial, priorize os arquivos Markdown, índices e acompanhamento SDD. Estado de janelas, arquivos recentes e configurações de plugins não representam decisões editoriais nem progresso das iniciativas.

### Consulta do registro da autoridade

O [mapa de uso do acervo](<registro da autoridade/README.md#mapa-de-uso-dos-documentos>) distingue orientação, modelos, registros históricos, fichas e rascunhos. Consulte por finalidade:

- **Registrar experiência:** [método de registro](<registro da autoridade/METODO_DE_REGISTRO.md>) e somente o [modelo](<registro da autoridade/modelos>) pertinente. Fichas de etapas vinculam experiências; não definem a próxima tarefa editorial nem a ordem de estudo.
- **Preparar ou revisar post/artigo:** [índice de publicações](<registro da autoridade/PUBLICACOES.md>), versão da peça, decisões da spec e skill da fase. O [modelo de texto público](<registro da autoridade/modelos/texto-publico.md>) complementa a ficha editorial e o percurso SDD.
- **Examinar canais:** [canais e autoridade](<registro da autoridade/CANAIS_E_AUTORIDADE.md>), distinguindo síntese vigente de pesquisa histórica e conferindo a spec da iniciativa.
- **Recuperar a origem de uma ideia:** [origem das ideias](<registro da autoridade/ORIGEM_DAS_IDEIAS.md>) e a fonte específica. Essa leitura é contextual, não obrigatória para todo trabalho.

Esses documentos permanecem no acervo; as skills os utilizam como contexto e modelos conforme a tarefa. Não copiar relatos ou pesquisa histórica para dentro de uma skill. Documento usado na construção continua preservado como fonte; modelo disponível, registro produzido, texto revisado e publicação são estados diferentes.

### Consulta da jornada do herói

O [mapa de uso dos documentos de apoio](<jornada do heroi/README.md#mapa-de-uso-dos-documentos-de-apoio>) distingue contexto narrativo de fonte histórica. Consulte por finalidade:

- **Preparar, redigir ou revisar uma história:** [universo narrativo](<jornada do heroi/UNIVERSO_NARRATIVO.md>), decisões da spec e relatos pertinentes. Primeira pessoa, humor e repertório pessoal orientam a escrita; exemplos fictícios e arcos propostos não comprovam vivências.
- **Localizar a origem de uma afirmação:** [mapa de origem](<jornada do heroi/MAPA_ORIGEM.md>) e apenas os trechos necessários dos anexos. Não carregar os quinze anexos indiscriminadamente nem tratar seus títulos históricos como decisões atuais.
- **Investigar uma referência mencionada:** [inventário de referências](<jornada do heroi/REFERENCIAS.md>), distinguindo menção histórica de fonte consultada e validada. O uso técnico efetivo pertence ao capítulo de estudo; repertório cultural e pessoal pertence ao contexto narrativo.

Esses documentos permanecem na jornada. Skills orientam procedimentos e consultam esse contexto por vínculo; specs registram escolhas e mudanças, sem incorporar todo o acervo. Páginas de 01 a 15 são contextos propostos, anexos são fontes e textos resultantes vão para o registro da autoridade. A retomada editorial é determinada pelas tasks da iniciativa, não pela numeração da jornada.

### Consulta dos capítulos e estudos

O [mapa de uso da área técnica](<capitulos estudos/README.md#mapa-de-uso-dos-documentos>) distingue planejamento, orientação editorial e fontes históricas. Consulte por finalidade:

- **Localizar ou acompanhar uma unidade:** [mapa de estudos](<capitulos estudos/MAPA_DE_ESTUDOS.md>), preservando IDs CAP, fontes, evidências e vínculos ao arquivo do capítulo. Sequência proposta não comprova estudo concluído.
- **Preparar ou revisar um capítulo:** [base do livro](<capitulos estudos/BASE_DO_LIVRO.md>), fontes selecionadas e skill da fase. Os próprios capítulos formarão o livro e devem permitir leitura técnica independente da história pessoal.
- **Recuperar a organização dos assuntos:** [estrutura e estudo](<capitulos estudos/ESTRUTURA_E_ESTUDO.md>), como consolidação histórica das sete partes; a sequência atual fica no mapa.
- **Conferir a formulação de origem:** [extração da última revisão](<capitulos estudos/EXTRACAO_ULTIMA_REVISAO.md>) e os trechos pertinentes dos anexos, com auxílio do mapa de origem da jornada quando necessário. Preservar transcrições; não converter afirmações da conversa em fatos técnicos validados.

Os cinco documentos permanecem nesta área. Conteúdo de estudo e suas fontes não pertencem às skills; estas descrevem o procedimento editorial. Vincule posts/artigos derivados ao acervo central. Consulte as tasks pertinentes para o escopo autorizado, sem iniciar estudo por mera disponibilidade do mapa nem duplicar a fonte histórica como capítulo vigente.

### Consulta das ferramentas de estudo

O [mapa das ferramentas](<ferramentas de estudo/README.md>) reúne três escopos de leitura para preparar estudos, posts, artigos ou histórias. Consulte o projeto pertinente ao assunto, além dos registros e notas Markdown selecionadas do Obsidian; não carregue os três projetos inteiros por padrão.

- **FlutterGuard-AI — ideia para estudo:** está somente como ideia a desenvolver, conforme relato do autor de 16/10/2026. Seus documentos descrevem propostas; não comprovam ferramenta implementada, testes executados ou resultados.
- **SDD-TDDkit — desenvolvimento e uso:** o autor inicia cada projeto com o SpecSimpleKit, testa e personaliza a base conforme a necessidade e usa essa experiência para evoluir o SDD-TDDkit. Este projeto editorial também recebeu uma adaptação dessa base. Distinguir base, adaptação local e evolução incorporada ao kit; uma mudança aqui não comprova integração no kit.
- **VagasAutomatizado — consulta privada:** chamado de VagasAutomatizada no pedido, está em `ferramentas de estudo/VagasAutomatizado/`. Reúne contexto pessoal/profissional e o projeto em uso na busca de vagas, segundo o autor. A consulta local está autorizada quando pertinente; arquivos ignorados pelo Git continuam disponíveis para essa leitura dirigida. Não copiar seu conteúdo, dados pessoais, currículos, contatos, candidaturas, capturas, anexos ou resumos privados para arquivos versionáveis deste repositório, inclusive fichas, logs e históricos. Aqui se documenta apenas sua existência, finalidade e regra de consulta. Um recorte público depende de autorização específica do autor e de conferência do que será exposto.

Antes de usar um projeto como fonte, leia seu ponto de entrada e as instruções locais pertinentes. Consultar documentação não autoriza executar scripts, desenvolver a ferramenta, enviar candidaturas ou importar suas regras operacionais para o SDD editorial. Relato autoral, proposta documentada e resultado técnico conferido são evidências diferentes. Registre caminho, data/versão e limite de cada fonte publicável; referências detalhadas à fonte privada ficam no próprio ambiente privado.

O VagasAutomatizado deve permanecer excluído pelo `.gitignore` deste repositório, com versionamento privado separado. Não adicionar à força, criar submódulo nem copiar a pasta para contornar essa separação. Se houver arquivos já rastreados, o `.gitignore` sozinho não os retira do índice: conferir o estado antes de afirmar proteção. A existência e a visibilidade de um repositório remoto exigem verificação própria.

Os vínculos entre projetos, dados e notas no Obsidian serão ampliados depois, conforme seleção do autor. Por enquanto, o mapa orienta a leitura; configurações de `.obsidian/` não substituem fontes nem autorizam expor dados privados. Posts/artigos continuam no acervo central e capítulos na área de estudos, preservando as origens `jornada`, `estudo` ou `ambas`.

## Fluxo SDD editorial

O fluxo usa três documentos de trabalho por iniciativa e os artefatos resultantes:

1. **Spec:** reúne análise inicial, especificação, decisões, lacunas e revisão de consistência no mesmo documento.
2. **Plano:** documento separado, elaborado com base na spec suficientemente definida; organiza entregas, dependências e critérios.
3. **Tasks:** documento separado, atualizado durante produção e conferência, com IDs estáveis e evidências.
4. **Artefatos:** textos ou documentos produzidos, revisados segundo sua finalidade e ligados às tarefas correspondentes.

Não crie um documento separado para cada análise ou revisão de spec. Reutilize os [modelos locais](<spec editorial/modelos>) de forma proporcional, sem reformatação gratuita de documentos existentes. Correções pequenas não exigem nova iniciativa ou toda a cadeia de revisão.

Mudança de intenção ou requisito retorna à spec; mudança de estratégia retorna ao plano; execução e evidências ficam nas tasks. Preserve IDs e histórico. Pareceres antigos não validam automaticamente versões novas.

## Skills por fase

Leia explicitamente a skill selecionada antes de usá-la. Os caminhos são relativos à raiz; as referências internas de cada skill são relativas à pasta dela.

| Trabalho solicitado | Skill local |
| --- | --- |
| Analisar, elaborar ou revisar a spec | [sdd-editorial-especificar](<spec editorial/skills/sdd-editorial-especificar/SKILL.md>) |
| Elaborar, ajustar ou conferir o plano | [sdd-editorial-planejar](<spec editorial/skills/sdd-editorial-planejar/SKILL.md>) |
| Decompor, acompanhar ou conferir tasks | [sdd-editorial-tarefas](<spec editorial/skills/sdd-editorial-tarefas/SKILL.md>) |
| Selecionar fontes e preparar ficha editorial | [editorial-preparar](<spec editorial/skills/editorial-preparar/SKILL.md>) |
| Elaborar esboço, rascunho ou reescrita delimitada | [editorial-redigir](<spec editorial/skills/editorial-redigir/SKILL.md>) |
| Emitir parecer especializado sobre versão identificada | [editorial-revisar](<spec editorial/skills/editorial-revisar/SKILL.md>) |
| Resolver pareceres, integrar e reconferir alterações | [editorial-integrar](<spec editorial/skills/editorial-integrar/SKILL.md>) |

Os [nove perfis de revisão](<spec editorial/skills/editorial-revisar/references/perfis.md>) cobrem estrutura, fatos/fontes, didática, continuidade, voz/tom, linha/fluidez, preparação linguística, leitura crítica e prova final. Selecione os pertinentes; não imponha nove pareceres a toda correção.

A cadeia pode ser executada sequencialmente pela mesma IA. Papéis distintos não comprovam independência nem autorizam delegação automática. Declare acesso ao histórico e a pareceres anteriores. Revisores emitem pareceres; o integrador aplica as decisões sobre o texto.

## Preservação, voz e evidência

- Preserve fontes, anexos de extração e versões necessárias à comparação. O controle de versão e a preservação de estados anteriores são gerenciados exclusivamente pelo Git (commits e histórico). Não crie pastas de backup manual ou snapshots de arquivos (como `historico/` ou similares) no workspace para simular versionamento. Não exclua fontes nem reorganize o acervo sem escopo autorizado.
- Transcrições e conversas de IA são registros históricos, não comprovação de fatos técnicos ou pessoais. Verifique fontes e sinalize o que não foi conferido.
- Não invente emoções, diálogos, acontecimentos, aprendizados ou resultados do autor. Diferencie relato confirmado, hipótese, metáfora e exemplo fictício.
- Use decisões editoriais e amostras reais para orientar a voz. Markdown selecionado do Obsidian é suficiente; não exige acesso ao cofre inteiro. Erros de notas rápidas não se tornam regras de estilo automaticamente.
- Preserve fatos, ressalvas e trechos que funcionam. Uma revisão pode concluir que não é necessário alterar o texto. Resolva conflitos por intenção, evidência e voz, não por maioria de pareceres.
- Diferencie conferência estrutural, exercício sintético, uso no piloto e apreciação humana. Não declare prazer de leitura, aprendizado ou reconhecimento da voz como comprovados pela IA.

## Conferência e entrega

Ao concluir uma tarefa, registre artefato e versão, critério examinado, evidência, resultado, limitações e pendências. Arquivo produzido sem conferência permanece produzido/aguardando conferência. Reabra o aspecto afetado quando uma mudança invalidar evidência anterior.

Verifique referências, coerência e alterações pertinentes à entrega. Não crie testes que apenas repitam o texto. Validação estrutural de uma skill não comprova comportamento editorial; consulte a cobertura registrada nas tasks e complemente os modos necessários antes de usá-los no piloto.

O piloto escolhido é [01 — Novo mundo, bagagem antiga](<jornada do heroi/01-novo-mundo-bagagem-antiga.md>) e pertence à spec 03. Antes de executá-lo, confira a preparação e o parecer da spec 02, a cobertura dos modos das skills e o plano/tasks da iniciativa 03 quando elaborados. IDs transferidos nas tasks 01 preservam origem, não execução. Não transforme exemplos sintéticos em vivências nem antecipe o piloto durante a análise da preparação.

Retorno autoral ausente permanece pendente. Texto revisado não significa aprovado ou publicado. Publicação exige instrução explícita e registro da versão e do destino.

Ao encerrar a sessão, informe o que mudou, o que foi conferido, os limites e o próximo passo. Mantenha o acompanhamento suficiente para que outra IA retome sem depender da memória da conversa.
