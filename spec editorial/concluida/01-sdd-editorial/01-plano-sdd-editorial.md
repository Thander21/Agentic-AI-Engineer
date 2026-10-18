# Plano de implementação do SDD editorial

**ID:** PLANO-EDITORIAL-001  
**Versão:** 0.5 — conferido e arquivado como concluído

**Base:** [SPEC-EDITORIAL-001, versão 0.7](01-especificacao-sdd-editorial.md)

**Estado:** ENT-01 a ENT-06 encerradas nos limites registrados nas tasks; ENT-07 transferida para a spec 03, sem execução.

**Regra vigente de escopo:** seção 19 da spec 01. As descrições de implementação e os contratos abaixo são preservados; menções à execução do piloto são condições para a iniciativa 03, não entregas remanescentes de 01.

## 1. Resultado pretendido

Construir uma primeira versão utilizável do método: guia, modelos e procedimentos reutilizáveis para elaborar specs, planos e tasks e para produzir e revisar textos. A implementação deverá permitir executar o piloto no texto 01 da jornada quando as escolhas editoriais necessárias estiverem definidas.

A análise e a revisão da metodologia permanecem na spec. Este plano define como materializá-la. As [tasks 01](01-tasks-sdd-editorial.md), já elaboradas, registrarão a execução e as conferências. Os documentos produzidos serão avaliados pelos critérios editoriais pertinentes à sua função.

## 2. Decisões de implementação

- Manter os documentos em Markdown, com nomes e caminhos locais estáveis.
- Criar um guia de operação como referência das passagens e dos estados. As skills referenciam o guia e os modelos, evitando cópias divergentes das regras.
- Separar as skills que elaboram o método das skills que produzem textos. Uma skill pode ter modos explícitos, mas cada execução informa seu modo e sua entrega.
- Manter as especialidades editoriais como perfis de uma skill de revisão. Cada parecer continua restrito ao papel e à versão examinada.
- Guardar os pacotes de skills no projeto, em `spec editorial/skills/`. O uso inicial será por leitura explícita de seu `SKILL.md`; a existência dessa pasta não significa descoberta automática pelo ambiente.
- Não instalar globalmente nem depender de acionamento automático nesta primeira implementação. Uma integração futura com descoberta automática deverá ter configuração e verificação próprias.
- Usar o processo manualmente para criar suas primeiras skills e modelos. Não atribuir o planejamento atual a skills ainda inexistentes.

## 3. Organização dos artefatos

Os caminhos de artefatos abaixo continuam relativos a `spec editorial/`. Os três documentos da iniciativa foram arquivados em `spec editorial/concluida/01-sdd-editorial/`; seus links refletem a localização atual. A linha de tasks indica o documento ao lado deste plano. Os demais caminhos identificam as entregas deste plano. Sua existência, versão e situação de conferência são acompanhadas nas tasks.

| Caminho | Função |
| --- | --- |
| `01-tasks-sdd-editorial.md` | Tarefas, implementação, conferência e pendências desta iniciativa. |
| `GUIA_DE_OPERACAO.md` | Como iniciar, escolher percurso, passar contexto, revisar, integrar e encerrar. |
| `modelos/spec.md` | Análise, requisitos, decisões, revisão e parecer de prontidão em um documento. |
| `modelos/plano.md` | Entregas, caminhos, dependências, cobertura e conferência. |
| `modelos/tasks.md` | Tarefas com resultados, evidências e estados. |
| `modelos/ficha-editorial.md` | Formas curta e completa para orientar uma entrega textual. |
| `modelos/parecer-editorial.md` | Achados, ganhos, possíveis perdas e passagens a preservar. |
| `modelos/integracao-e-avaliacao.md` | Decisões sobre pareceres, versões e avaliação do uso. |
| `skills/<nome>/SKILL.md` | Procedimento reutilizável identificado na seção 5. |
| `skills/editorial-revisar/references/perfis.md` | Critérios das especialidades de revisão. |

Os modelos de spec, plano e tasks explicitam o suporte necessário aos REQ-17 a REQ-19. São modelos para iniciativas futuras; não exigem reformatar retroativamente as specs 01 e 02.

O destino dos arquivos do piloto será definido no documento 02. Este plano não transfere registros, anexos ou textos da jornada para a pasta da metodologia. Pareceres curtos podem ficar no registro de integração; anexos separados só serão criados quando melhorarem a consulta.

## 4. Sequência de entregas e dependências

| ID | Entrega | Depende de | Critério de conferência |
| --- | --- | --- | --- |
| ENT-01 | Guia de operação. | Spec 0.5 e este plano. | Define entradas, papéis, percursos, estados, encaminhamento de dúvidas e encerramento; distingue método, texto e publicação. |
| ENT-02 | Modelos de spec, plano e tasks. | ENT-01. | Preservam o fluxo de três documentos; cada um recebe e devolve o contexto necessário à fase seguinte. |
| ENT-03 | Modelos de ficha, parecer e integração. | ENT-01. | Cumprem os contratos da seção 16.4 da spec, incluindo versão, fontes, limitações e comparação entre versões. |
| ENT-04 | Skills para elaborar e acompanhar a metodologia. | ENT-01, ENT-02 e modelo de parecer de ENT-03. | Cada modo possui gatilho, entradas, sequência, saída, limites e critério de encerramento. |
| ENT-05 | Skills de produção editorial e perfis de revisão. | ENT-01 e ENT-03. | Cobrem preparação, redação, revisão e refatoração; distinguem erro, preferência e fato não confirmado. |
| ENT-06 | Conferência integrada dos artefatos. | ENT-01 a ENT-05. | Ligações funcionam, requisitos têm cobertura e nenhuma passagem depende de campo ausente ou procedimento indefinido. Achados ficam nas tasks. |
| ENT-07 — transferida | Aplicação no piloto 01 e avaliação, agora na [spec 03](../../concluida/03-piloto-editorial/03-piloto-editorial.md). | Método de 01 e preparação suficiente em 02. | Critérios preservados em 03; não executada e não incluída no fechamento de 01. |

ENT-02 e ENT-03 podem ser elaboradas após o guia; ENT-04 e ENT-05 são frentes separáveis depois dos respectivos modelos. A execução pode ser inteiramente sequencial. O plano não exige agentes simultâneos.

O primeiro documento de tasks será elaborado manualmente a partir deste plano e do contrato da spec, pois o modelo e a skill de tarefas ainda serão construídos em ENT-02 e ENT-04. Depois de produzidos, conferir a compatibilidade das tasks existentes com eles, sem renumerar IDs ou reiniciar o histórico. Assim, a criação do processo não depende de suas próprias entregas ainda inexistentes.

Os antigos IMP-01 a IMP-07 da seção 16 da spec são insumos preliminares: guia → ENT-01; modelos → ENT-03; skills → ENT-04/05; conferência → ENT-06; piloto → ENT-07. ENT-02 acrescenta os modelos de elaboração do método. As tasks usarão os IDs ENT deste plano para evitar dois acompanhamentos concorrentes.

## 5. Agrupamento inicial das skills

| Nome e caminho sob `skills/` | Modos / responsabilidade | Saída e limites |
| --- | --- | --- |
| `sdd-editorial-especificar/SKILL.md` | Analisar contexto; elaborar spec; revisar consistência. | Atualiza a spec, com achados e parecer. Não gera plano ou implementação sem uma tarefa correspondente. A revisão no mesmo contexto é declarada como tal. |
| `sdd-editorial-planejar/SKILL.md` | Converter spec revisada em plano. | Plano separado, com entregas e cobertura; decisões que alterem requisitos retornam à spec. |
| `sdd-editorial-tarefas/SKILL.md` | Decompor plano; acompanhar execução; registrar conferência e reabertura. | Tasks atualizadas com evidência. Encaminha produção à capacidade apropriada; não equipara arquivo gerado a tarefa concluída. |
| `editorial-preparar/SKILL.md` | Reunir contexto, fontes e lacunas; formular perguntas. | Ficha editorial proporcional ao trabalho. Não inventa dados pessoais nem decide voz pelo autor. |
| `editorial-redigir/SKILL.md` | Elaborar esboço; redigir texto ou documento conforme sua função. | Versão identificada, com pendências. A redação de um guia privilegia precisão e utilidade; a narrativa usa apenas a liberdade definida na ficha. |
| `editorial-revisar/SKILL.md` | Executar um perfil por leitura. | Parecer com trecho, fundamento, ganho e possível perda; pode recomendar preservar. Não reescreve o arquivo durante a avaliação. |
| `editorial-integrar/SKILL.md` | Integrar pareceres; refatorar; encaminhar reconferência. | Nova versão e registro das decisões. Mudanças de sentido voltam ao revisor pertinente; questões autorais voltam ao autor. |

Os perfis de `editorial-revisar` serão: desenvolvimento/estrutura; fatos e fontes; didática; continuidade; voz e tom; linha e fluidez; preparação linguística; leitura crítica; prova final. Perfis não pertinentes à entrega são dispensados com motivo, sem aprovação fictícia.

Implementar e conferir artefatos é uma composição: a skill de tarefas delimita a entrega; a capacidade adequada a produz; a revisão examina os critérios; a integração resolve achados; as tasks registram o resultado. A criação técnica de pacotes de skills deverá seguir as instruções de autoria de skills disponíveis no ambiente durante a implementação, além dos critérios editoriais.

Cada pacote deverá identificar quando usar e quando não usar, contexto mínimo, documentos de referência, passos, formato de saída, limites e exemplo curto de aplicação. O exemplo ilustra o procedimento e não conta como evidência de execução real.

### 5.1. Estrutura e seleção de contexto

Cada `SKILL.md` terá frontmatter YAML com `name` e `description`, indicando capacidade e situação de uso. O nome corresponderá à pasta. A descrição deve permitir distinguir pedidos como “revise esta spec”, “escreva este episódio” e “confira estas tarefas”; mencionar escrita em um pedido não aciona automaticamente toda a cadeia.

No corpo, incluir: resultado esperado; escolha de modo; entradas mínimas; decisões específicas do procedimento; saída; limites; condições para pedir informação ou devolver o trabalho à etapa anterior. Manter o corpo enxuto e carregar referências detalhadas somente quando necessárias. Não incluir tutoriais genéricos, pastas vazias, scripts sem necessidade ou cópias completas do acervo.

Resolver caminhos de apoio a partir da localização do pacote. Os modelos compartilhados estão em `../../modelos/` e o guia em `../../GUIA_DE_OPERACAO.md`, em relação a cada pasta de skill. Isso torna explícita a dependência do conjunto local; copiar apenas uma pasta de skill não garante seu funcionamento isolado. Uma referência ausente deve ser informada, sem inventar seu conteúdo.

O pacote do revisor usará `references/perfis.md`, com seções identificadas por especialidade. Se o conteúdo ficar grande ou os perfis tiverem instruções extensas, poderão ser separados em arquivos referenciados, preservando os mesmos papéis. A implementação não exige sete conjuntos de instruções duplicadas sobre o projeto.

### 5.2. Contratos de execução por skill

**`sdd-editorial-especificar`**

- Recebe pedido, versão existente se houver, documentos pertinentes e decisões conhecidas. Identifica se a tarefa é analisar, elaborar ou revisar, sem executar os demais modos por consequência automática.
- Na análise, separa necessidade, preferência, restrição e hipótese; na elaboração, traduz as decisões em requisitos com critério observável; na revisão, procura ambiguidade, contradição, ausência de base e dependência circular.
- Devolve a spec atualizada com achados e decisões, ou um parecer localizado quando a tarefa for apenas analisar. Só indica prontidão quando as lacunas que impedem o próximo passo estiverem resolvidas. Pendências do piloto não devem bloquear indevidamente o planejamento.
- Se faltar decisão autoral essencial, formula uma pergunta específica e avança apenas nas partes independentes. Não assume que uma proposta anterior foi aceita.

**`sdd-editorial-planejar`**

- Recebe spec identificada e seu parecer de prontidão. Se houver mudança posterior relevante, reconfere o ponto afetado antes de usar um parecer antigo.
- Converte requisitos em entregas, dependências, caminhos e critérios. Distingue procedimento, arquivo e evidência; não cria um artefato para cada frase da spec.
- Devolve plano separado com cobertura dos requisitos, decisões de implementação e dependências externas. Requisito sem destino ou dependência circular impede declarar o plano pronto para tasks.
- Se descobrir uma necessidade que altera o escopo, devolve a questão à spec; não a introduz silenciosamente como tarefa técnica.

**`sdd-editorial-tarefas`**

- Recebe plano e spec identificados; para acompanhar uma execução, recebe também as tasks existentes e evidências dos artefatos.
- Cada tarefa representa uma entrega ou alteração verificável. Dividir tarefas que tenham resultados independentes; evitar tarefas como “melhorar tudo” ou uma lista para cada correção ortográfica.
- Devolve tasks com ID, requisitos, dependências, resultado esperado e critério de conclusão. No modo acompanhamento, registra a versão produzida, a conferência real e seus limites.
- Arquivo existente sem conferência fica produzido/aguardando conferência. Evidência invalidada por alteração posterior exige reabertura. A skill coordena o registro, sem declarar que realizou operações apenas planejadas.

**`editorial-preparar`**

- Recebe pedido, destino conhecido, registros e decisões editoriais disponíveis. Seleciona apenas o contexto necessário à entrega e identifica a origem de cada afirmação central.
- Produz ficha curta ou completa conforme escopo, quantidade de fontes e dificuldade. Identifica se o material é relato real, exemplo fictício ou documento operacional.
- Se faltar uma vivência, pergunta pelo acontecimento concreto e permite que o autor não queira relatá-lo. Se faltar fonte, registra a necessidade; uma transcrição de IA não se transforma em evidência técnica por estar arquivada.
- Devolve ficha utilizável e lacunas classificadas como impeditivas para a redação ou compatíveis com um rascunho marcado. Não incorpora toda a conversa original como contexto padrão.

**`editorial-redigir`**

- Recebe ficha, fontes, trechos vizinhos quando pertinentes e escolhas de voz. Confere o que pode afirmar e o que só pode propor antes de escrever.
- No modo documento operacional, prioriza decisões claras e instruções utilizáveis. No modo narrativo, escolhe progressão, cenas e explicações conforme a intenção; pode propor alternativas de abertura ou estrutura quando houver uma escolha relevante, sem exigir várias versões sempre.
- Usa detalhes reais e mudanças de entendimento para sustentar a narrativa. Metáforas, ritmo, humor e recursos literários têm liberdade dentro do contrato autoral. Não exige derrota, lição ou piada em cada seção; não converte ficção ilustrativa em autobiografia.
- Devolve esboço ou rascunho conforme solicitado, com versão e pendências identificadas fora da prosa final sempre que possível. Uma lacuna pode aparecer como marca editorial no rascunho, mas não como fato inventado.
- Se a nova direção mudar a promessa do texto, registra a proposta de mudança na ficha antes de apresentá-la como decisão consolidada.

**`editorial-revisar`**

- Recebe versão do texto, ficha ou contrato do artefato, perfil selecionado e fontes necessárias. Se o perfil for omitido, escolhe o pertinente ao pedido e explicita o escopo; não aplica todos por padrão.
- Faz a primeira leitura sem pareceres anteriores quando o contexto permitir. Cada perfil examina sua especialidade; problemas relevantes fora dela podem ser sinalizados para encaminhamento, sem simular uma revisão completa.
- Devolve achados fundamentados e trechos a preservar. Distingue erro normativo, ambiguidade, falta de evidência e preferência expressiva. A intensidade do humor vem da ficha, não do gosto do revisor.
- Não emite aprovação factual quando não consultou a base necessária. Não reescreve durante o parecer e não aplica detectores de autoria como evidência de naturalidade.

**`editorial-integrar`**

- Recebe versão de partida recuperável, pareceres e decisões autorais. Confirma que os pareceres se referem à versão pertinente; um parecer desatualizado precisa ser reavaliado no trecho afetado.
- Classifica achados, resolve conflitos por intenção, fontes e voz, e aplica mudanças justificadas. Preserva fatos, ressalvas e traços expressivos, inclusive quando a passagem não segue um padrão estilístico genérico.
- Devolve nova versão e registro do destino de cada achado. Faz leitura do conjunto após as alterações e encaminha mudanças de sentido à reconferência adequada.
- Impasses sobre vivência, posição do autor ou alteração da tese voltam ao autor. A integração não declara aprovação autoral nem publicação.

### 5.3. Referência de voz como entrada editorial

A voz do texto vem do autor e das decisões editoriais; as skills oferecem meios para desenvolvê-la e preservá-la. ENT-03 deve prever, na ficha, uma referência de voz proveniente da spec 02 com:

- Amostras escolhidas pelo autor e descrição do que deseja manter ou evitar em cada uma.
- Público, proximidade com o leitor, pessoa narrativa, variante linguística e intensidade de humor.
- Vocabulário técnico e metáforas pertinentes, sem exigir que o leitor conheça RPG ou anime.
- Liberdades criativas e limites factuais; diferenças de voz entre relato, postagem e documento operacional.

As amostras orientam escolhas, sem virar moldes de frases. Sua ausência não impede criar as skills, mas limita avaliar a fidelidade à voz no piloto. Um texto com gramática correta não está automaticamente aprovado em ritmo, interesse ou personalidade.

Textos selecionados do Obsidian podem ser fornecidos como Markdown comum, acompanhados de contexto, intenção, preferências do autor e indicação de reescrita por IA quando houver. Links e propriedades são aproveitados quando ajudarem a interpretação. Não há dependência de integração com o Obsidian ou importação do cofre inteiro; hábitos de anotação rápida não são automaticamente características a reproduzir no livro.

### 5.4. Avaliação da construção e do comportamento

ENT-04 e ENT-05 devem incluir conferência estrutural do frontmatter, nomes, referências e ausência de instruções incompletas. Usar o validador de skills disponível quando aplicável; sua aprovação verifica estrutura, não qualidade editorial. Não criar scripts próprios de teste para este projeto apenas para conferir texto.

ENT-06 incluirá exercícios curtos e identificados como avaliação, com entradas sintéticas ou recortes permitidos, sem alterar os originais. Eles não executam o piloto 01 antecipadamente e não substituem a apreciação do autor. Registrar nas tasks entrada, versão da skill, resultado observado e ajuste necessário. Comparar decisões e efeitos, não coincidência de palavras com uma resposta modelo.

| Procedimento | Situação de avaliação | Comportamento esperado |
| --- | --- | --- |
| Especificar | Pedido contém duas regras incompatíveis e um exemplo apresentado como sugestão. | Expõe o conflito e mantém o exemplo como proposta; não declara prontidão indevida. |
| Planejar | Uma parte depende de decisão editorial e outra pode ser preparada antes. | Planeja a parte independente e marca a dependência sem assumir a decisão ou bloquear tudo. |
| Tarefas | Arquivo produzido sem revisão, seguido de mudança após uma conferência. | Distingue produzido de concluído e reabre a conferência afetada. |
| Preparar | Registro incompleto sobre uma experiência pessoal. | Faz pergunta localizada ou marca a lacuna; não cria emoção, diálogo ou resultado. |
| Redigir | Ficha permite humor, mas o material não contém uma derrota. | Produz progressão coerente sem fabricar fracasso ou forçar uma lição moral. |
| Revisar | Trecho contém erro de concordância e fragmento intencional com função rítmica. | Corrige o erro e justifica manter ou discutir o fragmento, sem normalizar tudo. |
| Integrar | Dois pareceres discordam sobre uma piada, e outro altera uma ressalva factual. | Decide conforme a ficha e preserva a ressalva ou solicita reconferência; não aceita por maioria. |
| Seleção e limites | Pedido solicita somente análise de uma spec. | Seleciona o procedimento adequado e não gera rascunho narrativo, plano, tasks ou publicação sem necessidade. |

A avaliação pode ser manual e sequencial. Quando a execução tiver acesso ao resultado esperado ou a pareceres prévios, registrar essa limitação; não alegar independência. Um exercício com resultado ruim gera ajuste localizado e reconferência do aspecto afetado. Mais regras não são automaticamente uma melhoria.

Registrar a cobertura por modo e perfil: conferido documentalmente, exercitado com resultado observado ou ainda não avaliado. Um exercício de concordância não comprova revisão factual, continuidade ou estrutura. Exercitar os modos e perfis previstos para o primeiro uso com poucos casos representativos, podendo combinar aspectos no mesmo material e emitir pareceres distintos. Os demais permanecem com sua limitação explícita; antes de incorporá-los ao piloto, avaliar seu comportamento pertinente.

### 5.5. Condição para considerar uma skill pronta para o piloto

Uma skill estará pronta para uso inicial quando seu contrato estiver completo, suas referências acessíveis, sua estrutura conferida e as situações pertinentes de ENT-06 não revelarem impedimentos em aberto. O resultado será “pronta para piloto”, não “qualidade literária comprovada”. O piloto continua necessário para avaliar colaboração entre skills, esforço e voz do autor.

Falhas como inventar fatos, perder ressalvas, executar outra fase sem pedido ou declarar validação inexistente impedem a prontidão da skill afetada. Preferências literárias são avaliadas por trecho e pela intenção, com espaço para julgamento humano.

## 6. Identificação, versões e estados

Usar `SPEC-EDITORIAL-001`, `PLANO-EDITORIAL-001` e, nas tasks, `TASKS-EDITORIAL-001`, com tarefas `T01-001`, `T01-002` e assim por diante. Não renumerar tarefas após criação; novas tarefas recebem novos IDs. Cada tarefa indica a versão da spec/plano relevante e a entrega ENT correspondente.

Preservar os IDs existentes de sessões, episódios e publicações. Para uma entrega editorial sem ID anterior, atribuir `TXT-001`, `TXT-002` etc., verificando previamente os IDs usados. Distinguir o ID do texto do número da etapa da jornada. Cada parecer identifica o ID e a revisão exata do texto, por exemplo `TXT-001 / r01`.

As versões anteriores necessárias à comparação devem ser recuperáveis antes de integrar mudanças. O guia deverá orientar a preservação de cópias identificadas ou o uso de histórico disponível, sem presumir que salvar por cima conserva uma versão.

Nas tasks, adotar os estados da spec: pendente; em execução; produzida/aguardando conferência; concluída; bloqueada com motivo. Nos registros de conteúdo, conservar nota de estudo, caso documentado, caso conferido, texto para leitura e capítulo revisado. Publicação e apreciação autoral são informações separadas, não consequências automáticas de concluir uma tarefa.

## 7. Cobertura dos requisitos

| Requisito | Entregas responsáveis | O que conferir |
| --- | --- | --- |
| REQ-01 | ENT-03, ENT-05 | Público, pergunta e contribuição identificados na ficha. |
| REQ-02 | ENT-03, ENT-05 | Afirmações relevantes ligadas a fontes ou pendências. |
| REQ-03 | ENT-03, ENT-05 | Fato, hipótese, interpretação e ficção distinguíveis. |
| REQ-04 | ENT-03, ENT-05, ENT-07 | Espaço criativo e decisão autoral preservados. |
| REQ-05 | ENT-03, ENT-05 | Vínculos com jornada, livro e textos vizinhos. |
| REQ-06 | ENT-03, ENT-05 | Pareceres e critérios próprios por perspectiva. |
| REQ-07 | ENT-01, ENT-03 | Reaproveitamento mantém a ligação à origem. |
| REQ-08 | ENT-01, ENT-03, ENT-07 | Percurso e preenchimento proporcionais. |
| REQ-09 | ENT-02, ENT-03, ENT-04, ENT-05 | Mudança registra motivo e impactos. |
| REQ-10 | ENT-01, ENT-02, ENT-03 | Rascunho, revisão e publicação não se confundem. |
| REQ-11 | ENT-03, ENT-05 | Contexto, papel e versão examinada identificados. |
| REQ-12 | ENT-01, ENT-05 | Estrutura precede acabamento. |
| REQ-13 | ENT-05 | Perfis de língua, voz e fluidez respeitam escolhas expressivas. |
| REQ-14 | ENT-03, ENT-05 | Refatoração preserva sentido ou explicita a mudança. |
| REQ-15 | ENT-01, ENT-03, ENT-05 | Conflitos resolvidos e encerramento fundamentado. |
| REQ-16 | ENT-03, ENT-05, ENT-07 | Apreciação qualitativa e retorno humano claramente identificados. |
| REQ-17 | ENT-02, ENT-04 | Análise e revisão permanecem na spec. |
| REQ-18 | ENT-02, ENT-04 | Plano separado vincula entregas à spec. |
| REQ-19 | ENT-02, ENT-04 | Tasks mantêm estado, execução, evidência e pendências. |
| REQ-20 | ENT-03, ENT-04, ENT-05, ENT-06 | Revisão adequada ao artefato retorna às tasks. |

Esta é cobertura planejada. ENT-06 examina os artefatos produzidos; ENT-07 avalia seu uso. Nenhum requisito está marcado como comprovado apenas por constar na tabela.

## 8. Conferência proporcional às entregas

Para guia, modelos e skills, fazer leitura de estrutura, coerência, linguagem e conformidade com os contratos. Percorrer manualmente uma entrada, a saída esperada e o encaminhamento de uma lacuna, sem exigir código ou uma suíte de testes. Registrar essa conferência como documental, sem confundi-la com aplicação real ao piloto.

Nos pareceres, observar os três compromissos: primeira leitura sem pareceres anteriores quando possível; ganho e possível perda em cada sugestão; preservação do que funciona. Se o revisor tiver acesso ao histórico, explicitar a limitação. A leitura final integrada confere efeitos das alterações sobre o conjunto.

Nas tasks, registrar o artefato e sua versão, critérios examinados, resultado e achados. Um impeditivo aberto impede concluir a tarefa afetada; uma preferência não acolhida pode ser encerrada com justificativa. Conferências posteriores devem atingir os aspectos invalidados pela mudança.

## 9. Dependências do piloto e avaliação

**Destino vigente desde v0.4:** esta seção conserva as condições da entrega transferida para a spec 03. A análise e os complementos necessários de contexto, voz, fatos e cobertura das skills ficam na spec 02. Não são pendências do escopo encerrado da iniciativa 01.

O piloto permanece [01 — Novo mundo, bagagem antiga](<../../../jornada do heroi/01-novo-mundo-bagagem-antiga.md>). Antes de ENT-07, o [resumo editorial 02](../02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md) precisa definir para essa entrega: leitor, propósito, formato, voz, variante linguística, humor, destino, local dos arquivos de trabalho e momento de uso. Também precisam estar disponíveis os detalhes pessoais necessários ao relato.

Essas pendências não bloqueiam ENT-01 a ENT-06. Não é necessário fechar o calendário completo de postagens; é necessário saber a finalidade e as condições de uso do texto piloto. Publicação continua fora da execução automática.

A avaliação deverá separar: suficiência da spec e do contexto recebido; funcionamento dos procedimentos; qualidade e voz do texto; esforço e retrabalho. Usar o modelo de integração e registrar a localização do resultado nas tasks, sem impor um documento extra de acompanhamento. O autor avalia sua voz e experiência de leitura; a ausência dessa apreciação permanece pendente.

Nas tasks de ENT-07, separar produção/revisão do texto e avaliação autoral. A parte executada pode ser conferida enquanto se aguarda o autor, mas a entrega de avaliação completa do piloto não será concluída sem esse retorno. Registrar a dependência sem presumir aprovação ou deixar indefinido o critério de conclusão.

## 10. Prontidão para gerar tasks

**Registro histórico das versões 0.2/0.3:** a decomposição abaixo já foi executada. O encerramento do escopo 0.4 está na seção 12 e nas tasks 0.21.

O plano define sete entregas, sete pacotes de skills, seus caminhos, dependências, contratos e cobertura dos vinte requisitos. A versão 0.2 detalha seleção de contexto, contratos por skill, referência de voz e situações de avaliação. As decisões editoriais ainda abertas têm destino e momento de resolução identificados. O agrupamento não altera as regras da spec.

**Parecer documental de planejamento: apto para decomposição em tasks.** Esse parecer não comprova implementação nem validação em uso. A situação atual de execução e conferência está nas tasks. Este plano foi elaborado com acesso à spec e ao histórico, sem alegação de revisão independente.

**Decomposição realizada:** [tasks 01](01-tasks-sdd-editorial.md), com tarefas delimitadas a partir de ENT-01 a ENT-07, incluindo produção e conferência antes da conclusão de cada entrega. Consultar ali o próximo trabalho executável.

## 11. Histórico de revisão do plano

| Versão | Revisão | Resultado |
| --- | --- | --- |
| 0.1 | Agrupamento das skills, entregas e cobertura. | Estrutura geral definida; contratos ainda resumidos. |
| 0.2 | Revisão com orientação de autoria de skills e detalhamento das seções 5.1 a 5.5. | Lacunas de planejamento tratadas; comportamento ainda não avaliado porque as skills não foram implementadas. |
| 0.3 | Conferência cruzada com a spec: início manual das tasks, cobertura dos modos/perfis, conclusão da avaliação autoral e uso de amostras Markdown. | Apto para tasks; sem impedimentos documentais restantes nesta revisão. |
| 0.4 | Separação autorizada pela spec 01 v0.6: ENT-01 a ENT-06 em 01; preparação em 02; ENT-07 em 03. | Escopo de construção encerrado; cobertura e critérios práticos preservados para o piloto futuro. |
| 0.5 | Auditoria e arquivamento, com base na spec 0.7; correção de E03 e destinos dos critérios antigos conferidos. | Método concluído no recorte; piloto não executado. |

## 12. Conferência da redistribuição

Conferidos os vínculos entre spec 01 v0.6, este plano v0.4, tasks v0.21 e specs 02/03. ENT-01 a ENT-06 continuam cobertas por T01-001 a T01-017; ENT-07 e suas quatro tarefas têm destino explícito em 03. A tabela de requisitos da seção 7 conserva a responsabilidade prática de ENT-07 onde aplicável; a transferência não transforma avaliação humana em conferência documental.

Complementos condicionais dos exercícios serão delimitados e registrados em 02, aproveitando T01-016 como evidência histórica. Seus resultados não serão retroativamente atribuídos aos exercícios antigos.

**Resultado:** plano coerente com a separação de escopo autorizada. Revisão pela mesma IA, com acesso ao histórico. O fechamento de 01 é sustentado pelas evidências das tasks; planejamento e execução de 03 aguardam a preparação em 02.

## 13. Auditoria e arquivamento — v0.5

Base atual: spec 01 v0.7 e tasks v0.22. A revisão anterior ao arquivamento preserva ENT-01 a ENT-06 e a transferência de ENT-07. A seção 20 da spec reconcilia todas as decisões e a checklist original. Corrigida a falha de aplicação em E03; o contrato da skill e os critérios do plano não precisaram mudar. Não foi encontrada entrega ausente no escopo documental.

Spec, plano e tasks arquivados juntos em `spec editorial/concluida/01-sdd-editorial/`. Guia, modelos, skills e avaliações continuam nos caminhos de uso. Links atualizados e conferidos após a mudança. Parecer: coerente com o encerramento e apto ao arquivamento; avaliação aplicada continua em 03. Revisão pela mesma IA, com acesso ao histórico.
