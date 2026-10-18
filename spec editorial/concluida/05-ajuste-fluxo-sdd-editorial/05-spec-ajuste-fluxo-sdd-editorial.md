# Spec 05 — Ajuste do fluxo e da documentação SDD editorial

**ID:** SPEC-EDITORIAL-005  
**Versão:** 0.7 — 2026-10-17 — implementação e conferência documental concluídas  
**Estado:** concluída no escopo da correção documental, após seleção e implementação autorizadas. [Plano v0.1](05-plano-ajuste-fluxo-sdd-editorial.md), [tasks v0.2](05-tasks-ajuste-fluxo-sdd-editorial.md) e encerramento na seção 9. D05-01/02 e requisitos preservados; avaliação editorial em uso permanece no piloto 03.  
**Origem:** análise de 16/10/2026 e pedido do autor de gerar o backlog antes de retomar o piloto 03.

## 1. Problema e resultado esperado

O método oferece fontes, papéis e critérios úteis, mas seu uso gerou documentação excessiva, repetição de acompanhamento, estados divergentes e manutenção do próprio método dentro do piloto. As retiradas de etapas, episódios e sessões reduziram arquivos, porém parte do diário administrativo foi transferida às tasks. Corrigir apenas a localização não resolveu a forma de trabalhar.

Objetivo: tornar o fluxo `spec → plano → tasks → artefatos` proporcional, com documentação suficiente para uma IA localizar o trabalho, compreender o escopo e executar até a condição de parada adequada, sem reconstruir toda a história do repositório.

O público desta entrega é o autor e as IAs que trabalham no projeto. Não é conteúdo público. Esta iniciativa deve refazer as orientações e interfaces necessárias para coordenar a sequência editorial da seção 4.4, além de eliminar a burocracia e as divergências identificadas. A 03 continua responsável pelo texto e pela avaliação editorial do piloto. O SDD organiza a iniciativa; as skills conduzem a produção do texto dentro dela. Não criar nova spec/plano/tasks para cada peça pequena ou para cada etapa de escrita.

## 2. Evidências e base de entrada

| Fonte examinada no levantamento | Problema observado / uso nesta iniciativa |
| --- | --- |
| [Spec 03 v0.9](../../changes/03-piloto-editorial/03-piloto-editorial.md) | Cabeçalho registra produção, enquanto seções mantêm “plano futuro”, estados de origem e prontidão anterior. Distinguir histórico e orientação atual. |
| [Plano 03 v0.3](../../changes/03-piloto-editorial/03-plano-piloto-editorial.md) e [tasks 03](../../changes/03-piloto-editorial/03-tasks-piloto-editorial.md) | T03-007/008 são manutenção do método incorporada ao piloto; acompanhamento disperso e registros longos. Preservar origem e resultado ao separar responsabilidades. |
| [Ficha FIC03-001 r01](<../../../registro da autoridade/publicacoes/01-novo-mundo-bagagem-antiga/ficha-editorial.md>) | Ficha extensa, com procedimentos repetidos e estado de entrada que pode ser confundido com situação atual. |
| [Guia v0.9](../../GUIA_DE_OPERACAO.md), [AGENTS](../../../AGENTS.md), [modelos](../../modelos) e [skills](../../skills) | Conferir hierarquia, leitura mínima, seleção de percurso e repetição de regras. Não presumir que todos os recursos devam ser lidos em cada tarefa. |
| [Spec 01](../../concluida/01-sdd-editorial/01-especificacao-sdd-editorial.md) e [tasks 01](../../concluida/01-sdd-editorial/01-tasks-sdd-editorial.md) | Base do método e limites das avaliações anteriores; identificar somente os aspectos afetados pela correção. |
| [Spec 04](../../concluida/04-alinhamento-editorial/04-spec-alinhamento-editorial.md) | Responsabilidades de localização já definidas; atualizar somente interfaces que precisarem refletir a simplificação. |

Na análise anterior, spec/plano/tasks de 03 somavam aproximadamente 5.880 palavras, ficha 2.221 e corpo do artigo 709. Isso é evidência contextual de custo documental, não um limite obrigatório de tamanho nem prova isolada de falha. Conferir o estado real ao selecionar esta iniciativa, pois os arquivos podem evoluir.

## 3. Escopo e requisitos de correção

| ID | Correção necessária | Critério de aceitação |
| --- | --- | --- |
| R05-01 | Definir a função e autoridade de cada documento. | Spec decide intenção/requisitos; plano organiza entregas; tasks concentram execução; artefato contém texto/conhecimento. README navega, guia descreve o procedimento vigente, skills executam os papéis e modelos fornecem campos proporcionais. Estado atual tem um responsável único; história e proposta não prevalecem como orientação vigente. Aplicar o contrato da seção 4.1. |
| R05-02 | Reduzir preenchimento e registros repetitivos. | Cada campo mantido serve a uma decisão, execução ou conferência. O acompanhamento reúne ID, estado, resultado/versão, evidência suficiente e pendência/próxima ação; explicação adicional só quando necessária. Não manter diário de arquivos alterados, relatórios de cada rodada, nove justificativas de dispensa ou campos sem aplicação. Fontes e decisões únicas permanecem localizáveis. |
| R05-03 | Definir entrada mínima por iniciativa e peça. | Retomada identifica pedido/limite autorizado, fase, tarefa quando houver, artefato/revisão, decisões pertinentes, fontes selecionadas e pendência/próxima ação. Preparação avalia o próximo conteúdo pelo pedido, material disponível, pendências e ponto da jornada/estudo, sem seguir a numeração automaticamente. Leitura começa no acompanhamento atual e na peça/ficha; guia e skill da fase são consultados explicitamente conforme AGENTS, sem carregar todos os modelos ou avaliações. Separar direção geral do projeto de escolhas particulares da peça; 02 é entrada do piloto, não configuração universal de futuras publicações. |
| R05-04 | Tornar percurso e revisão proporcionais sem perder o mínimo editorial. | Conferir fidelidade à intenção, fatos/fontes e ressalvas relevantes, coerência e legibilidade. Ficha breve atende escopo estável; esboço/ficha completa se justificam por estrutura, múltiplas fontes ou decisões complexas. Selecionar perfis adicionais para questões presentes, sem exigir os nove nem justificar nove dispensas. No capítulo, incluir pré-requisitos e suficiência didática; no relato, respeitar vivências e direção de voz; na chamada, fidelidade à peça de origem. Manter produção, conferência e apreciação autoral distintas. |
| R05-05 | Definir fases, alcance de “continue” e condições de parada. | Refinar/analisar no backlog não seleciona nem implementa. Seleção para trabalho ativo move a mesma pasta para changes e autoriza somente a fase pedida. “Continue” retoma o escopo já autorizado até sua entrega ou dependência real, sem parada mecânica por task e sem iniciar fase não pedida. Decisão/fato essencial, preservação pendente e retorno autoral interrompem somente a parte dependente; publicação exige instrução explícita. Aplicar seção 4.2. |
| R05-06 | Separar correção do método e produção, com tratamento claro de conclusões anteriores. | 05 executa a correção e 03 recebe impactos/dependências. T03-007/008 conservam origem/resultados como ocorridos, sem transferir conclusão para uma execução fictícia em 05. Evolução de procedimento registra vínculo de substituição nos pontos pertinentes de 01/04, preservando o escopo histórico. Se um defeito invalidar aceitação anterior, registrar evidência e aspecto, reabrir a iniciativa e aplicar a movimentação prevista; o alcance da reconferência fica limitado ao afetado. Correção de navegação não reabre conteúdo. |
| R05-07 | Reconciliar estado atual e localização de 03 e suas peças. | Uma tabela atual inclui todos os IDs de 03 e seus estados; registros antigos ficam identificados como históricos ou são retirados quando apenas repetem mudanças disponíveis no Git. Spec/ficha/índice apontam para o acompanhamento vigente e a peça exata, sem próximos passos concorrentes. Revisão de metadados não aprova nem reescreve PUB-001; preservar conteúdo único e decisões já tomadas. |
| R05-08 | Preservar pelo Git textos de publicações, jornada e capítulos de estudo, conforme D05-01. | Sempre que uma alteração exigir preservar uma versão desses textos, conferir se ela está recuperável no Git; se não estiver, solicitar o commit do autor e aguardar antes da alteração dependente. A necessidade de preservação não se limita a comparações. Partes independentes continuam. Sem commit do conjunto inteiro por rotina, cópias paralelas ou commits/pushes automáticos. |
| R05-09 | Separar conferência operacional em 05 de avaliação editorial no piloto. | Em 05, percorrer as entradas e saídas documentais da seção 5.1 com material existente, observando informação ausente, perguntas repetidas e registro redundante, sem alegar eficácia geral. Voz reconhecida, prazer de leitura, utilidade real dos pareceres e esforço autoral continuam em 03 após sua retomada. O fechamento de 05 não depende da apreciação humana do piloto, nem declara essa apreciação realizada. Não inventar tempo ou satisfação. |
| R05-10 | Reconciliar orientação vigente e estabelecer a liberação da 03. | Plano mapeia R05-01–12 a entregas, documentos afetados e evidências proporcionais. AGENTS, README, guia, skills/modelos afetados e entrada de 03 respeitam os contratos 4.1/4.2 e a adaptação 4.3. README e guia devem explicar os dois fluxos e remeter à mesma sequência 4.4. Não restam instruções ativas conflitantes, recriação das camadas retiradas, importação do motor de software ou leitura indiscriminada. Liberação exige implementação conferida, percurso 5.1 e pendências individualizadas conforme 5.2; não ocorre pela aprovação desta spec. |
| R05-11 | Fixar a sequência editorial e seus retornos. | Orientações, plano/tasks e skills seguem 4.4: preparar → estruturar quando necessário → redigir → revisar → integrar → reconferir → leitura autoral → ajustes se houver → prova final. Estrutura/fatos/sentido antecedem acabamento; prova final examina a versão posterior ao retorno e aos ajustes. Etapas cumpridas são reconhecidas por evidência, não repetidas por rotina. Texto sem retorno fica pronto para leitura autoral, sem aprovação ou fechamento humano presumidos. Publicação é separada. |
| R05-12 | Coordenar as skills com contexto e limites por etapa. | Para cada etapa, definir entrada mínima, modo/skill, ação permitida, saída identificada, condição de avanço e retorno quando houver lacuna. O plano coordena entregas/dependências; tasks mantêm fase, versão e próxima ação atuais; skills executam seus papéis. Não exigir contexto do acervo inteiro, nova skill por etapa ou delegação automática. Aplicar 4.5 e conferir V05-07/08. |

## 4. Limites e preservações

- Manter os IDs existentes, fontes autorais e transcrições. Simplificar orientação não autoriza eliminar fontes ou resultados únicos.
- Preservar FIC03-001, ESB03-001 e PUB-001 r01, suas decisões de leitor, voz, canais e exposição. Corrigir metadados/localização não equivale a revisar ou aprovar a prosa.
- Manter jornada como relato/contexto, estudos como formação e capítulos, publicações como acervo das peças. Não recriar as camadas retiradas.
- Git registra versões; GitHub é remoto quando sincronizado, sem presumir existência de push. Não criar diário de saves, cópia manual, manifesto de preservação ou outro relatório para duplicar estas correções.
- Não introduzir código, infraestrutura ou suíte de software. Usar leitura documental, conferência de referências e percurso dirigido sobre material existente.
- A publicação e a apreciação autoral do piloto não são entregas desta iniciativa. As evidências sintéticas de 01/02 conservam seus limites; não repetir todas as avaliações para demonstrar correções pontuais.

### 4.1. Contrato documental e resolução de divergência

Instruções explícitas do autor delimitam o trabalho e prevalecem sobre orientações locais, respeitadas as regras do ambiente. Uma proposta não vira regra por ser mais recente. AGENTS contém invariantes e roteamento; guia, o procedimento editorial vigente; spec da iniciativa, intenção/requisitos e decisões aplicáveis à entrega; plano, a estratégia; tasks, o progresso e a evidência; peça/ficha, seu conteúdo e contexto particular. README aponta para essas fontes, sem manter outro acompanhamento detalhado.

Registros encerrados explicam a decisão e a evidência de sua época; não impõem um próximo passo antigo. Regras duráveis que precisem sobreviver ao fechamento devem estar nas orientações vigentes, vinculadas à decisão, sem obrigar ler todas as iniciativas concluídas. Se duas instruções vigentes divergirem no aspecto necessário à tarefa, identificar o conflito e sua decisão mais recente efetivamente aceita; não escolher pela quantidade de documentos ou fabricar preferência do autor.

### 4.2. Contrato de fase e passagem entre agentes/papéis

| Situação | Entrada suficiente e saída esperada | Limite |
| --- | --- | --- |
| Refinamento no backlog | Pedido e fontes pertinentes → spec com requisitos, lacunas e parecer. | Não mover ou implementar automaticamente; fase adotada no refinamento anterior. |
| Seleção/planejamento | Escolha explícita de trabalhar a iniciativa e spec suficiente → mesma pasta em changes, plano e decomposição quando pedidos. | Localização não concede autorização para fases adicionais. |
| Execução editorial | Escopo autorizado, task disponível e contexto mínimo → artefato e conferência pertinente registrados uma vez nas tasks. | Pode seguir tasks dependentes dentro da entrega autorizada; não exigir novo “continue” por arquivo. |
| Dependência real | Identificar fato/decisão ausente, versão a preservar ou retorno necessário → pergunta específica e condição de retomada. | Continuar partes independentes; não inventar conteúdo nem bloquear atividades sem dependência. |
| Encerramento | Critérios da entrega atendidos, evidências e pendências com destino → situação e próxima ação inequívocas. | Só liberar produção da 03 conforme 5.2; publicação continua separada. |

As passagens usam versões e fontes identificadas. Uma mesma IA pode executar papéis sequenciais, declarando acesso ao histórico sem alegar independência. Mudar de papel não cria autorização para editar texto, delegar ou publicar além do pedido.

### 4.3. Contrato de adaptação SDD ao editorial

Adotar da referência SDD a conferência do estado real, distinção entre proposta e decisão, recorte, rastreabilidade e mudança de intenção explícita. Manter os três documentos editoriais e as áreas de conteúdo existentes. Não instalar ou executar o kit, trocar a estrutura por `change.md`, exigir motor, hooks, `.sdd`, `evidence.jsonl`, RED/GREEN, frases rígidas de aprovação ou verificador independente obrigatório. A referência de software não governa o trabalho editorial.

Ajustar as skills locais pertinentes antes de propor nova skill. Esta iniciativa não inclui criar ou instalar uma skill genérica de engenharia agêntica. Contratos de contexto, papéis, autorização, evidência e parada são a personalização necessária; não exigem infraestrutura de software.

### 4.4. Sequência editorial acordada — D05-02

**Decisão autoral — 17/10/2026:** o autor aprovou o entendimento discutido e pediu ajustar a spec 05 para manter essa sequência e coordenar as skills. Publicações, relatos da jornada e capítulos usam o mesmo encadeamento, com profundidade adequada à finalidade. A preparação pode receber um conteúdo já escolhido pelo autor; nesse caso, não escolhe outro por iniciativa própria.

**Preparar → estruturar quando necessário → redigir → revisar → integrar → reconferir → leitura autoral → ajustes, se houver → prova final.**

| Etapa | Responsabilidade e saída | Skill/papel e condição de avanço |
| --- | --- | --- |
| Preparar | Avaliar qual conteúdo vem a seguir e sua relação com jornada ou estudo, usando intenção do autor, fontes, material disponível e pendências. Definir leitor, contribuição, natureza (história, técnica ou combinação), tom, formato, limites e fontes em ficha proporcional. | `editorial-preparar`. Avançar com base suficiente ou lacunas delimitadas compatíveis com rascunho; fato ou escolha essencial ausente retorna ao autor/fonte. Não forçar vínculo pessoal a estudo técnico. |
| Estruturar, quando necessário | Organizar como apresentar o conteúdo: abertura, progressão, explicações/cenas confirmadas e fechamento, conforme natureza/tom recebidos. Produzir esboço; não reabrir preferências já resolvidas. | `editorial-redigir`, modo esboço. Escopo breve/estável pode seguir sem esboço separado, com a sequência compreensível no próprio rascunho. Não inventar acontecimentos para preencher estrutura. |
| Redigir | Transformar ficha, fontes e esboço quando existente em rascunho identificado. Fazer leitura de entrega, sem chamá-la de revisão especializada ou prova final. | `editorial-redigir`, modo redação. Entregar versão legível e lacunas explícitas dentro do escopo; mudança de intenção volta à spec/ficha antes de virar decisão. |
| Revisar | Examinar foco, estrutura, fatos e sentido antes do acabamento; didática, continuidade e voz conforme a peça; depois fluidez/língua. Produzir achados e preservações fundamentados, sem exigir um arquivo por perfil. | `editorial-revisar`, perfis pertinentes. Parecer não altera silenciosamente o texto; lacunas limitam as conclusões. Mudança estrutural relevante precisa ser integrada antes das leituras que dependem dela. |
| Integrar | Decidir acolher, recusar com motivo ou manter pendente cada achado relevante e aplicar as alterações autorizadas, preservando sentido, fontes e voz. | `editorial-integrar`. Nova versão e decisões localizáveis; conflito de intenção/vivência volta ao autor. Preservação de texto segue D05-01 antes da edição dependente. |
| Reconferir | Examinar os aspectos alterados, a resolução dos achados e efeitos colaterais. Não reutilizar parecer de uma versão anterior como conferência da nova. | `editorial-revisar`, perfis afetados. Voltar à integração se persistir problema; entregar versão identificada para leitura autoral quando os critérios pertinentes forem atendidos. |
| Leitura autoral | O autor avalia voz, sentido, clareza, exposição e experiência de leitura. A IA registra o retorno real e esclarece dúvidas sem respondê-las pelo autor. | Autor, com apoio da IA. Ausência de retorno mantém a peça pronta para leitura autoral; não presumir aprovação, prazer de leitura ou encerramento da tarefa dependente. |
| Ajustes, se houver | Aplicar decisões do autor e reconferir os aspectos afetados; se não houver ajustes, passar à prova. | `editorial-integrar` e `editorial-revisar`. Se uma alteração mudar intenção, fato ou exposição além do retorno recebido, esclarecer e retornar ao ponto afetado; não impor rodada completa por correção local. |
| Prova final | Conferir língua, títulos, links, resíduos e integridade da versão resultante da leitura e dos ajustes. Não iniciar reescrita substancial na prova. | `editorial-revisar`, P09. Resíduo local é corrigido e reconferido; problema de sentido/estrutura retorna à etapa responsável e invalida a prova no aspecto afetado. Prova não publica o texto. |

As etapas têm função e ordem, sem exigir arquivo separado ou nova autorização a cada passagem dentro do escopo já autorizado. Podem ocorrer na mesma sessão, com papéis explícitos. Revisão/integração podem iterar por estrutura antes do acabamento; isso não autoriza saltar a reconferência da versão entregue. Uma conferência técnica antes da leitura autoral pode retirar resíduos, mas não substitui a prova final posterior.

O fluxo SDD é a organização externa: pedido/escopo → análise/fontes → esclarecimentos essenciais → spec revisada → plano conferido → tasks conferidas → análise de consistência entre os três → execução/conferência → encerramento. Dentro da execução de uma peça ocorre a sequência acima, e o retorno autoral integra seu critério quando previsto. Análise pré-execução é conferência entre documentos existentes, não outro arquivo obrigatório.

### 4.5. Coordenação das skills e passagem de contexto

Cada etapa recebe apenas o necessário: objetivo e limite autorizado; natureza/leitor/tom e demais decisões pertinentes; ficha vigente quando houver; artefato e revisão exatos; fontes selecionadas; lacunas/achados a tratar; saída esperada e condição de passagem. Receber esse contexto não obriga reler todos os documentos de origem. A skill consulta fonte adicional quando uma questão concreta exigir.

O plano define quais entregas e passagens compõem o trabalho; as tasks identificam etapa atual, peça/revisão, dependência e próxima ação; a skill aplica o procedimento de seu papel. Não criar um coordenador, log de passagem ou uma coleção de skills novos por rotina. Reutilizar preparar/redigir/revisar/integrar; especificar/planejar/tarefas organizam a iniciativa e não escrevem automaticamente as peças.

A saída informa artefato/revisão, resultado, critério conferido e pendência/próxima etapa no acompanhamento pertinente, sem repetir toda a ficha ou fontes. Uma lacuna factual volta à preparação/fonte; problema de estrutura ao esboço/redação; achado não resolvido à integração; intenção alterada à spec/ficha e ao autor quando necessário. Parecer é entrega do revisor, alteração é responsabilidade do integrador. Nenhuma passagem autoriza inventar fato, reconhecer voz em nome do autor ou publicar.

## 5. Estratégia proposta para o futuro plano

Primeiro, conferir responsabilidades e a sequência 4.4/coordenação 4.5; depois, refazer guia/roteamento e simplificar modelos/skills afetados para essas passagens; em seguida, reconciliar o acompanhamento de 03 sem reiniciar etapas sustentadas por evidência. Por fim, percorrer a retomada usando os arquivos reais existentes e registrar somente o resultado necessário nas futuras tasks 05.

Esta proposta ainda não é plano de execução. Não criar plano/tasks vazios, novos exemplos de escrita ou um relatório por achado. Quando a iniciativa for selecionada, o plano definirá entregas proporcionais e cobertura R05-01–12.

### 5.1. Percurso dirigido a conferir na implementação

| Caso | Situação de entrada | Resultado observável esperado |
| --- | --- | --- |
| V05-01 | Pedido de analisar um backlog, como este. | Localizar o pedido e registrar análise na spec sem mover a pasta, implementar ou iniciar outra fase. |
| V05-02 | Retomar T03-003 com os arquivos existentes. | Localizar estado, espera por 05, PUB-001/ficha e decisões específicas; montar a entrada necessária sem percorrer as quinze etapas. A conferência não redige a chamada nem antecipa sua task. |
| V05-03 | Definir a preparação de outra peça a partir das regras e modelos atuais. | Separar direção geral e decisões daquela peça; não herdar leitor/canal do piloto nem criar uma spec, sessão ou episódio apenas por rotina. Identificar lacuna essencial se houver. Não criar a peça. |
| V05-04 | Mudança pontual versus revisão de estrutura. | Identificar a conferência mínima e justificar apenas aprofundamentos necessários; não acionar todos os perfis para uma correção local nem omitir fatos/ressalvas por simplificação. |
| V05-05 | Necessidade de preservar publicação, jornada ou capítulo de estudo. | Verificar se a versão está recuperável no Git; se faltar, solicitar commit do autor e aguardar a alteração dependente, conforme D05-01. Se o caso não ocorrer, conferir a instrução como tal e marcar comportamento ainda não exercitado; não fabricar sobrescrita ou pedido de commit para testar. |
| V05-06 | Evolução de regra ou defeito em conclusão encerrada. | Identificar documento responsável e distinguir substituição de procedimento de reabertura de aceitação invalidada, com destino do impacto e sem duplicar execução histórica. |
| V05-07 | Percorrer a sequência de uma história, texto técnico ou peça mista nos documentos e interfaces das skills. | Identificar escolha/ficha na preparação, esboço condicional, rascunho, revisão, integração, reconferência, leitura humana, ajustes condicionais e prova final nessa ordem. Diferenciar tom/natureza recebidos de estrutura e reconhecer etapa já cumprida sem reiniciá-la. Não escrever nova peça nem simular leitura autoral. |
| V05-08 | Conferir a passagem entre as skills, incluindo lacuna e alteração posterior ao parecer. | Cada etapa identifica entrada/versão, ação, saída e limite; revisão não edita o original, integração não presume retorno humano e reconferência lê a versão nova. Fonte ausente ou mudança de intenção tem destino explícito; ajustes autorais levam à reconferência/prova da versão resultante. Não criar log intermediário. |

Estes casos são critérios de conferência, não exercícios já executados. Usar as fontes existentes e registrar nas futuras tasks somente o necessário: observado/não exercitado, evidência, limite e destino. Conferência de links auxilia a navegação, mas não substitui a leitura dos contratos. Não exigir execução de todos os modos das skills nem inventar retorno humano para fechar 05.

### 5.2. Condição de liberação da 03

Liberar a retomada somente depois de implementar e conferir R05-01–12 nos documentos afetados, resolver divergências operacionais impeditivas e concluir o percurso dirigido no alcance que os casos reais permitirem, incluindo a sequência 4.4 e a coordenação 4.5. Toda cobertura não exercitada recebe destino e condição de retomada; um impeditivo não pode ser transferido apenas para encerrar 05. O acompanhamento deve permitir retomar T03-003 sem reconstruir decisões, e a dependência de 05 deve ser atualizada na entrada de 03.

A eficácia editorial completa e a apreciação autoral continuam no piloto. Uma limitação dessas avaliações não cria dependência circular nem impede fechar a correção documental de 05; tampouco permite declarar voz, prazer de leitura ou utilidade demonstrados antes do uso real.

## 6. Dependências, pendências e relação com a 03

**Retomada da 03:** aguarda a correção e conferência do fluxo nesta iniciativa. Isso é dependência editorial definida pelo autor, não tentativa de produção bloqueada nem cancelamento do piloto. O material produzido permanece onde está; T03-003 é a próxima tarefa de produção prevista após a liberação; conferir seu enquadramento na sequência 4.4. Ficha/esboço/artigo já produzidos são entradas aproveitáveis, não etapas automaticamente aprovadas ou trabalho a refazer por rotina. Não mover 03 de pasta ou reiniciar suas tarefas nesta abertura de backlog.

**01 e 04:** permanecem bases históricas até que se identifique aceitação anterior invalidada. Evolução de procedimento é implementada e conferida em 05, com vínculo nos pontos de origem pertinentes. Reabertura efetiva, se necessária, identifica a evidência invalidada e segue a movimentação definida, limitando o trabalho ao aspecto afetado. Não duplicar a execução de 05 nem apagar as evidências originais.

**Preservação real:** antes de alterar publicação, jornada ou capítulo cuja versão deva ser preservada, aplicar D05-01/R05-08. A regra não se limita a comparações formais. O estado local não commitado não foi resolvido pelo refinamento desta spec; não executar commit ou push automaticamente.

**Questões para o planejamento:** escolher o formato mínimo de acompanhamento e a profundidade dos ajustes às skills/modelos. A rotina de preservação foi definida pelo autor em D05-01, na seção 8; não perguntar novamente. As demais escolhas operacionais serão propostas e conferidas sem reabrir preferências autorais já recebidas.

## 7. Revisão da abertura — histórico v0.1

**Versão examinada:** v0.1, em 17/10/2026, pela mesma IA que participou da análise e das alterações anteriores, com acesso ao histórico. Sem revisão independente.

**Parecer:** apta para planejamento quando selecionada para `changes/`. Objetivo, dez correções avaliáveis, limites e dependência da 03 definidos; não há lacuna essencial que impeça organizar o plano. Isso não declara correções executadas nem método validado.

**Próximo passo:** selecionar a iniciativa 05, movê-la para `changes/` com seus links e elaborar plano/tasks proporcionais. Continuar o piloto somente após a reconciliação e conferência previstas em R05-10. O pedido atual autoriza o registro do backlog, sem executar as correções.

**Histórico v0.1 — 17/10/2026:** backlog criado a partir da análise e do pedido do autor. Nenhuma correção marcada como concluída; arquivos existentes e alterações em andamento preservados.

**Conferência da abertura:** R05-01–10 sem duplicação; 36 links locais examinados nesta spec, índice e acompanhamento 03, sem destinos ausentes. Whitespace da spec nova e diff dos documentos de navegação conferidos. Nenhum plano/tasks antecipado, commit ou alteração de staging; ficha e prosa do piloto preservadas.

## 8. Análises e consolidação antes da implementação — v0.2–v0.6

**Escopo do refinamento v0.2:** analisar e refinar esta especificação no backlog, confrontando README, guia e SDD adaptado ao editorial. Registrar achados aqui não implementa as correções. A localização foi mantida conforme pedido explícito, sem mover a iniciativa ou iniciar plano/tasks.

**Referências consultadas:** skill local `sdd-editorial-especificar` v0.1, AGENTS, README e guia v0.9, interfaces das skills preparar/planejar/tarefas, acompanhamento 03 e fonte local do SpecSimpleKit, versão declarada 0.1.0. Não foi encontrada skill genérica de engenharia agêntica nos catálogos locais examinados. A análise usa seus aspectos pertinentes — contexto suficiente, contratos de passagem, autorização, rastreabilidade e evidência — sem alegar uso de uma skill inexistente.

Do kit foram consultados o [ponto de entrada](<../../../ferramentas de estudo/SDD-TDDkit/AGENTS.md>), o [refinamento de backlog](<../../../ferramentas de estudo/SDD-TDDkit/SpecSimpleKit/kernel/.agents/skills/backlog-refinement/SKILL.md>) e o [fluxo SDD fonte](<../../../ferramentas de estudo/SDD-TDDkit/SpecSimpleKit/kernel/.agents/rules/sdd-fluxo.md>). São referências comparativas de software; suas instruções não foram ativadas como regras deste repositório, conforme AGENTS editorial. Nenhum script, instalador ou motor do kit foi executado; nenhuma alteração feita no kit.

### O que já está bem definido

README distingue localização e fase, preserva IDs e centraliza a navegação. Guia distingue preparação, autoria, revisão, integração e apreciação; proíbe inventar vivências e não confunde publicação com texto revisado. R05-01–10 preservam essas responsabilidades e o material já produzido. O defeito principal não é ausência do método, mas falta de contratos operacionais claros entre suas partes e excesso de informação concorrente.

### Achados da v0.2 e destino na especificação consolidada

| ID / situação na v0.6 | Evidência e gap identificado na v0.2 | Incorporação na spec; aplicação ainda pendente |
| --- | --- | --- |
| A05-01 — incorporado à especificação | O kit usa `change.md` com plano interno, motor e RED/GREEN; o editorial usa spec/plano/tasks separados e conferência de texto. R05-10 não explicita esse limite de adaptação. | R05-10 e contrato 4.3 definem a adaptação e os mecanismos de software excluídos. |
| A05-02 — incorporado à especificação | README, tabela de passagem, exige mover para changes ao selecionar análise; guia seção 1 repete essa orientação, mas ambos admitem análise na organização e o autor pediu análise no backlog. A fase não tem transição suficientemente explícita. | R05-05 e contrato 4.2 distinguem refinamento, seleção e autorização da fase. |
| A05-03 — incorporado à especificação | README determina devolver uma iniciativa reaberta a changes. Seção 6 desta spec fala em rever/reabrir apenas o aspecto de 01/04, mantendo-as concluídas, sem distinguir revisão histórica de reabertura efetiva. | R05-06 e seção 6 distinguem substituição de procedimento e reabertura efetiva. |
| A05-04 — incorporado à especificação | README combina tabela atual com blocos datados ainda escritos como próximo passo. Guia manda considerar T02-005 antes do piloto, embora 02 esteja encerrada; suas instruções genéricas de IDs ainda citam sessões como se fossem camada ativa. R05-07 cobre principalmente 03. | R05-01/02/03/07/10 e contrato 4.1 delimitam instrução vigente, histórico e estado atual. |
| A05-05 — incorporado à especificação | A skill preparar aponta diretamente ao resumo 02 para decisões vigentes. Essa referência é válida para o piloto, mas não define como outra peça recebe seu contexto sem herdar leitor/canal/decisões específicos de 02. | R05-03 e V05-03 separam contexto geral, da iniciativa e da peça, sem universalizar 02. |
| A05-06 — incorporado à especificação | R05-04 pede reduzir perfis, mas não define o mínimo de conferência; o guia seção 3 exige justificar a dispensa de perfil, o que incentiva tratar todos como padrão. | R05-04 e V05-04 definem mínimo editorial e seleção de aprofundamentos. |
| A05-07 — incorporado à especificação | Na v0.2, R05-08 não definia como preservar versões sem commits automáticos ou cópias. | D05-01/R05-08 e V05-05 incorporam a decisão autoral de solicitar commit quando necessário preservar texto. |
| A05-08 — incorporado à especificação | R05-09 inclui voz, clareza e uso do método; seção 4 exclui a apreciação do piloto, e 03 aguarda o fechamento de 05. Sem separar as evidências, pode haver dependência circular de validação. | R05-09 e 5.2 separam conferência documental de 05 e apreciação do piloto, sem dependência circular. |
| A05-09 — incorporado à especificação | R05-10 exige reconciliação, mas não identifica os contratos que precisam mudar nem uma condição suficiente de liberação. Uma busca de links, isoladamente, não detectou as divergências acima. | R05-10 e 5.1/5.2 definem rastreabilidade no plano e condição suficiente de liberação. |
| A05-10 — incorporado à especificação | A v0.5 separava fases de gestão, mas não fixava integralmente a sequência de produção agora aprovada, em especial leitura autoral, ajustes e prova final posterior. | D05-02, R05-11 e 4.4 estabelecem a sequência e os retornos; V05-07 deve conferir seu alinhamento nas orientações. |
| A05-11 — incorporado à especificação | A v0.5 identificava papéis/contexto de forma genérica, sem contrato por etapa que coordenasse o que cada skill recebe, faz e entrega. | R05-12, 4.4/4.5 e V05-08 definem interfaces e coordenação no plano/tasks, sem nova camada de logs ou agentes. |

Os onze encaminhamentos estão consolidados em R05-01–12 e nas seções 4.1–5.2, incluindo a sequência e coordenação acordadas em D05-02. Estão resolvidos no nível da especificação, sem declarar as correções implementadas ou validadas em uso. A autoria das escolhas operacionais é da IA responsável, justificada pelas decisões do autor e pelas fontes identificadas; D05-01 permanece decisão literal do autor.

### Questão ao autor e parecer atual

**Q05-01 — resolvida em 17/10/2026 / D05-01:** o autor escolheu a primeira opção e esclareceu: “solicitar o commit sempre que precisar preservar texto de publicação, jornada ou capitus estudos”. Aplica-se a publicações, jornada e capítulos de estudo, sempre que for necessário preservar uma versão antes de alterá-la, não somente quando houver comparação formal. Conferir se essa versão já está recuperável no Git; caso não esteja, solicitar o commit do autor e aguardar antes da alteração dependente. Partes independentes continuam. Não exigir commit de todo o conjunto como rotina. Não há autorização de commit/push automático nem de cópias paralelas. R05-08 recebeu a decisão; A05-07 está resolvido na especificação, com aplicação ainda pendente.

**Parecer de especificação v0.6 — anterior à implementação:** apta para planejamento. A reanálise identificou duas lacunas específicas da sequência discutida, agora incorporadas como A05-10/11, R05-11/12 e contratos 4.4/4.5. Os nove achados anteriores mantêm destino, D05-01 está preservada e D05-02 registra o entendimento aprovado. Não há dúvida essencial aberta no escopo examinado. Isso não declara o fluxo implementado: ainda faltam plano/tasks, ajustes dos arquivos e conferência de suas interfaces.

**Necessidade de análise adicional:** não é necessária outra análise geral antes do plano. O planejamento deverá mapear os doze requisitos a entregas/documentos e garantir que nenhuma etapa ou passagem 4.4/4.5 fique sem responsável ou critério. Verificar especialmente a posição da prova final nas orientações antigas e o reaproveitamento das etapas já realizadas em 03. Novo conflito concreto de intenção, fonte, preservação ou fluxo retorna à spec; não repetir perguntas já respondidas nem avaliações completas por rotina.

**Encaminhamento registrado na v0.6:** selecionar 05 para changes e elaborar plano/tasks proporcionais quando essa fase for pedida. Este pedido atualizou e reconferiu somente a especificação no backlog e sua entrada de navegação. Guia, skills, textos de publicação/jornada/estudos e localização da iniciativa não foram alterados. Mesma IA autora/revisora com histórico disponível, sem revisão independente ou eficácia editorial demonstrada.

**Histórico v0.2 — 17/10/2026:** análise registrada na própria spec; README/guia examinados como interfaces; nove achados e contrato de adaptação propostos. Sem alteração das regras do guia, das skills, do kit ou da prosa do piloto. A entrada do índice foi atualizada apenas para refletir a análise atual.

**Conferência da análise v0.2:** dez IDs R05 preservados e nove IDs A05 sem duplicação; 33 links locais na spec e índice, sem destinos ausentes. Whitespace da spec e diff do índice conferidos. Sem plano/tasks antecipados, commit ou alteração de staging. Q05-01 estava sem resposta naquela conferência; nenhuma implementação dependente foi executada.

**Histórico v0.3 — 17/10/2026:** resposta autoral incorporada como D05-01 a R05-08 e Q05-01 encerrada. Parecer reconferido somente no aspecto de preservação; demais achados mantidos, sem aceitação presumida ou início de implementação.

**Histórico v0.4 — 17/10/2026:** esclarecimento autoral incorporado à D05-01 e R05-08: preservação necessária de textos de publicação, jornada e capítulos de estudo, sem restringir o gatilho a comparação. Demais encaminhamentos mantidos; implementação não iniciada.

**Histórico v0.5 — 17/10/2026:** oito encaminhamentos restantes consolidados com D05-01 nos dez requisitos existentes; definidos contratos documentais/de fase/adaptação, seis casos de conferência e liberação sem dependência circular. IDs preservados e parecer reconferido: apta para plano, sem nova análise ampla necessária no escopo atual. Guia, skills e peças não alterados nesta rodada.

**Conferência v0.5:** R05-01–10, A05-01–09 e V05-01–06 identificados sem duplicação; destinos dos nove achados presentes nos requisitos/contratos; seções referenciadas e 33 links locais da spec/índice conferidos, sem destinos ausentes. Whitespace e diff do índice sem erros. Conferência documental pela mesma IA, sem execução dos casos futuros, commit ou alteração de staging.

**Histórico v0.6 — 17/10/2026:** D05-02 incorpora o entendimento aprovado na conversa: sequência editorial completa e skills coordenadas com entrada/ação/saída/limite. Acrescentados R05-11/12, A05-10/11 e V05-07/08; IDs anteriores preservados. Reanálise distingue gestão SDD e produção, prepara escolha de conteúdo sem sequência numérica automática e posiciona prova final depois do retorno/ajustes. Prontidão documental mantida para plano; implementação pendente.

**Conferência v0.6:** doze requisitos, onze achados e oito casos previstos sem duplicação; nove etapas editoriais na ordem acordada, com estrutura e ajustes condicionais explícitos. Conferidos os contratos de contexto, autoria, reconferência, retorno e preservação, sem identificar dúvida essencial adicional. Referências de seção e 33 links locais da spec/índice válidos; whitespace e diff do índice sem erros. Conferência documental pela mesma IA com histórico, sem executar o fluxo futuro, alterar peças, criar plano/tasks, commit ou staging.

## 9. Implementação e encerramento — v0.7

O autor autorizou validar e implementar a correção. A mesma pasta foi selecionada para changes, plano e tasks elaborados/conferidos antes da execução. Guia 1.0, README, AGENTS, sete skills, seis modelos e interfaces de 03 foram reconciliados com os doze requisitos. 01/04 receberam notas de vigência sem invalidar por si só as evidências históricas. Ficha do piloto recebeu apenas navegação/contexto histórico; corpos de publicação, jornada e estudos permaneceram preservados.

**Resultado:** concluída no escopo documental. Critérios/evidências e destinos dos limites estão nas tasks; elas não demonstram eficácia literária, todos os modos das skills ou retorno humano. A dependência de método da 03 foi satisfeita; próxima produção é T03-003, sem chamada criada por esta iniciativa. Não houve publicação, commit, push, motor do kit ou cópia paralela. Plano/tasks conservam como base a spec v0.6 aceita antes da execução; esta v0.7 registra somente resultado e vigência, sem alterar os requisitos.

A pasta segue para concluida com links atualizados. O [guia](../../GUIA_DE_OPERACAO.md) e as skills são o procedimento vigente; esta spec conserva intenção/decisões e os limites da correção, sem exigir sua leitura integral a cada peça.
