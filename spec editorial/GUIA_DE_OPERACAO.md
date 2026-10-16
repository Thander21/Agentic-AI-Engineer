# Guia de operação do SDD editorial

**Versão:** 0.7 — 2026-10-16 — jornada pessoal e leitura técnica independente

**Base:** [spec 01, v0.7](concluida/01-sdd-editorial/01-especificacao-sdd-editorial.md) e [plano 01, v0.5](concluida/01-sdd-editorial/01-plano-sdd-editorial.md)

**Entrega:** ENT-01 / T01-001  
**Estado:** guia do método; construção e avaliação inicial registradas nas [tasks 01](concluida/01-sdd-editorial/01-tasks-sdd-editorial.md). Preparação em 02 e piloto em 03 têm escopos próprios.

## 1. Começar pelo trabalho solicitado

Localize a iniciativa pelo [índice de organização](README.md): `backlog/` para trabalho aguardando seleção, `changes/` para análise ou execução ativa e `concluida/` para encerramento conferido. Spec, plano e tasks acompanham a pasta da iniciativa quando existirem. Atualize links ao mover, preserve IDs e evidências e não crie cópias concorrentes. A pasta não substitui os estados detalhados das tasks nem autoriza executar fases adicionais.

Identifique a entrega pedida, sua fase atual e os documentos já existentes. Uma solicitação de análise não inicia automaticamente redação, implementação ou publicação. Reutilize decisões anteriores e avance nas partes que tenham contexto suficiente.

| Situação | Ação | Resultado esperado |
| --- | --- | --- |
| Ideia ou necessidade ainda pouco definida | Analisar contexto e elaborar ou revisar a spec. | Intenção, requisitos, lacunas e decisões no documento inicial. |
| Spec suficiente para planejar | Elaborar plano separado. | Entregas, dependências, caminhos e critérios ligados à versão da spec. |
| Plano suficiente para executar | Gerar tasks. | Trabalho delimitado, com dependências e conferência previstas. |
| Tarefa disponível para execução | Produzir o artefato solicitado e conferir seu critério. | Arquivo identificado e resultado registrado nas tasks. |
| Texto a escrever ou revisar | Preparar ficha proporcional, selecionar percurso e executar os papéis pertinentes. | Rascunho ou parecer no escopo solicitado. |
| Retorno sobre material existente | Localizar a versão e avaliar o impacto. | Correção localizada ou revisão da intenção, com histórico preservado. |

Análise, especificação e revisão de consistência ficam juntas na spec. Plano e tasks são documentos separados. Os artefatos resultantes recebem revisão adequada à sua finalidade. O resumo editorial 02 é outra iniciativa, e não o plano da spec 01.

## Jornada pessoal e finalidade de cada texto

A jornada é pessoal, narrada em primeira pessoa, com humor, retórica, cotidiano e referências escolhidas pelo autor. Família, seu pet (um furão), filmes, animes, livros e outros interesses podem participar conforme os relatos forem trazidos. Esses temas já estão autorizados como direção; nomes, cenas, diálogos, emoções e acontecimentos específicos precisam de fonte autoral. Nenhum tema precisa aparecer em todo texto.

Os capítulos de estudo são o percurso técnico autônomo e formarão o livro. Devem apresentar conceitos, pré-requisitos e fontes suficientes para quem não acompanha a história pessoal. Relatos podem ser vinculados como leitura complementar; compreender a jornada não é pré-requisito para aprender o conteúdo. Posts e artigos recebem voz conforme a finalidade: história pessoal, explicação técnica ou combinação explícita das duas.

O método serve à organização pessoal do autor: rotina, pausas e escolhas reais orientam o trabalho, sem metas de exposição ou produção presumidas. Specs, planos e tasks conservam clareza e evidência em linguagem direta; não precisam imitar formalidade corporativa nem transformar cada registro em história. Na preparação e revisão, distinguir precisão técnica de formalidade da voz. A escolha autoral vigente é registrada em RA02-15 da spec 02; orientações anteriores de tom profissional para toda a jornada ficam superadas.

## 2. Contexto mínimo

Antes de produzir, identifique:

- Pedido atual, resultado esperado e limite do trabalho.
- Spec e plano pertinentes, com versões; tarefa correspondente, quando houver.
- Artefato de entrada e sua versão, se for revisão ou refatoração.
- Público, intenção, formato e destino conhecidos.
- Fontes e registros necessários, com localização dos trechos relevantes.
- Escolhas de voz e convenções aplicáveis; decisões ainda pendentes.
- Papel executado, saída esperada e critério de conferência.

Para um documento operacional, o contrato da tarefa e suas fontes podem oferecer contexto suficiente. Para um relato, acrescentar fatos confirmados, liberdade criativa e referências de voz. Amostras do autor em Markdown são suficientes; links ou propriedades do Obsidian só entram se contribuírem para a interpretação.

Selecione o contexto necessário ao trabalho, sem carregar todo o acervo. Transcrição histórica informa o que foi dito; não prova uma afirmação técnica nem representa automaticamente uma decisão vigente. Divergências entre fontes devem ser expostas antes de sustentar uma conclusão.

### Quando falta informação

Se a lacuna altera intenção, vivência ou conclusão central, formule uma pergunta específica ao autor ou registre a necessidade de pesquisa. Trabalhe nas partes independentes. Se a ausência não impedir um rascunho, mantenha uma marca editorial identificável, sem preencher a lacuna como fato.

Decisões de público, tom, formato e canal pertencem à spec da iniciativa pertinente; para a primeira publicação, consultar a síntese vigente do [resumo editorial 02](concluida/02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md). A ausência dessas escolhas não impede construir modelos genéricos, mas pode impedir redigir ou avaliar o texto concreto. Fonte inacessível, instrução ausente e preferência não definida são limitações distintas: indique qual delas afeta a entrega.

## 3. Escolher o percurso

**Percurso leve:** para entrega curta, de escopo estável e poucas fontes, usar ficha breve, rascunho, revisão pertinente, integração e leitura final. Uma pessoa ou IA pode assumir os papéis sequencialmente. Não é necessário criar um arquivo por parecer.

**Percurso completo:** para capítulo, grande reorganização, várias fontes ou decisões relevantes, usar ficha completa, esboço, revisão estrutural, pareceres especializados, integração, acabamento e prova. Explicitar por que os perfis selecionados são necessários.

O tamanho sozinho não decide: um parágrafo com afirmações técnicas delicadas pode exigir conferência factual. Dispensar um perfil requer motivo; não avaliar um aspecto deve permanecer visível. O documento operacional não precisa de arco narrativo, piadas ou metáforas de RPG.

## 4. Produzir e passar o trabalho adiante

| Passagem | Quem atua | Entrada → saída | Condição de avanço |
| --- | --- | --- | --- |
| Preparação | Preparador editorial. | Pedido e fontes → ficha com contexto e lacunas. | Há base para o escopo escolhido ou para um rascunho com pendências explícitas. |
| Estrutura | Editor de desenvolvimento ou redator. | Ficha → esboço, quando necessário. | A sequência atende à intenção e aos pré-requisitos do leitor. |
| Redação | Redator. | Ficha, esboço e fontes → rascunho identificado. | A entrega solicitada está legível e suas lacunas estão sinalizadas. |
| Revisão estrutural e integração | Editor de desenvolvimento emite parecer; editor responsável aplica as decisões. | Rascunho → achados de foco, ordem e lacunas → versão estruturalmente ajustada. | Os problemas estruturais relevantes são resolvidos antes das leituras que dependem da nova estrutura. |
| Revisões especializadas | Revisores dos perfis escolhidos. | Mesma versão estabilizada e contexto pertinente → pareceres. | Cada parecer informa seu escopo, fundamento e limites. |
| Integração | Editor responsável. | Rascunho e pareceres → nova versão e decisões. | Conflitos são resolvidos; mudanças de sentido são encaminhadas à reconferência. |
| Acabamento e integração | Editor de linha/tom e preparador linguístico emitem pareceres; editor responsável aplica as decisões. | Versão integrada → pareceres → nova versão com ajustes de fluidez e língua. | Precisão, voz e convenções foram preservadas; a prova recebe a versão resultante. |
| Prova e leitura autoral | Revisor de prova; depois autor. | Versão consolidada → conferência final e apreciação humana. | O resultado distingue texto revisado, pendências e retorno efetivamente recebido. |

Depois de mudanças estruturais, entregue aos próximos revisores a versão nova. Parecer sobre versão antiga não se aplica automaticamente à atual. A primeira leitura de cada revisor deve ocorrer sem os outros pareceres quando possível; se já estiverem no contexto, declare a limitação. Na reconferência dirigida, forneça os achados que precisam ser examinados.

Nenhum papel implica autorização para outro agente editar simultaneamente o arquivo principal. Revisores entregam pareceres; o editor responsável integra as alterações. A cadeia funciona também sem agentes separados.

## 5. Emitir pareceres úteis

Cada achado contém papel, versão, trecho, problema, motivo, critério ou fonte, sugestão, ganho esperado, possível perda e importância. Pode recomendar manter uma passagem, explicando sua função. Não existe número mínimo de mudanças.

- **Impeditivo:** compromete integridade ou intenção central; precisa ser resolvido antes de concluir a entrega afetada.
- **Revisão necessária:** prejudica compreensão ou consistência; requer correção ou justificativa explícita.
- **Sugestão:** alternativa expressiva, que pode ser recusada com motivo.

Use os perfis conforme a necessidade: estrutura; fatos/fontes; didática; continuidade; voz/tom; linha/fluidez; preparação linguística; leitura crítica; prova. Seus critérios estão na [referência de perfis](skills/editorial-revisar/references/perfis.md). A existência das instruções não comprova comportamento: consulte a cobertura de avaliação nas tasks antes do piloto.

Concordância entre IAs não comprova um fato. Ortografia correta não demonstra prazer de leitura. Uma simulação de leitor não substitui retorno humano. A avaliação de naturalidade deve apontar trechos e razões, sem tentar provar autoria por detector de IA.

## 6. Integrar e refatorar

Antes de editar, preserve uma versão recuperável. Use histórico já disponível e verificado ou uma cópia identificada por revisão; salvar por cima de um arquivo não garante recuperação. Registre o caminho da versão de partida no acompanhamento.

Para cada achado, registre acolhido, recusado com motivo ou pendente. Decida conflitos pela intenção, fontes e voz escolhida, nunca por maioria de revisores. Questões de vivência, posicionamento ou mudança de tese retornam ao autor.

Reorganizar, cortar e reescrever devem preservar fatos, ressalvas, fontes e função da passagem. Se a alteração mudar a promessa ou a interpretação, atualize a ficha ou a spec pertinente e examine o impacto no plano, nas tasks e nos textos relacionados.

Após integrar, releia o conjunto: correções locais podem quebrar transições, introduzir repetição ou apagar humor. Reconferir apenas o que a mudança afetou: conclusão alterada retorna à revisão factual; nova sequência à didática; metáfora modificada à continuidade. Uma vírgula sem efeito no sentido não exige reiniciar toda a cadeia.

## 7. Identificações e estados

Mantenha IDs existentes de sessões, episódios e publicações. Entregas sem ID anterior podem receber `TXT-001`, verificando antes os IDs já usados. A revisão `r01`, `r02` etc. identifica a versão do artefato; o número da etapa da jornada não substitui essa identificação. Specs, planos e tasks mantêm seus IDs próprios definidos no plano.

| Acompanhamento | Estados ou informações | O que não presumir |
| --- | --- | --- |
| Execução de tarefa | Pendente; em execução; produzida/aguardando conferência; concluída; bloqueada com motivo. | Arquivo produzido não equivale a tarefa concluída. |
| Maturidade do conteúdo | Nota de estudo; caso documentado; caso conferido; texto para leitura; capítulo revisado. | Nem todo texto precisa virar capítulo; o estado depende do material e de sua base. |
| Apreciação autoral | Pendente ou retorno recebido, com decisões registradas. | Ausência de resposta não significa aprovação. |
| Publicação | Não publicada ou publicação ocorrida, com destino e versão identificados. | Revisão concluída não publica o conteúdo. |

As definições de maturidade seguem a [base do livro](<../capitulos estudos/BASE_DO_LIVRO.md>). Reutilize o registro de origem por vínculo, sem duplicá-lo como uma nova experiência para cada postagem ou capítulo.

### Contrato de localização e passagem ao acervo

- `capitulos estudos/` mantém mapa, sequência de aprendizagem e capítulos; `jornada do heroi/` mantém contexto narrativo e fontes preservadas. As quinze etapas não substituem o currículo.
- `registro da autoridade/publicacoes/` guarda todos os posts e artigos criados, inclusive rascunhos e derivados de capítulos. O [índice de publicações](<../registro da autoridade/PUBLICACOES.md>) identifica a versão de trabalho e os vínculos. Fontes antigas fora da pasta podem ser inventariadas por referência; sua cópia histórica permanece identificada, sem concorrer com novas versões editoriais.
- Cada peça recebe ID, revisão, origem (`jornada`, `estudo` ou `ambas`), links às fontes/capítulos/episódios pertinentes, ficha e tarefa quando existentes. Episódio pessoal é opcional para uma explicação técnica. Artigo e chamada são peças distintas, ligadas entre si.
- A ficha, os pareceres e as revisões podem acompanhar a peça em sua pasta. Specs, planos, tasks e avaliações do método permanecem em `spec editorial/`. Um capítulo que gera um artigo conserva seu arquivo de estudo e aponta para a publicação derivada.
- Ao criar ou revisar uma peça, atualizar seu índice e registrar separadamente estado editorial, retorno autoral e publicação. Cada envio efetivo registra artefato, revisão exata, destino, data e URL; ausência de informação fica explícita. Preparar uma peça não autoriza enviá-la.
- Notas de sessão e decisões de estudo documentam experiências. Mudanças de intenção editorial voltam à spec; estratégia ao plano; execução às tasks. O método de registro não substitui preparação, redação, revisão e integração SDD.

Convenção aplicada na iniciativa 04. A conferência da nova interface é documental; as evidências históricas da v0.5 e das skills conservam seus limites. Antes do piloto, T02-005 deve considerar esta versão do guia e a ficha atualizada ao selecionar procedimentos e complementos.

## 8. Conferir e encerrar

Para concluir uma tarefa, registre: arquivo/versão, critério examinado, evidência, resultado, achados e pendências. Dependência futura mantém a tarefa pendente; impedimento encontrado durante a tentativa de execução gera bloqueio com motivo e condição de retomada.

Uma rodada editorial termina sem impeditivos abertos, com revisões necessárias resolvidas ou justificadas e uma prova referente à versão integrada. Apreciação humana ausente resulta em “pronto para leitura autoral”, nunca em aprovação presumida. Se essa apreciação integra o critério da tarefa, ela continua pendente.

Como ponto de partida, fazer uma rodada completa e outra dirigida aos achados. Se a estrutura continuar instável, voltar ao esboço ou à especificação em vez de repetir polimento indefinidamente. Esse limite não permite ignorar problemas.

Separar quatro evidências: estrutura dos arquivos; comportamento nos exercícios; uso integrado no piloto; apreciação do autor. Um validador de `SKILL.md` não comprova os três últimos. Registrar aspectos não avaliados e restrições da conferência. Reabrir as tarefas cujas evidências forem invalidadas por mudanças posteriores.

## 9. Uso inicial neste projeto

O guia, os seis modelos e as sete skills foram construídos. Confirme caminhos e versões antes de usar os recursos. As skills locais são lidas explicitamente, sem presumir descoberta automática pelo ambiente. A situação de conferência e avaliação de cada entrega permanece nas tasks.

O piloto permanece **01 — Novo mundo, bagagem antiga**, sob a [spec 03](backlog/03-piloto-editorial/03-piloto-editorial.md). A [spec 02](concluida/02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md) reúne análise de história/contexto, voz/tom e adequação das skills, além das condições de uso. Antes do piloto, receber sua preparação suficiente, confirmar fatos pessoais relevantes, complementar modos necessários ainda não exercitados e preservar o original. Os exercícios usam material separado e não antecipam a reescrita do piloto.

Para continuar, consultar o acompanhamento da iniciativa pertinente. Se ainda não houver plano/tasks, seguir o parecer e a próxima ação da própria spec. As tasks 01 conservam as evidências e os IDs transferidos; não obrigam a executar o piloto para encerrar a construção do método. Não manter neste guia uma segunda lista de progresso nem inventar preferências de público, canal ou voz.

## 10. Histórico

| Versão | Alteração |
| --- | --- |
| 0.1 | Guia inicial, produzido antes dos modelos e skills. |
| 0.2 | T01-015: papéis de parecer e aplicação explicitados nas passagens estrutural e de acabamento; referência aos perfis existentes e retirada de instruções de progresso desatualizadas. |
| 0.3 | Separação autorizada: método em 01, preparação em 02 e piloto em 03. Atualizada a orientação de retomada; contratos editoriais e limites de evidência preservados. |
| 0.4 | Referências de 01 atualizadas para o arquivo de concluídos; guia e recursos operacionais permanecem ativos. |
| 0.5 | Convenção backlog → changes → concluida documentada no índice; referências de 02/03 atualizadas. Avaliações preservadas como evidência, sem alteração dos contratos editoriais. |
| 0.6 | 2026-10-16: contrato de responsabilidades, origem dupla e passagem ao acervo; decisões da primeira publicação remetem à síntese vigente de 02. Conferência documental na iniciativa 04. |
