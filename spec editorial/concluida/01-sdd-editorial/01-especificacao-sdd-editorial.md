# Especificação do SDD editorial

> Vigência operacional — 17/10/2026: documento histórico do escopo encerrado. A [iniciativa 05](<../05-ajuste-fluxo-sdd-editorial/05-spec-ajuste-fluxo-sdd-editorial.md>) atualiza procedimento e interfaces; consultar o [guia vigente](../../GUIA_DE_OPERACAO.md) e as tasks da iniciativa ativa. As evidências originais conservam seus limites; esta evolução não reexecuta nem invalida por si só a aceitação histórica.

**ID:** SPEC-EDITORIAL-001  
**Versão:** 0.7 — auditada e arquivada como concluída

**Data:** 2026-10-14

**Estado:** concluída e arquivada no escopo de construção documental e avaliação inicial do método; auditoria e evidências nas tasks 01 v0.22.

**Objeto:** definir e construir a metodologia de escrita, com conferência documental e exercícios iniciais delimitados.

**Decisão vigente do autor:** separar o fechamento do método, a preparação editorial e o piloto. A seção 19 governa o escopo atual. As seções anteriores preservam a evolução da proposta; referências ao piloto como condição de conclusão da iniciativa 01 foram substituídas por essa decisão, sem eliminar seus critérios.

[Índice do projeto](../../../README.md) · [Base do livro](<../../../capitulos estudos/BASE_DO_LIVRO.md>) · [Estrutura e estudo](<../../../capitulos estudos/ESTRUTURA_E_ESTUDO.md>)

## 1. Problema e intenção

O projeto reúne estudo, registros pessoais, narrativa de formação, conteúdo técnico, publicações e um futuro livro. Precisamos transformar esse material em textos coerentes, rastreáveis e com voz própria, preservando as diferenças entre experiência vivida, fonte consultada e criação narrativa.

O SDD editorial deverá explicitar o compromisso de cada texto com o leitor e orientar sua revisão. A especificação precisa permitir descoberta durante a escrita: uma solução narrativa melhor pode justificar sua atualização.

Este primeiro documento é a especificação da metodologia. Vamos detalhá-lo antes de produzir modelos operacionais, skills ou automações. O nome “SDD editorial” designa uma adaptação própria; não representa um framework estabelecido.

## 2. Decisões já recebidas e propostas a avaliar

| Situação | Definição |
| --- | --- |
| Direção confirmada pelo autor | Criar uma metodologia específica para escrita, usando SDD para desenvolver a própria metodologia. |
| Escopo confirmado | Escrita criativa e editorial; não haverá desenvolvimento de código ou aplicação como entrega desta metodologia. |
| Identidade já escolhida | Jornada medieval de RPG/isekai, com bagagem da vida anterior, dificuldades, humor e crescimento; títulos profissionais e referências animescas. |
| Base já existente | Quinze etapas da jornada, sete partes técnicas provisórias do livro e registros de aprendizagem e autoridade. |
| Proposta inicial | Trabalhar em Markdown, com especificações proporcionais ao tamanho e ao risco editorial do texto. |
| Em avaliação | Regras detalhadas, estados, critérios, modelos, responsabilidades e eventual criação de skills. |

Os assuntos técnicos do livro continuam sendo conteúdo editorial. Sua presença não transforma esta iniciativa em um projeto de software.

## 3. Resultado esperado e limites

O método deve permitir recuperar por que um texto existe, para quem foi escrito, em que se apoia, o que ainda falta e como foi revisado. Deve servir ao autor e à IA que colaborar com ele, preservando a decisão autoral sobre voz e experiência pessoal.

Estão no escopo: diretrizes editoriais, referência narrativa, especificação de textos, pesquisa e fontes, elaboração de rascunhos, revisão, continuidade, reaproveitamento e mudanças de direção.

Ficam fora desta primeira entrega: instalar frameworks, criar skills executáveis, automatizar revisões, migrar os documentos atuais, redigir o livro inteiro ou publicar conteúdo. A primeira entrega é este documento de trabalho.

## 4. Mapa da base existente

| Material | Papel no método | Adaptação a investigar |
| --- | --- | --- |
| [Base do livro](<../../../capitulos estudos/BASE_DO_LIVRO.md>) | Aproveitamento editorial e estados do material. | Harmonizar estados e critérios sem criar dois fluxos concorrentes. |
| [Estrutura e estudo](<../../../capitulos estudos/ESTRUTURA_E_ESTUDO.md>) | Sete partes técnicas provisórias e lacunas de formação. | Ligar objetivos de aprendizagem às especificações de capítulos. |
| [Jornada do herói](<../../../jornada do heroi/README.md>) | Quinze etapas do percurso completo. | Relacionar episódios e capítulos sem transformar automaticamente etapas em capítulos. |
| [Universo narrativo](<../../../jornada do heroi/UNIVERSO_NARRATIVO.md>) | Identidade, tom e referências de aventura. | Definir continuidade, liberdade criativa e limites entre metáfora e fato. |
| [Método de registro](<../../../registro da autoridade/METODO_DE_REGISTRO.md>) | Sessões, episódios, decisões e retornos com IDs. | Reutilizar os registros como evidência e matéria-prima. |
| [Canais e autoridade](<../../../registro da autoridade/CANAIS_E_AUTORIDADE.md>) | Destinos públicos e construção de confiança. | Adaptar a apresentação ao canal, mantendo origem e limites das afirmações. |
| [Mapa de origem](<../../../jornada do heroi/MAPA_ORIGEM.md>) | Rastreabilidade dos trechos extraídos da conversa. | Distinguir transcrição histórica de decisão vigente. |

As fontes históricas preservam o que foi dito. Uma afirmação da conversa anterior só entra como orientação atual após avaliação; sua extração não equivale à validação factual.

## 5. Requisitos do método e critérios de avaliação futura

Os vinte requisitos permanecem como contratos do método. A iniciativa 01 entrega sua cobertura documental e os exercícios registrados; os critérios de aplicação ao texto e de apreciação humana abaixo serão examinados na spec 03. Não se declara atendimento prático integral ao encerrar a construção do método.

| ID | O método deverá permitir | Como avaliar no piloto |
| --- | --- | --- |
| REQ-01 | Identificar público, pergunta central e contribuição do texto. | A especificação apresenta esses três itens de forma compreensível. |
| REQ-02 | Relacionar afirmações relevantes a registros ou fontes. | A revisão consegue localizar sua base ou identificar uma pendência. |
| REQ-03 | Distinguir fato, interpretação, hipótese, metáfora e exemplo fictício. | Nenhuma invenção é apresentada como experiência pessoal comprovada. |
| REQ-04 | Preservar voz autoral e espaço para exploração. | O autor avalia se o texto representa sua voz e pode alterar o esboço com justificativa. |
| REQ-05 | Manter continuidade entre jornada, estudo e livro. | O texto indica seus vínculos e respeita os conceitos e fatos já estabelecidos. |
| REQ-06 | Separar revisão factual, didática e literária. | Cada leitura produz achados próprios e pendências identificáveis. |
| REQ-07 | Reaproveitar conteúdo sem multiplicar versões conflitantes. | Publicação e capítulo apontam para o mesmo registro de origem. |
| REQ-08 | Dimensionar o esforço editorial. | Um texto breve exige menos preenchimento que um capítulo. |
| REQ-09 | Registrar mudanças que afetem outros textos. | Uma alteração relevante aponta motivo, documentos afetados e ação necessária. |
| REQ-10 | Distinguir rascunho, texto revisado e texto publicado. | O estado não sugere publicação ou validação que não ocorreu. |
| REQ-11 | Fornecer contexto suficiente e identificado a cada papel editorial. | Cada parecer informa a versão lida, as referências recebidas e suas limitações. |
| REQ-12 | Revisar estrutura antes do acabamento linguístico. | Mudanças de argumento e sequência antecedem a preparação e a prova final. |
| REQ-13 | Examinar tom, ortografia, sintaxe, pontuação e fluidez sem apagar a voz autoral. | As sugestões distinguem erro, ambiguidade e escolha expressiva. |
| REQ-14 | Refatorar textos preservando sentido e rastreabilidade. | A comparação antes/depois conserva fatos, ressalvas e referências ou explicita sua alteração. |
| REQ-15 | Integrar pareceres e encerrar rodadas com critérios claros. | Os achados têm destino, conflitos são decididos e pendências permanecem visíveis. |
| REQ-16 | Avaliar interesse e prazer de leitura qualitativamente. | A leitura identifica trechos concretos de curiosidade, cansaço ou confusão; retorno humano ausente fica indicado. |
| REQ-17 | Reunir análise, especificação e revisão no documento inicial de cada iniciativa. | A spec identifica contexto, requisitos, decisões, achados e parecer de prontidão. |
| REQ-18 | Gerar um plano separado e vinculado à versão da spec. | O plano relaciona entregas, dependências e critérios aos requisitos de origem. |
| REQ-19 | Manter tarefas, implementação e conferência no documento de tasks. | Cada tarefa registra estado, artefato produzido, conferência e pendências; produção e validação são distintas. |
| REQ-20 | Aplicar revisão editorial pertinente aos artefatos gerados e devolver seus resultados às tasks. | Os achados apontam versão e tarefa; documentos de método são avaliados por clareza e coerência, sem exigir narrativa criativa. |

## 6. Regras editoriais candidatas

Estas regras serão refinadas nesta especificação antes de sua adoção como instruções operacionais.

| ID | Regra proposta | Aplicação |
| --- | --- | --- |
| REG-01 | Preservar transcrições e registros de origem; escrever sínteses separadamente. | Uma revisão literária não altera a fonte histórica. |
| REG-02 | Sustentar afirmações de aprendizagem e competência com evidências proporcionais. | Distinguir intenção de estudar, entendimento demonstrado e resultado observado. |
| REG-03 | Usar a aventura para dar sentido ao percurso. | Humor e metáforas ajudam a leitura; conceitos técnicos mantêm precisão. |
| REG-04 | Respeitar o relato pessoal do autor. | Emoções, diálogos, derrotas e conquistas não são preenchidos pela IA como fatos. |
| REG-05 | Admitir episódios sem resolução e progresso sem sofrimento. | A experiência determina o arco; a fórmula narrativa não exige fabricar um conflito. |
| REG-06 | Construir rapport por reconhecimento, honestidade e utilidade. | Evitar promessas de transformação garantida e autoridade baseada apenas em títulos. |
| REG-07 | Permitir exploração antes e durante a especificação. | Descobertas podem mudar o propósito do texto; registrar mudanças relevantes. |
| REG-08 | Escolher a ordem didática do livro conforme o leitor. | Preservar a cronologia nos registros e explicitar reorganizações na narrativa. |
| REG-09 | Identificar fontes e limites das conclusões. | Separar citação, paráfrase, interpretação e resultado próprio. |
| REG-10 | Registrar a participação da IA quando relevante para compreender a produção. | Identificar sugestões, pesquisa e reescritas que ainda dependem de conferência. |
| REG-11 | Vincular pendências ao trecho afetado. | Uma dúvida factual não desaparece apenas porque a redação ficou convincente. |
| REG-12 | Tratar naturalidade como qualidade de leitura, não como detecção de autoria. | Não usar um suposto detector de IA como prova de escrita humana. |
| REG-13 | Manter uma versão de trabalho sob responsabilidade editorial definida. | Revisores emitem pareceres sobre a mesma versão; a integração gera a seguinte. |
| REG-14 | Adequar a revisão à intenção expressiva. | Fragmentos, coloquialismos e pontuação rítmica podem ser escolhas conscientes; corrigir o que prejudica sentido ou consistência. |

## 7. Especificação proposta para cada texto

Uma ficha deverá conter, proporcionalmente ao trabalho:

- Identificação, versão, estado e destino editorial.
- Público, pergunta do leitor e resultado esperado.
- Vínculos com etapa da jornada, parte do livro e registros de origem.
- Fontes disponíveis, afirmações a conferir e lacunas.
- Conteúdo necessário, pré-requisitos e limites de escopo.
- Movimento narrativo possível e espaço de liberdade criativa.
- Variante do português, pessoa narrativa, tempo verbal predominante e referências de voz.
- Relação com o texto anterior e o seguinte, quando integrar uma sequência.
- Critérios factuais, didáticos e literários de revisão.
- Decisões, pendências e próximo passo.

**Forma curta proposta:** intenção, base, direção narrativa e critério de revisão, para textos breves. **Forma completa proposta:** todos os campos pertinentes, para capítulos ou textos que exijam mais pesquisa. Os modelos só serão criados após o detalhamento deste documento.

## 8. Fluxo proposto e aplicação à própria metodologia

| Passo | Para um texto | Para criar nosso SDD editorial |
| --- | --- | --- |
| Explorar | Investigar a ideia e experimentar uma abordagem. | Mapear o acervo, as dificuldades e as necessidades do autor. |
| Especificar | Definir intenção, base e critérios. | Refinar este documento e resolver as decisões necessárias ao piloto. |
| Planejar | Escolher fontes, sequência e tarefas de escrita. | Escolher um episódio piloto e preparar apenas os modelos necessários. |
| Escrever | Produzir um rascunho e registrar descobertas. | Aplicar o método ao episódio e registrar dificuldades de uso. |
| Revisar | Examinar fatos, ensino e qualidade literária. | Comparar o resultado do piloto com os requisitos desta especificação. |
| Incorporar | Registrar a versão e seus vínculos. | Ajustar a metodologia e definir sua primeira versão operacional. |

O fluxo admite retorno a qualquer passo. O estado do processo e o estado editorial são distintos: um capítulo pode voltar à pesquisa sem perder a versão anterior.

Os estados já presentes na base do livro — nota de estudo, caso documentado, caso conferido, texto para leitura e capítulo revisado — serão o ponto de partida. Publicação será registrada separadamente. A nomenclatura final permanece em avaliação.

## 9. Mapa de skills possíveis

As entradas abaixo são capacidades candidatas, ainda sem arquivos `SKILL.md`, comandos ou execução automática. Primeiro verificaremos se instruções simples e modelos bastam. Uma skill só se justifica quando houver um procedimento recorrente e suficientemente definido.

| Capacidade candidata | Entrada → saída | Limite de atuação | Requisitos ligados |
| --- | --- | --- | --- |
| Especificar texto | Ideia e contexto → ficha com lacunas explícitas. | Não decidir silenciosamente fatos ou intenções pessoais. | REQ-01, 04, 08 |
| Mapear fontes | Registros e referências → relações entre afirmações e evidências. | Não tratar uma citação recuperada como fato verificado. | REQ-02, 03 |
| Planejar narrativa | Especificação → alternativas de esboço. | Não inventar acontecimentos autobiográficos. | REQ-03, 04, 05 |
| Redigir com contexto | Ficha e fontes → rascunho identificado. | Não preencher lacunas factuais como certezas. | REQ-02, 03, 04 |
| Revisar precisão e ensino | Rascunho e fontes → achados factuais e didáticos. | Não declarar compreensão do leitor sem retorno ou evidência. | REQ-02, 06 |
| Revisar voz e continuidade | Rascunho e referência narrativa → sugestões literárias e inconsistências. | Preservar a escolha final do autor. | REQ-04, 05, 06 |
| Adaptar e analisar impacto | Texto e destino ou mudança → versão derivada e vínculos afetados. | Não publicar nem atualizar outros textos silenciosamente. | REQ-07, 09, 10 |

Ao detalhar uma skill, definir: quando usar, quando não usar, entradas mínimas, fontes permitidas, sequência, saída, limites, perguntas necessárias e exemplo de avaliação. Uma skill descreve um procedimento reutilizável; um agente assume um papel ao executá-lo. Uma única pessoa ou IA pode executar várias dessas atividades. A cadeia de papéis e suas passagens estão detalhadas na seção 15; ainda não há agentes ou skills implementados.

## 10. Responsabilidades propostas

**Autor:** confirma vivências, intenção, posicionamento, voz e decisões editoriais relevantes; decide a publicação.

**IA colaboradora:** organiza contexto, aponta ambiguidades, propõe alternativas, redige e revisa com indicação das fontes e das incertezas. Sua revisão não equivale a confirmação independente de fatos.

**Leitor ou revisor, quando participar:** oferece retorno sobre clareza, precisão e experiência de leitura. Até que participe, esse retorno permanece pendente.

## 11. Decisões abertas para o detalhamento

| ID | Questão | Ponto de partida proposto |
| --- | --- | --- |
| DEC-01 | Qual leitor terá prioridade? | Explicitar experiência prévia e dificuldade central antes de detalhar capítulos. |
| DEC-02 | Como equilibrar relato e ensino? | Ajustar por tipo de texto; evitar uma proporção universal. |
| DEC-03 | Qual intensidade de humor e fantasia? | Registro histórico: título profissional, subtítulo animesco e metáforas pontuais. Direção de voz substituída por [RA02-15 da spec 02](../02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md#ra02-15--jornada-pessoal-e-autonomia-técnica--2026-10-16): jornada pessoal em primeira pessoa, com humor e retórica, sem limite à abertura. |
| DEC-04 | Quais campos são obrigatórios por formato? | Começar com ficha curta e ampliar apenas onde faltar contexto. |
| DEC-05 | Onde guardar fichas, rascunhos e revisões? | Projetar a organização respeitando as pastas existentes, antes de criar novas. |
| DEC-06 | Como registrar versões e correções? | Definir identificação, histórico relevante e ligação com textos derivados. |
| DEC-07 — definida | Qual texto será o piloto? | Primeiro texto da jornada: 01 — Novo mundo, bagagem antiga. Execução posterior à implementação inicial da metodologia e à definição editorial de onde, como e quando será usado; ver seção 15.8. |
| DEC-08 — escopo inicial definido | O que precisa virar skill? | Cobrir os procedimentos de elaboração da metodologia e de editoração das seções 16.5 e 17.3. O plano definirá o agrupamento; ajustes posteriores dependem do uso. |
| DEC-09 — regra inicial definida | O que impede concluir uma revisão? | Aplicar as categorias e condições das seções 15.5 e 15.7; avaliar sua adequação no piloto. |
| DEC-10 | Qual variante do português e quais convenções editoriais? | Confirmar PT-BR ou PT-PT, estrangeirismos, maiúsculas, diálogos, citações e termos técnicos; não inferir pela localização do autor. |
| DEC-11 | Quais amostras representam a voz desejada? | Selecionar trechos reconhecidos pelo autor e exemplos que ele deseja evitar; o exemplo fictício do universo narrativo é apenas uma referência inicial. |
| DEC-12 | Qual é a intensidade de revisão de cada entrega? | Usar os percursos leve e completo da seção 15 como hipóteses para o piloto. |

## 12. Critérios históricos para a primeira versão operacional

Checklist preservada da proposta anterior à separação. Os itens não marcados não são pendências ativas de 01: seu destino e o atendimento já demonstrado estão reconciliados na seção 20. O piloto e a decisão sobre uma versão 1.0 continuam futuros, em 03.

- [ ] Definir os objetivos e os limites de cada tipo de texto utilizado no piloto.
- [ ] Resolver as decisões abertas que afetem diretamente o piloto.
- [ ] Harmonizar a proposta com a base editorial e o método de registro existentes.
- [ ] Aplicar uma ficha a um episódio real, preservando suas fontes.
- [ ] Produzir e revisar um rascunho pelas três perspectivas: factual, didática e literária.
- [ ] Avaliar os requisitos REQ-01 a REQ-20 com exemplos e registrar os que não foram exercitados.
- [ ] Ensaiar uma refatoração e verificar se sentido, ressalvas, fontes e voz foram preservados.
- [ ] Exercitar a passagem entre revisores, a integração de pareceres e o encerramento de uma rodada.
- [ ] Obter avaliação do autor sobre voz, utilidade e esforço de preenchimento.
- [ ] Reduzir campos ou etapas que gerem esforço sem contribuir para o resultado.
- [ ] Registrar ajustes, limites e pendências antes de definir a versão 1.0.

Esses itens representam trabalho futuro. A existência desta especificação não significa que o método já foi validado.

## 13. Próximo incremento — registro histórico anterior à implementação

Gerar o plano separado desta spec conforme a seção 17. Usar a seção 16 como insumo preliminar, incluindo os procedimentos de elaboração da própria metodologia. Depois gerar as tasks e implementar as entregas na ordem definida. As escolhas de leitor, voz, formato e destino serão detalhadas no documento 02 e precisam estar suficientes antes do piloto **01 — Novo mundo, bagagem antiga**. O suporte genérico pode ser planejado com essas escolhas pendentes.

## 14. Histórico

| Versão | Alteração | Estado |
| --- | --- | --- |
| 0.1 — 2026-10-13 | Especificação inicial da metodologia, com mapa do acervo, requisitos, regras candidatas, capacidades, decisões e avaliação proposta. | Em elaboração; nenhum piloto executado. |
| 0.2 — 2026-10-13 | Análise de lacunas; contexto por papel, sequência de redação, revisão especializada, refatoração, integração e critérios de encerramento. | Propostas para detalhamento; cadeia ainda não executada. |
| 0.3 — 2026-10-13 | Primeira leitura sem pareceres anteriores, ganho e possível perda por sugestão, preservação de trechos que funcionam e escolha do texto 01 como piloto posterior. | Piloto definido, ainda não iniciado; definição editorial e implementação inicial pendentes. |
| 0.4 — 2026-10-13 | Plano de implementação, contratos mínimos, cobertura dos requisitos e dependências do resumo editorial 02. | Planejamento registrado; modelos, skills e piloto ainda não executados. |
| 0.5 — 2026-10-13 | Fluxo spec → plano → tasks → artefatos; procedimentos para elaborar a metodologia; correção da ordem de avanço e revisão de prontidão. | Apta para gerar o plano; implementação e piloto pendentes. |

## 15. Sequência de redação e cadeia editorial

### 15.1. Lacunas encontradas na versão 0.1

A etapa “revisar” agrupava atividades que precisam de critérios e momentos diferentes. O mapa de skills também reunia precisão com didática e voz com continuidade, dificultando identificar a responsabilidade por cada achado. Faltavam preparação linguística, leitura de fluidez, refatoração, contexto por papel, integração de pareceres e encerramento de rodadas.

Há três correções de interpretação: os estados do material não descrevem todas as tarefas editoriais; revisão por vários agentes não prova independência factual; qualidade literária não se reduz à ausência de erros. A cadeia abaixo amplia o método sem transformar escrita em desenvolvimento de software ou exigir uma suíte de testes.

### 15.2. Contexto comum e contexto específico

Cada trabalho parte de um pacote de contexto que referencia documentos existentes, sem copiar todo o acervo para cada agente:

1. **Projeto:** propósito, leitor prioritário, diretrizes vigentes e limites autorais.
2. **Obra:** parte do livro, etapa da jornada, conceitos já apresentados, cronologia real e vocabulário narrativo pertinente.
3. **Texto:** especificação, versão exata do rascunho, destino e pergunta central.
4. **Base documental:** registros, fontes e afirmações pendentes relevantes ao trecho.
5. **Voz:** variante linguística, amostras escolhidas pelo autor, intensidade de humor e escolhas expressivas.
6. **Tarefa:** aspecto a revisar, extensão do trecho, critérios, formato do parecer e permissões de edição.

O revisor de continuidade recebe também resumos ou trechos vizinhos; o factual recebe as fontes utilizadas; o linguístico recebe as convenções de escrita. Se faltar contexto necessário, o parecer declara a limitação e solicita o elemento específico. Não preencher lacunas pessoais ou técnicas por suposição.

Conflitos entre documentos são registrados para decisão. Instruções atuais do autor orientam o trabalho; transcrições históricas e exemplos fictícios não substituem decisões editoriais vigentes. Quando uma instrução pedir mudança de direção, atualizar a especificação e identificar os textos afetados.

### 15.3. Da matéria-prima à versão para leitura

| Ordem | Trabalho e papel | Entrega e condição de passagem |
| --- | --- | --- |
| 1 | Curadoria de contexto e fontes | Dossiê enxuto com origem, lacunas e vínculos. Há base suficiente para o escopo escolhido, ou ele é reduzido. |
| 2 | Especificação editorial | Pergunta, leitor, intenção, limites e critérios do texto. Dúvidas que impedem escrever estão identificadas. |
| 3 | Edição de desenvolvimento | Esboço com função de cada seção, progressão didática e movimento narrativo. O percurso atende à intenção. |
| 4 | Redação | Primeiro rascunho completo, com pendências visíveis. É permitido descobrir outra estrutura e propor ajuste na especificação. |
| 5 | Revisão estrutural | Parecer sobre foco, ordem, lacunas, redundâncias, abertura, transições e fechamento. Problemas estruturais são resolvidos antes do polimento. |
| 6 | Revisões factual, didática e de continuidade | Pareceres distintos sobre a mesma versão estabilizada. Podem ocorrer em paralelo porque não alteram diretamente o texto. |
| 7 | Integração e refatoração | Editor responsável seleciona alterações e produz nova versão. Mudanças de sentido retornam à revisão pertinente. |
| 8 | Edição de linha, tom e leitura | Ajustes de ritmo, concretude, cadência, humor e voz. Preservar precisão e personalidade. |
| 9 | Preparação linguística | Revisão de ortografia, concordância, regência, sintaxe, pontuação e convenções, respeitando a variante escolhida. |
| 10 | Prova final e leitura autoral | Conferência da versão consolidada, títulos, referências, links, repetições residuais e alterações introduzidas. Registrar a apreciação do autor e, quando disponível, de leitores. |

A unidade de redação pode ser seção, episódio ou capítulo. Cada unidade precisa cumprir sua função e se conectar ao conjunto; não é obrigatório impor missão, derrota e vitória a todas elas. O capítulo pode alternar cena, explicação, exemplo e reflexão conforme a necessidade do leitor.

**Percurso leve:** para um texto curto, combinar os papéis em uma ficha breve, um rascunho e uma revisão integrada seguida de leitura final. Manter explícitas as dúvidas factuais e a voz escolhida.

**Percurso completo:** para capítulos, textos com muitas fontes ou mudanças relevantes, aplicar as passagens acima com pareceres separados. Intensificar a revisão conforme as dificuldades reais; a quantidade de agentes não é um objetivo.

### 15.4. Especialidades de revisão a mapear em skills

| Papel | Perguntas principais | Limite do parecer |
| --- | --- | --- |
| Editor de desenvolvimento | O texto cumpre a promessa? A ordem ajuda? Há conteúdo ausente ou dispensável? | Não reestruturar a obra inteira sem apontar impacto e motivo. |
| Revisor factual e de fontes | As afirmações correspondem às fontes? A conclusão excede a evidência? Citações e atribuições estão corretas? | Concordância entre IAs não substitui consulta à fonte. |
| Editor didático | O leitor tem os pré-requisitos? O exemplo explica? Há saltos de raciocínio? | Uma simulação de leitor é hipótese editorial, não retorno de uma pessoa real. |
| Editor de continuidade | Cronologia, termos, metáforas e conhecimento do narrador são consistentes? O capítulo repete ou contradiz outro? | Distinguir aprendizado posterior de conhecimento disponível no momento vivido. |
| Editor de voz e tom | O autor se reconheceria? O humor combina com o assunto? Há exagero, tom professoral ou linguagem promocional? | Propor alternativas localizadas, sem uniformizar toda a escrita. |
| Editor de linha e fluidez | As frases se conectam? Há abstração excessiva, ritmo monótono, clichês ou explicações repetidas? | Não exigir frases sempre curtas nem remover uma repetição com função expressiva. |
| Preparador linguístico | Há erro ortográfico, ambiguidade sintática ou pontuação que prejudica o sentido? As convenções são consistentes? | Separar correção normativa de preferência e licença estilística. |
| Leitor crítico | Onde surge curiosidade, prazer, cansaço ou vontade de abandonar a leitura? | Apontar trechos e razões; não prometer reação universal do público. |
| Revisor de prova | A versão final incorporou as decisões? Restaram gralhas, links quebrados ou inconsistências de apresentação? | Se houver mudança substancial, devolver à edição em vez de reescrever na prova. |

Os papéis refinam o mapa da seção 9. Cada futura skill deverá referenciar os requisitos que atende e devolver achados no contrato abaixo. O editor responsável coordena as passagens; revisores não iniciam reescritas concorrentes do mesmo arquivo.

### 15.5. Pareceres, conflitos e refatoração textual

Cada achado informa: **papel, versão examinada, seção ou trecho, categoria, problema, motivo, referência ao critério ou fonte, sugestão, ganho esperado, possível perda e importância**. Preferir uma explicação local e uma alternativa útil a avaliações genéricas como “deixar mais humano”.

**Primeira leitura sem pareceres anteriores:** cada revisor recebe o texto, a especificação, as fontes e as decisões vigentes necessárias à sua tarefa, mas não os pareceres dos outros revisores. Registra sua avaliação antes de consultar essas avaliações. Depois, o editor reúne os achados para integração. Isso reduz a influência entre pareceres; não comprova independência factual. Quando a mesma sessão já tiver acesso aos pareceres anteriores, declarar essa limitação em vez de chamar a leitura de independente. Nas rodadas dirigidas de reconferência, os achados anteriores são fornecidos para verificar sua resolução.

**Responsabilidade por sugestão:** explicar o benefício pretendido e o que a alteração pode enfraquecer, como precisão, ressalva, ritmo, humor ou personalidade. Se nenhuma perda for identificada, registrar isso brevemente. “Mais elegante” ou “mais humano” não bastam como justificativa. Uma correção obrigatória também deve preservar o sentido no contexto.

**Preservação do que funciona:** o parecer pode recomendar manter uma passagem, identificando sua função e por que ela atende à intenção. Não há quantidade mínima de alterações por revisor. Essas recomendações protegem escolhas expressivas durante a integração, sem impedir uma mudança posterior justificada.

Importâncias propostas:

- **Impeditivo:** compromete a integridade ou a intenção central, como invenção autobiográfica, contradição factual relevante ou conclusão sem base necessária.
- **Revisão necessária:** prejudica compreensão, progressão ou consistência; precisa de correção ou justificativa explícita do editor.
- **Sugestão:** alternativa expressiva ou preferência que o autor pode recusar.

O editor registra cada achado como acolhido, recusado com motivo ou pendente. Pareceres conflitantes são resolvidos pela intenção do texto, pelas fontes e pela voz escolhida; impasses de intenção ou vivência voltam ao autor. Não decidir por maioria de agentes.

**Refatorar um texto** significa reorganizar, cortar, dividir, fundir ou reescrever para melhorar sua função. Antes de alterar, identificar o que deve ser preservado: fatos, argumento, ressalvas, fontes, função narrativa e traços de voz. Depois, comparar a versão anterior com a nova e registrar o efeito pretendido. Se mudar a tese, o escopo ou a interpretação factual, tratar como mudança editorial e atualizar a especificação, não como simples polimento.

Exemplos de retorno dirigido: reorganização de explicação volta à leitura didática; mudança de conclusão volta à conferência factual; alteração de metáfora volta à continuidade; mudança de pontuação que altera sentido requer reler o trecho no contexto. Não reiniciar toda a cadeia após cada vírgula corrigida.

### 15.6. Escrita natural e prazer de leitura

Avaliar a presença de detalhes concretos, intenção reconhecível, progressão, variação de ritmo, transições e espaço para a interpretação do leitor. Observar também excesso de frases genéricas, explicação de piadas, dramatização repetitiva e conclusões que apenas repetem a abertura. Esses são pontos de observação, não proibições universais.

Uma leitura em voz alta pode revelar tropeços, frases excessivamente carregadas e pontuação incompatível com a cadência desejada. Se for realizada, registrar os trechos afetados; não declarar a leitura como executada quando houve apenas análise silenciosa.

Para cada aspecto literário, usar **funciona / precisa de ajuste / não avaliado**, acompanhado de trecho e justificativa. Não definir nota automática de “humanidade” nem prometer que um texto será prazeroso para todos. A IA pode antecipar dificuldades; a apreciação do autor e o retorno de leitores oferecem evidência diferente, que deve ser identificada como tal.

### 15.7. Encerramento e avaliação do piloto

Uma rodada termina quando não restam achados impeditivos abertos, as revisões necessárias foram resolvidas ou justificadas, a prova corresponde à versão integrada e as pendências de pesquisa ou retorno humano estão declaradas. Quando falta avaliação do autor, marcar “pronto para leitura autoral”, sem presumir sua aprovação.

Como limite inicial a experimentar, realizar uma rodada completa e uma rodada dirigida aos problemas encontrados. Se o texto continuar instável, retornar à especificação ou ao esboço e registrar a causa; não acumular polimento indefinidamente. Esse limite é uma hipótese de trabalho, não autorização para ignorar problemas.

O piloto deve registrar o que melhorou entre versões, o que perdeu voz ou clareza, quais pareceres foram úteis, onde houve retrabalho e qual esforço foi exigido. Avaliar também uma alteração que preserve o sentido e outra que exija reconsiderar a especificação, sem inventar acontecimentos para construir esses exemplos.

O resultado será uma decisão sobre simplificar, manter ou ajustar cada passagem. Skills executáveis, modelos separados e automações continuam fora desta revisão documental. A implementação inicial necessária ao piloto acontecerá em uma etapa posterior; o piloto avaliará essa implementação antes de sua consolidação.

### 15.8. Piloto escolhido e condições de início

**Decisão do autor:** usar o primeiro texto da jornada, [01 — Novo mundo, bagagem antiga](<../../../jornada do heroi/01-novo-mundo-bagagem-antiga.md>), como piloto após a implementação inicial da spec e a definição editorial. O arquivo atual é a base de planejamento da etapa; suas cenas propostas não constituem, por si só, um relato autobiográfico confirmado.

Usar como apoio o [anexo 01](<../../../jornada do heroi/01-texto-anexo.md>) e a [ficha de registro da etapa 01](<../../../jornada do heroi/01-novo-mundo-bagagem-antiga.md#acompanhamento>). Confirmar com o autor os detalhes pessoais necessários à redação. Preservar uma versão de referência para comparar o rascunho e o texto revisado.

Antes de iniciar o piloto, definir:

| Dimensão | Decisão necessária | Estado |
| --- | --- | --- |
| Onde | Destino editorial do texto: uso interno, canal público ou posição na obra; localização dos arquivos de trabalho e versões. | Pendente. |
| Como | Leitor, formato, extensão pretendida, voz, variante do português, intensidade de humor e percurso de revisão. | Pendente. |
| Quando | Momento de produção e uso, dependências e eventual ocasião de publicação; uma data só será registrada quando definida. | Pendente. |
| Implementação inicial | Modelos, procedimentos e skills que forem escolhidos para executar o percurso de revisão. | Pendente. |

**Sequência acordada:** concluir as definições necessárias → implementar o método inicial → executar o piloto no texto 01 → avaliar e ajustar a metodologia. A publicação, se escolhida como destino, permanece uma decisão separada da realização do piloto.

Na avaliação, comparar rascunho original e versão revisada, percepção do autor sobre voz, clareza e prazer de leitura, esforço exigido e utilidade dos pareceres. Conferir também os três ajustes: leitura inicial sem influência dos pareceres disponíveis, benefício e possível perda das sugestões, e preservação consciente dos trechos que funcionam. Registrar limitações e etapas não executadas.

**Estado atual:** piloto definido e não iniciado. Esta revisão não redige nem modifica o texto 01.

## 16. Insumos preliminares para o plano

### 16.1. Limite desta etapa

A primeira análise está concluída. Esta seção preserva as propostas da versão 0.4 como insumos para o plano separado; não é o plano vigente nem um quadro de execução. O método permanece provisório até ser usado e avaliado. As entregas abaixo ainda não existem. Ao gerar o plano, consolidar nele a sequência e os caminhos escolhidos; nesta spec permanecem os requisitos e contratos que essas entregas devem cumprir.

O documento 01 define **como conduzir o trabalho editorial**. O [documento 02](../02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md) reúne **as escolhas editoriais que orientarão esse trabalho**. Podemos preparar procedimentos e modelos genéricos enquanto essas escolhas estão abertas; o piloto depende das definições necessárias ao texto 01.

### 16.2. Regras de operação da primeira implementação

1. Cada trabalho identifica a especificação, o texto, a versão e os documentos de contexto usados. Uma decisão editorial ausente permanece pendente; o agente não escolhe silenciosamente pelo autor.
2. O editor responsável organiza as passagens e integra as alterações. Os revisores entregam pareceres sobre uma versão identificada e não editam simultaneamente o mesmo rascunho.
3. A primeira leitura dos revisores não recebe pareceres dos demais; as decisões e fontes necessárias continuam disponíveis. Se houver exposição prévia, registrar a limitação.
4. Cada sugestão explica problema, ganho e possível perda. Recomendar manter uma passagem é um resultado válido.
5. Mudanças relevantes preservam a versão anterior e registram motivo, efeitos sobre sentido e textos relacionados. Fatos novos exigem conferência; mudanças de intenção exigem atualização da ficha.
6. Aplicar apenas as revisões pertinentes à entrega. Um aspecto dispensado recebe motivo; um aspecto não examinado fica como não avaliado.
7. Encerrar conforme a seção 15.7, mantendo explícitas as pendências e a necessidade de leitura autoral. Publicação é um acontecimento separado, que exige decisão do autor.

Essas regras consolidam as seções anteriores como base de implementação; não acrescentam obrigação de executar todas as especialidades para todo texto.

### 16.3. Entregas mínimas e ordem de construção

Os nomes abaixo são nomes planejados, relativos à pasta `spec editorial`. A localização dos textos, registros e publicações será definida no documento 02, preservando a organização existente.

| Ordem / ID | Entrega planejada | Conteúdo mínimo | Dependência | Conferência da entrega |
| --- | --- | --- | --- | --- |
| 1 / IMP-01 | `GUIA_DE_OPERACAO.md` | Ordem das passagens, papéis, percurso leve e completo, estados e encaminhamento de lacunas. | Seções 8, 15 e 16 deste documento. | O guia permite identificar próximo passo, responsável e condição de passagem sem redefinir a metodologia. |
| 2 / IMP-02 | `modelos/ficha-editorial.md` | Contexto, intenção, leitor, origem, fontes, esboço, restrições, critérios e pendências; forma curta e completa no mesmo modelo. | IMP-01 e contrato da seção 16.4. | É possível separar escolha editorial ausente de informação factual ainda não confirmada. |
| 3 / IMP-03 | `modelos/parecer-editorial.md` | Papel, versão, contexto recebido, achados, trechos a preservar e limitações. | IMP-01 e contrato da seção 16.4. | Sugestões, correções necessárias e impeditivos ficam distintos; ganho e possível perda estão explícitos. |
| 4 / IMP-04 | `modelos/integracao-e-avaliacao.md` | Destino dos achados, conflitos, alterações, reconferências, leitura final e avaliação do esforço e da voz. | IMP-02 e IMP-03. | A comparação entre versões explica decisões e separa revisão concluída, apreciação autoral e publicação. |
| 5 / IMP-05 | Skills editoriais mínimas | Procedimentos de preparação, redação, revisão e integração descritos na seção 16.5. | IMP-01 a IMP-04. | Cada skill tem entrada, saída, limites e referências aos modelos, sem copiar regras divergentes. |
| 6 / IMP-06 | Conferência documental do conjunto | Leitura dos modelos e procedimentos, cobertura dos requisitos, links e contradições. | IMP-01 a IMP-05. | Não há passagem sem entrada ou saída definida; pendências do 02 aparecem como dependências. |
| 7 / IMP-07 | Piloto no texto 01 | Aplicação do método ao material escolhido e avaliação separada da spec e das skills. | IMP-06 e decisões editoriais necessárias do 02. | Há evidências de uso e apreciação do autor; limitações e ajustes ficam registrados. |

**Estado de IMP-01 a IMP-07:** pendentes. A conferência documental verifica a organização e a coerência dos artefatos; a utilidade da metodologia será avaliada no piloto.

### 16.4. Contratos dos modelos

**Ficha editorial:** identificação e versão; tipo de entrega; etapa da jornada e parte do livro, quando aplicável; intenção e pergunta; público e pré-requisitos; escolhas recebidas do 02; registros e fontes com localização relevante; fatos confirmados e lacunas; direção narrativa e esboço; critérios de revisão; percurso escolhido; próximo passo. O esboço pode nascer depois da ficha e evoluir nela.

Na forma curta, agrupar os campos em intenção, contexto e base, direção e critérios. Em ambas as formas, identificar versão e pendências. O preenchimento não exige inventar uma parte do livro para uma postagem ou um conflito para um relato.

**Parecer editorial:** identificação do texto e da versão; papel e escopo; documentos recebidos; acesso ou não a pareceres anteriores; achados com trecho, motivo, critério ou fonte, sugestão, ganho, possível perda e importância; passagens que convém preservar; aspectos não avaliados. Um parecer sem alterações pode registrar que a leitura não encontrou problemas no escopo examinado, com seus limites.

**Integração e avaliação:** versão de partida; pareceres considerados; decisão por achado e justificativa; conflitos e sua resolução; alterações e efeitos; versão resultante; reconferências necessárias e realizadas; apreciação autoral recebida ou pendente; esforço percebido; resultado da avaliação documental e das skills em campos separados. Retorno de leitores e publicação só são registrados quando ocorrerem.

Para evitar nova nomenclatura concorrente, manter os IDs existentes dos registros de origem. Nos materiais editoriais, usar identificação local estável do texto e número de versão, definidos no guia de operação, sem renumerar sessões e episódios históricos.

### 16.5. Skills mínimas a implementar

| Procedimento candidato | Entrada → saída | Responsabilidade e limites |
| --- | --- | --- |
| Preparar trabalho editorial | Pedido, acervo pertinente e decisões do 02 → ficha com contexto e lacunas. | Recuperar fontes, delimitar escopo e formular perguntas específicas; não preencher vivências ausentes. |
| Planejar e redigir | Ficha e base suficiente → esboço e rascunho identificado. | Trabalhar intenção, progressão e narrativa; marcar hipóteses e propor alterações da ficha quando necessário. |
| Revisar por especialidade | Ficha, versão do texto, referências e papel selecionado → parecer. | Aplicar uma das perspectivas da seção 15.4 por leitura, distinguindo contexto disponível e limites. |
| Integrar e refatorar | Rascunho e pareceres → versão revisada e registro de integração. | Resolver achados, preservar passagens eficazes e encaminhar reconferências; não presumir aprovação do autor. |

Esses quatro procedimentos cobrem a produção editorial. Somam-se a eles os procedimentos para elaborar a metodologia da seção 17.3. As especialidades serão perfis do procedimento de revisão, com critérios próprios; separar uma especialidade em outra skill somente se o uso mostrar necessidade. A revisão final utiliza o perfil de prova, e a apreciação humana continua distinta da avaliação da IA.

Na implementação, definir o local e o formato de instalação das skills conforme o ambiente usado. Os nomes acima descrevem funções, não comandos já disponíveis. Não é necessário executar agentes em paralelo para usar o método; a passagem de contexto e a responsabilidade editorial devem funcionar também sequencialmente.

### 16.6. Cobertura dos requisitos

| Requisitos | Entregas responsáveis | Evidência esperada posteriormente |
| --- | --- | --- |
| REQ-01, 02, 03 | IMP-02 e preparação/revisão de IMP-05. | Intenção explícita, fontes localizáveis e distinção entre fato, interpretação e invenção. |
| REQ-04, 16 | IMP-02, IMP-03, IMP-04 e perfis de voz/leitura. | Sugestões fundamentadas e apreciação do autor sobre voz e experiência de leitura. |
| REQ-05, 07, 09 | IMP-02, IMP-04 e perfis de continuidade/integração. | Vínculos com a origem, relações entre textos e impactos das mudanças. |
| REQ-06, 11, 13 | IMP-03 e revisão por especialidade de IMP-05. | Pareceres com contexto, versão e critérios distintos por leitura. |
| REQ-08, 12 | IMP-01, IMP-02 e execução de IMP-05. | Percurso proporcional e revisão estrutural anterior ao acabamento. |
| REQ-10, 14, 15 | IMP-01, IMP-04 e integração de IMP-05. | Histórico de alterações, sentido preservado ou mudança justificada e encerramento explícito. |

IMP-06 confere a cobertura planejada; IMP-07 verifica seu uso real. Esta tabela não marca requisitos como atendidos. A cobertura dos REQ-17 a REQ-20 deve ser acrescentada no plano por meio dos procedimentos e contratos da seção 17.

### 16.7. Dependências editoriais e condição para avançar

O documento 02 deve fornecer, para a entrega do piloto: destino e localização de trabalho; leitor e intenção; formato e extensão pretendida; voz, variante do português e intensidade de humor; momento de uso e condição de eventual publicação. Uma escolha consciente de uso apenas interno é válida. Não é necessário definir todo o calendário de postagens para produzir um texto.

Enquanto essas decisões estiverem abertas, é possível construir IMP-01 a IMP-06 com campos pendentes explícitos. A definição editorial deve estar suficiente antes de iniciar IMP-07. Isso permite implementar o suporte genérico sem antecipar decisões sobre o conteúdo ou os canais.

**Próximo passo concreto:** gerar o plano separado, seguido do documento de tasks. A criação do guia, dos modelos e das skills será conduzida pelas tarefas. A execução no texto 01 permanece condicionada às definições do documento 02.

## 17. Organização documental acordada

### 17.1. Três documentos de trabalho e seus artefatos

| Passo | Documento | Conteúdo e responsabilidade |
| --- | --- | --- |
| Analisar, especificar e revisar | Spec inicial | Contexto, necessidades, escopo, requisitos, regras, lacunas, alternativas, decisões e revisão de consistência. Atualizar a própria spec quando houver mudança de intenção ou de comportamento esperado. |
| Planejar | Plano separado | Versão da spec utilizada, entregas, organização dos arquivos, dependências, sequência, cobertura dos requisitos e critérios de conferência. Atualizar quando mudar a estratégia de execução. |
| Executar e conferir | Tasks separadas | Tarefas, implementação, evidências de conferência, achados e pendências. Atualizar durante todo o trabalho; não criar outro documento obrigatório apenas para acompanhar a implementação. |
| Produzir e validar | Artefatos gerados | Guia, modelos, skills, documentos ou textos previstos no plano. Aplicar as revisões editoriais pertinentes e vincular o resultado às tasks. |

Análise e revisão não exigem documentos separados. Pareceres extensos podem ser anexados quando úteis, mas a spec registra as decisões sobre seu próprio conteúdo e as tasks registram o resultado da conferência das entregas. A avaliação do piloto pode ser uma entrega prevista no plano, sem se tornar um quarto documento obrigatório para toda iniciativa.

Para esta iniciativa, os documentos são esta spec, o [plano 01](01-plano-sdd-editorial.md) e as [tasks 01](01-tasks-sdd-editorial.md). Plano e tasks já foram elaborados; a implementação está em andamento, com resultados registrados nas tasks. O prefixo identifica a iniciativa, não o número da fase. O documento `02-resumo-editorial-onde-como-quando.md` é outra spec e poderá ter seu próprio plano e tasks; não corresponde à fase de planejamento da spec 01.

### 17.2. Contratos e passagem entre documentos

**Spec → plano:** contexto, escopo, requisitos e critérios estão identificados; os achados impeditivos de planejamento foram resolvidos; pendências restantes têm destino e indicam o momento em que precisam ser resolvidas. O parecer de prontidão fica na spec. A revisão documental não equivale a validação do método em uso.

**Plano → tasks:** cada entrega tem função, dependências e critério de conferência; todos os requisitos estão ligados às entregas; caminhos e agrupamento das skills são definidos. O plano informa a versão da spec que orientou sua elaboração. Não pode criar regras contrárias à spec sem atualizar a decisão nela.

**Tasks → artefatos conferidos:** cada tarefa contém ID estável, requisito relacionado, resultado esperado, dependências, responsável ou papel, estado, localização do artefato e versão conferida, resultado da conferência e pendências. Estados mínimos: pendente, em execução, produzida/aguardando conferência, concluída e bloqueada com motivo. A conclusão depende do critério de entrega e da conferência; escrever o arquivo não basta.

**Retorno de revisão:** achados sobre uma entrega voltam à tarefa correspondente. Se revelarem problema na intenção ou nas regras, registrar a decisão nesta spec e atualizar o plano e as tarefas afetadas. Reabrir uma tarefa quando uma mudança invalidar sua conferência, preservando a evidência anterior e seu contexto.

### 17.3. Procedimentos para elaborar e evoluir a metodologia

| Procedimento a mapear em skill | Entrada → saída | Limite e documento de destino |
| --- | --- | --- |
| Analisar contexto e necessidades | Pedido e acervo → problema, objetivos, restrições, lacunas e perguntas. | Registrar na spec; distinguir fatos, propostas e decisões do autor. |
| Elaborar especificação | Análise e decisões → requisitos, regras, limites e critérios. | Atualizar a spec sem misturar tarefas concluídas com intenções futuras. |
| Revisar consistência da spec | Versão da spec e referências → achados, correções e parecer de prontidão. | Registrar na spec; indicar pendências que bloqueiam o plano e as que pertencem a etapas posteriores. |
| Elaborar plano | Spec revisada → entregas, sequência, dependências e cobertura. | Gerar plano separado; não implementar artefatos durante o planejamento. |
| Elaborar e acompanhar tasks | Plano e spec → tarefas delimitadas, atualizadas com implementação e conferência. | Registrar evidências e motivos de bloqueio; não declarar conclusão apenas pela geração de conteúdo. |
| Implementar e conferir entregas | Tarefa, plano e contexto → artefato e resultado de revisão. | Usar as capacidades de autoria apropriadas e devolver os achados às tasks. |

O plano definirá quais procedimentos compartilham uma skill e quais precisam de arquivos próprios, preservando as entradas e saídas de cada etapa. Na criação inicial dessas skills, o processo será aplicado manualmente com esta spec como referência; não presumir que skills ainda inexistentes já conduziram a análise.

As skills de editoração da seção 16.5 validam também os documentos da metodologia, com escopo adequado: clareza, coerência, precisão, língua e utilidade. Humor, arco narrativo e prazer de leitura criativa são critérios pertinentes aos textos da jornada, não exigências artificiais para um plano ou uma lista de tarefas. Conferir uma skill inclui verificar seu contrato de uso; polimento linguístico isolado não demonstra que o procedimento funciona.

## 18. Revisão de prontidão para o plano — versão 0.5

### 18.1. Achados e correções desta revisão

| Achado | Correção aplicada | Situação |
| --- | --- | --- |
| O plano estava incorporado à spec, e o próximo passo saltava diretamente para o guia. | Seção 16 identificada como insumo preliminar; seções 13 e 17 determinam plano separado e depois tasks. | Resolvido para planejamento. |
| As quatro skills iniciais cobriam redação, mas não a elaboração da própria metodologia. | Seção 17.3 inclui análise, especificação, revisão, planejamento e tarefas. | Resolvido no escopo; agrupamento fica para o plano. |
| DEC-08 adiava toda definição de skills para depois do piloto, embora este dependesse delas. | Escopo inicial definido e refinamento posterior preservado. | Resolvido. |
| A numeração 02 poderia ser confundida com o plano da iniciativa 01. | Prefixos por iniciativa e natureza independente da spec 02 explicitados. | Resolvido. |
| Não havia contrato suficiente para atualizar implementação e conferência nas tasks. | Campos, estados, evidências e reabertura definidos na seção 17.2. | Resolvido. |

### 18.2. Pendências e momento de resolução

| Pendência | Onde resolver | Impede gerar o plano? |
| --- | --- | --- |
| Leitor, voz, variante do português, formato, destino e momento de uso do piloto. | Spec 02, antes do piloto. | Não; o plano deve registrar a dependência. |
| Caminhos finais, agrupamento e instalação das skills. | Plano 01, antes das tarefas de criação. | Não; são decisões próprias do planejamento. |
| Campos operacionais por formato, identificação das versões e harmonização dos estados. | Plano e entregas de guia/modelos, respeitando os contratos desta spec. | Não; exigem conferência antes do piloto. |
| Adequação real do esforço, voz e cadeia de revisão. | Piloto e avaliação posterior. | Não; ainda não pode ser declarada validada. |

### 18.3. Parecer

**Apta para elaboração do plano.** Há objetivo, escopo, requisitos identificados, contratos de entrada e saída, critérios de revisão, destino das pendências e separação entre spec, plano, tasks e artefatos. Nesta revisão não restou achado impeditivo para o planejamento.

Este parecer resulta de revisão documental da IA colaboradora, com acesso ao histórico; não é revisão independente nem aprovação autoral do conteúdo futuro. A metodologia não está implementada ou validada em uso. O próximo artefato é `01-plano-sdd-editorial.md`, com cobertura dos REQ-01 a REQ-20 e das duas famílias de procedimentos: elaboração da metodologia e editoração.

### 18.4. Revisão do detalhamento das skills no plano

O [plano, versão 0.2](01-plano-sdd-editorial.md), foi revisto quanto à suficiência das definições das skills. A versão inicial identificava papéis, mas deixava implícitos decisões de contexto, tratamento de lacunas, limites de atuação e avaliação de comportamento.

Foram detalhados no plano: contratos por skill; estrutura e carregamento das referências; referência de voz recebida do documento 02; situações curtas de avaliação; condição de prontidão para o piloto. Esses ajustes concretizam os requisitos existentes e não alteram o escopo da spec 0.5.

**Conclusão:** o detalhamento é suficiente para gerar tarefas de autoria e conferência das skills. A qualidade de sua execução ainda não foi demonstrada. A voz depende de material e decisões do autor; o procedimento não pode suprir essas entradas por invenção. O próximo artefato passa a ser `01-tasks-sdd-editorial.md`.

### 18.5. Conferência final do plano para tasks

Revisado o plano 0.3 em relação aos contratos desta spec e às dependências do documento 02. Foram esclarecidos: criação manual das primeiras tasks antes de existir sua skill; cobertura de avaliação por modo e perfil; separação entre texto revisado e avaliação autoral concluída; uso de amostras Markdown sem dependência do Obsidian. Corrigida também a indicação desatualizada de que o plano ainda não existia.

**Parecer: apto para gerar tasks.** Não há impedimento documental identificado nesta revisão. Os requisitos permanecem os da spec 0.5. Definições de voz e destino continuam necessárias antes do piloto, e a avaliação prática das skills permanece futura. A revisão foi realizada com acesso ao histórico, sem alegação de independência.

## 19. Encerramento e redistribuição autorizada — versão 0.6

### 19.1. Decisão e limites vigentes

Em 2026-10-14, o autor solicitou encerrar a spec 01, transferir o piloto para a spec 03 e analisar na spec 02 o que falta antes dele: textos de referência, tom, skills, história e contexto. Esta é uma mudança explícita de escopo, não uma declaração de execução do trabalho transferido.

| Iniciativa | Responsabilidade vigente | Condição de conclusão |
| --- | --- | --- |
| 01 — Método | Guia, seis modelos, sete skills, nove perfis, conferência integrada e exercícios iniciais. ENT-01 a ENT-06; T01-001 a T01-017. | Evidências documentais e dos percursos exercitados registradas, com limitações e pendências posteriores encaminhadas. |
| [02 — Preparação editorial](../02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md) | Analisar acervo e lacunas; definir história, contexto, voz/tom, leitor, formato e condições de uso; avaliar adequação e cobertura das skills para o percurso pretendido. | Contexto suficiente e decisões necessárias recebidas; complementos ou ajustes das skills pertinentes conferidos antes de liberar seu uso. |
| [03 — Piloto](../../changes/03-piloto-editorial/03-piloto-editorial.md) | Preparar ficha final, escrever, revisar, integrar, receber avaliação autoral e avaliar o método em uso. | Texto e avaliação documentados; ajustes necessários resolvidos ou encaminhados com critérios, sem presumir aprovação ou publicação. |

ENT-07 e T01-018 a T01-021 deixam o escopo ativo de 01 e ficam rastreadas na spec 03. PEN-01 e a análise/complementação condicional de PEN-02 passam à spec 02; PEN-03 passa à spec 03. IDs anteriores são preservados como origem. Não há cancelamento dos critérios de voz, fatos, fontes, versões, revisão ou apreciação humana.

### 19.2. Conferência de fechamento

Base examinada: plano 0.3 e tasks 0.20 anteriores à separação; registros T01-015 a T01-017; entradas, saídas e cobertura de T01-016; contratos das sete skills v0.1 e nove perfis. Conferência pela IA responsável pelas alterações, com acesso ao histórico e aos pareceres anteriores; não é avaliação independente.

- Os artefatos da metodologia têm registros de produção/conferência nas tasks. A revisão presente verifica o fechamento e a transferência; não repete nem amplia as validações estruturais históricas.
- E01–E07 preservam saídas e limites. Em E07, a integração preserva o texto; não comprova capacidade de refatoração substancial. Voz real, esforço autoral e prazer de leitura continuam sem avaliação humana.
- A suficiência de contexto para escrever ainda não está demonstrada: o texto 01 é planejamento e as cenas não constituem autobiografia confirmada. Essa análise pertence agora a 02.
- O plano, as tasks e a orientação de retomada precisam apontar para a divisão 01 → 02 → 03. Ajustados nesta revisão; pareceres históricos continuam limitados às versões que examinaram.

**Parecer:** iniciativa 01 encerrada no novo escopo autorizado. Não foi identificado impeditivo remanescente de construção documental neste recorte. O encerramento não significa que todas as modalidades das skills foram avaliadas ou que a metodologia foi aprovada em uso real. Defeitos futuros no método poderão reabrir apenas os aspectos afetados.

### 19.3. Histórico e próximo passo

Versão 0.6: separação autorizada do escopo; plano atualizado para 0.4 e tasks para 0.21. Os requisitos REQ-01 a REQ-20 são preservados, com validação aplicada na iniciativa 03. A versão 0.5 permanece recuperável no commit `e931a1bbcd599c2337e576eb4bc6ad8a8f01c53d`.

Próximo trabalho: análise e decisões da spec 02, conforme seu diagnóstico vigente. Não iniciar a ficha final nem a redação do piloto durante essa análise.

## 20. Auditoria anterior ao arquivamento — versão 0.7

**Pedido:** conferir omissões, falhas e erros antes de arquivar como concluída. **Base:** spec 0.6, plano 0.4, tasks 0.21, guia 0.3, seis modelos v0.1, sete skills/perfis v0.1, entradas e saídas E01–E07. Revisão pela mesma IA, com acesso ao histórico; não é auditoria independente nem novo piloto.

### Achados e resolução

| ID | Achado / fundamento | Correção e resultado |
| --- | --- | --- |
| ARQ-01 | E03 marcou EX-T02 bloqueada sem tentativa de execução, contrariando o modelo e a skill de tasks. O parecer inicial não detectou a falha. | Corrigida a saída para pendente, com dependência DEC-A preservada; reconferência dirigida registrada no arquivo de saídas r1.1. T01-016 e a reconciliação de T01-017 reexaminadas nesse aspecto e novamente concluídas; skill já continha a regra correta. |
| ARQ-02 | A checklist da seção 12 e decisões da seção 11 não tinham destinação individual após a transferência. Um leitor poderia interpretá-las como pendências esquecidas de 01. | Reconciliação abaixo mantém todos os itens e distingue atendimento documental de avaliação futura. Rótulos históricos explicitados; nenhum checkbox de piloto marcado como executado. |
| ARQ-03 | Linhas em branco dividiam a tabela de histórico das tasks a partir de 0.18. | Removidas as separações indevidas; conteúdo das versões preservado em tabela contínua. |
| ARQ-04 | Arquivar os três documentos muda seus caminhos e poderia romper referências internas e de entrada. | Links recalculados para o arquivo; guia, AGENTS e specs ativas apontam para os novos destinos. Modelos, skills e avaliações permanecem em seus locais de uso. |
| ARQ-05 | A spec 03 recebia os critérios por referência, mas não explicitava os dois tipos de alteração previstos na seção 15.7/15.8 da origem. | Acrescentada a exigência futura de observar alteração que preserve sentido e alteração que exija reconsiderar a especificação, sem inventar acontecimentos para demonstrá-las. |

### Destino de todas as decisões da seção 11

| Decisões de origem | Situação / evidência ou destino |
| --- | --- |
| DEC-01, DEC-02, DEC-03 | Leitor, relação relato/ensino e intensidade narrativa: spec 02, D02-02/D02-03/D02-04 e R02-01/R02-03. Preferências continuam abertas. |
| DEC-04 | Formas curta/completa entregues em `modelos/ficha-editorial.md`; escolha aplicada ao piloto em D02-10 e ficha final de 03. |
| DEC-05 | Local do texto: D02-05 em 02. Arquivos do método têm locais definidos; arquivamento desta iniciativa não decide local do piloto. |
| DEC-06 | IDs, versões e preservação definidos no guia, seção 7, e modelos de tasks/integração. Comparação real do piloto em 03. |
| DEC-07 | Piloto escolhido e preservado em 03; não executado. |
| DEC-08 | Sete skills e nove perfis construídos e conferidos; T01-008 a T01-016, com cobertura parcial de comportamento. Complementos pertinentes em 02. |
| DEC-09 | Importância e encerramento definidos no parecer, integração e guia; casos sintéticos em E06/E07. Aplicação real em 03. |
| DEC-10, DEC-11 | Variante/convenções e referências de voz: D02-04/D02-09 em 02; reconhecimento humano em 03. |
| DEC-12 | Percursos definidos no guia; seleção pertinente em D02-10 e avaliação de esforço em 03. |

### Destino integral da checklist da seção 12

| Item original | Atendimento demonstrado / trabalho restante |
| --- | --- |
| Objetivos e limites dos tipos de texto do piloto | Spec 02, D02-01 a D02-03; ainda a definir. |
| Decisões abertas que afetam o piloto | Spec 02, D02-01 a D02-10 e achados A02. |
| Harmonizar proposta com a base e o método de registro | Guia, ficha e integração distinguem IDs, estados de conteúdo e publicação; conferência documental T01-015. |
| Aplicar ficha a episódio real | Spec 03, origem T01-018; E04 é sintético e não substitui esse item. |
| Produzir/revisar rascunho factual, didático e literário | Spec 03, origem T01-019; selecionar perfis segundo o recorte, justificando dispensas. |
| Avaliar REQ-01 a REQ-20 e registrar os não exercitados | Cobertura documental nas tasks e plano; comportamento limitado a E01–E07. Avaliação aplicada herdada por 03, sem aprovação integral antecipada. |
| Ensaiar refatoração preservando sentido, fontes e voz | Complemento condicional em 02; integração real em 03. E07 preservou o texto e não demonstrou refatoração substancial. |
| Passagem entre revisores, integração e encerramento | E04→E07 exercitam cadeia breve; funcionamento em história real será examinado em 03. |
| Avaliação autoral de voz, utilidade e esforço | Spec 03, origem T01-020/PEN-03; não recebida. |
| Reduzir campos/etapas sem contribuição | Spec 03, origem T01-021, conforme esforço observado, sem cortar requisitos antes de evidência. |
| Ajustes, limites e pendências antes de 1.0 | Spec 03, origem T01-021. O arquivo concluído continua v0.7; arquivamento não o promove a método validado v1.0. |

### Parecer final

Os vinte requisitos possuem cobertura documental nas seis entregas do método, com responsabilidades de avaliação real preservadas em 03. Sete pacotes passaram novamente no validador estrutural; nomes, referências, nove perfis e limites dos exercícios foram conferidos. A falha encontrada em E03 foi corrigida sem ampliar sua evidência. Nenhum item de construção ficou sem entrega ou encaminhamento no escopo examinado.

**Apta para arquivamento como concluída**, após as correções registradas. Permanecem fora desta conclusão a avaliação de todas as modalidades, voz real, esforço autoral e piloto. Os destinos são as specs 02/03, não uma lista de melhorias opcionais.

**Histórico v0.7:** auditoria, correções e arquivamento em `spec editorial/concluida/01-sdd-editorial/`; plano v0.5 e tasks v0.22. Versões de partida preservadas em `spec editorial/historico/2026-10-14-antes-do-arquivamento/`. O acompanhamento final registra a conferência dos caminhos após a mudança.
