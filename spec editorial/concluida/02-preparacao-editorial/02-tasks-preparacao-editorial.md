# Tasks 02 — Preparação editorial

**ID:** TASKS-EDITORIAL-002  
**Versão:** 0.21

**Data:** 2026-10-16

**Spec de referência:** [SPEC-EDITORIAL-002 v0.26](02-resumo-editorial-onde-como-quando.md).
**Plano de referência:** [PLANO-EDITORIAL-002 v0.9](02-plano-preparacao-editorial.md), reconferências e destinos definidos no documento.
**Responsável pelo acompanhamento:** IA no papel de editor responsável.  
**Estado geral:** T02-001 a T02-007 concluídas no escopo documental e sintético de preparação. Piloto, apreciação autoral e publicação pertencem às próximas entregas.

## 1. Escopo e preservação

Executar ENT02-01 a ENT02-05 do plano, cobrindo R02-01 a R02-05. Caminhos simples partem desta pasta; caminhos iniciados por `spec editorial/` partem da raiz do repositório.

Preservar fontes, anexos e texto 01 da jornada. A spec v0.5 e o índice anteriores à abertura estão em `spec editorial/historico/2026-10-14-antes-da-abertura-do-change-02/`, com igualdade dos hashes conferida antes da edição. Novas integrações exigem versão recuperável correspondente.

D02-01 a D02-10 têm encaminhamento suficiente para o recorte de RA02-16. Consulte a síntese e o parecer da spec v0.26; registros antigos conservam o estado da data. T01-018 a T01-021 permanecem origens de 03, sem execução atribuída aqui.

## 2. Definição das tarefas

| ID | Entrega / requisitos | Dependências | Papel responsável | Resultado e destino | Critério de conclusão |
| --- | --- | --- | --- | --- | --- |
| T02-001 | ENT02-01; R02-02. | Spec e fontes apontadas disponíveis. | IA analista; conferência editorial. | Inventário factual e lacunas na spec. | Conferir afirmações centrais e atribuição nas fontes; distinguir intenção, autopercepção, experiência, metáfora e resposta de IA; formular perguntas delimitadas sem presumir respostas. |
| T02-002 | ENT02-01; R02-02; D02-06/D02-08. | T02-001 e retorno factual do autor. | Autor confirma; IA registra e confere a representação. | História e limites de exposição na spec. | Receber posição atual sobre estudar/orquestrar/ler código e fatos necessários; registrar confirmações e limites ou exclusões justificadas por recorte. Sem retorno essencial, manter pendência. |
| T02-003 | ENT02-02; R02-03; D02-04/D02-09. | T02-001, amostras selecionadas e retorno do autor. | IA compara; autor define referências. | Referência de voz na spec; anexo identificado apenas se necessário. | Registrar origem/participação conhecida de IA, trechos, características a preservar/evitar, variante e humor; distinguir preferência recebida de impressão da IA. |
| T02-004 | ENT02-03; R02-01/R02-05; origem histórica: spec v0.19. | T02-002/T02-003 e decisões do autor. | IA apresenta consequências; autor define preferências. | Condições da primeira publicação na spec. | Fechar finalidade, recorte, canal, formato/extensão, armazenamento/versões e momento/condições de uso para o texto; preservar público/voz recebidos e publicação como ação específica. |
| T02-005 | ENT02-04; R02-04; D02-10. | T02-004 e cobertura de T01-016. | IA analisa e confere contratos. | Seleção de modos/perfis na spec; matriz de cobertura neste acompanhamento. | Justificar cada modo necessário e dispensas pertinentes; confrontar versão e cobertura; definir complementos com critérios prévios ou justificar ausência de necessidade. |
| T02-006 | ENT02-04; R02-04. | T02-005. | IA executora e conferente, com limites declarados. | Evidências dos complementos necessários; destino previsto `spec editorial/avaliacoes/T02/`. | Executar e conferir somente os casos requeridos, registrar entradas/saídas e reconferir correções. Se nenhum caso for necessário, concluir por justificativa conferida de T02-005, sem alegar exercício realizado. |
| T02-007 | ENT02-05; R02-01 a R02-05. | T02-002/T02-003/T02-004/T02-005/T02-006. | IA consolida; autor resolve pendências pessoais essenciais. | Parecer de suficiência na spec e resultado neste acompanhamento. | Examinar os cinco R02 com evidência e versão; resolver impeditivos e explicitar pendências compatíveis; identificar a entrada de 03 ou registrar insuficiência concreta. |

## 3. Estados e acompanhamento atual

Usar pendente para trabalho não iniciado, inclusive com dependências futuras; em execução após início efetivo; produzida/aguardando conferência para saída ainda não inteiramente examinada; concluída somente com critério e evidência atendidos. Bloqueada com motivo exige tentativa de avanço e impedimento concreto. Ao reabrir, preservar a evidência anterior e identificar a mudança que a invalidou.

| Tarefa | Estado | Artefato / versão produzida | Conferência da entrega | Pendências / próximo passo |
| --- | --- | --- | --- | --- |
| T02-001 | Concluída | Spec 02 v0.7, inventário IF02-01 a IF02-08 e perguntas Q02-01 a Q02-03. | Atende no escopo documental; registro de execução abaixo. Não confirma veracidade dos relatos. | Inventário disponível para T02-002 e seleção de amostras em T02-003. |
| T02-002 | Concluída | Spec v0.16, RA02-01 a RA02-09 e delimitação do recorte factual. | Intenção atual, participação, ação/resultado relatado, sequência aproximada e autorização dos nomes conferidas nos retornos; detalhes não necessários excluídos do recorte. | Reabrir o aspecto afetado se o recorte exigir novos fatos, diagnóstico técnico ou exposição adicional. |
| T02-003 | Concluída | Spec v0.24, RA02-15; direção pessoal reconferida documentalmente, com referência histórica v0.14 em português brasileiro; fonte em [02-amostras-de-voz.md](02-amostras-de-voz.md), preservada. | Amostras, combinação, participação conhecida de IA, variante e direção de humor conferidas com os retornos autorais; D02-04/D02-09 atualizadas por retorno explícito em RA02-15; preferência recebida não equivale a validação do futuro texto. | Aplicar a referência no futuro texto; fidelidade da voz ainda dependerá de apreciação autoral em 03. |
| T02-004 | Concluída | Spec v0.25, RA02-16. | Extensão recebida; recorte, canais, versões e prontidão definidos. | Texto e apreciação em 03; publicação separada. |
| T02-005 | Concluída | Matriz RA02-16; critérios EX02-A/B. | Versões e cobertura histórica confrontadas; complementos e dispensas justificados. | Conferir resultados de T02-006. |
| T02-006 | Concluída | EX02-A/B, entradas r01, fichas/redação r01, pareceres e r02. | Critérios A1–A6/B1–B7 atendidos; fontes, versões, chamada e recusa de D1 conferidas. | Limites sintéticos explícitos; uso real em 03. |
| T02-007 | Concluída | Parecer final da spec v0.26. | R02-01 a R02-05 examinados; sem impeditivo no recorte. | 03 recebe ficha/textos/retorno e PEN-03; publicação separada. |

## 4. Registro da abertura — 2026-10-14

**Executado:** avaliação da spec v0.5, atualização para v0.6 e criação do plano v0.1 e destas tasks v0.1. A iniciativa já estava em changes. Preservadas cópias da spec e do índice anteriores à edição, com hashes iguais aos arquivos de partida.

**Conferência documental:** cobertura dos cinco R02 e das dez D02; sete IDs T02 únicos; dependências sem ciclos; correspondência das cinco ENT02 com tarefas de produção e conferência; distinção entre planejar a preparação e liberar o piloto. Evidências de prontidão estão na seção “Avaliação para abertura do change — v0.6” da spec e na seção 9 do plano. Conferidos os três documentos de 02 e o índice: 32 referências locais com destinos existentes, nenhum marcador de conflito e nenhuma dependência ausente ou circular. `git diff --check` sem erros nos arquivos rastreados; arquivos novos examinados diretamente na conferência documental. Resultado estrutural, sem avaliação comportamental ou autoral.

**Resultado:** estrutura suficiente para iniciar a preparação por T02-001. Abertura do change não conclui nenhuma das sete tarefas. Não houve novo exercício nem retorno autoral nesta rodada.

**Responsável e limites:** IA responsável pela elaboração e conferência, com acesso ao histórico e a pareceres anteriores; sem alegação de revisão independente. A revisão documental não confirma relatos pessoais, eficácia das skills, prazer de leitura ou voz do futuro texto.

### T02-001 — execução e conferência — 2026-10-14

**Base:** spec v0.6 → v0.7, plano v0.1 e tasks v0.1 → v0.2. Alteração de evidência e acompanhamento, sem novo requisito ou estratégia. Preservadas spec v0.6, tasks v0.1 e índice em `spec editorial/historico/2026-10-14-antes-do-inventario-T02-001/`, com hashes iguais aos arquivos de partida.

**Executado:** leitura dos cinco blocos F002/F024/F040/F041/F065 e de seus intervalos no original; consulta ao mapa de origem, texto 01, EP-000 e ficha da etapa. Produzidos oito itens de inventário e três perguntas na seção “Inventário factual conferido — T02-001 / v0.7” da spec. Q02-01 a Q02-03 apresentadas ao autor em duas perguntas agrupadas na conversa.

**Conferido:** atribuição e natureza das afirmações, limites de competência e cronologia, separação entre proposta narrativa e vivência e suficiência das perguntas para a próxima etapa. F002 mistura pergunta autoral e resposta; F040 é proposta de IA; F024/F041 não fixam por si uma posição atual. Números históricos de EP-000 não foram revalidados.

**Resultado:** atende ao critério documental de T02-001; tarefa concluída. ENT02-01 permanece incompleta até T02-002 receber as confirmações necessárias. T02-002 iniciada pela apresentação das perguntas, aguardando retorno; T02-003 liberada para seleção de amostras. As demais dependências permanecem.

**Responsável e limites:** mesma IA responsável pela edição, com acesso ao histórico e aos pareceres anteriores. Conferência de transcrição e interpretação, sem confirmação pessoal, diagnóstico técnico, apreciação humana de voz ou redação do piloto.

**Conferência final da rodada:** os cinco blocos do anexo correspondem aos intervalos do original após retirar a marca de citação Markdown e espaços externos ao bloco; sem alegação de comparação byte a byte do arquivo inteiro. Quatro documentos ativos examinados, 34 referências locais com destino existente e nenhum marcador de conflito. `git diff --check` sem erros nos arquivos rastreados. Critério de T02-001 relido contra os oito itens e três perguntas da spec; resultado documental atende, com confirmação autoral ainda pendente.

### T02-002 — primeiro retorno autoral — 2026-10-14

**Executado e evidência:** recebidas duas respostas na conversa e registradas em RA02-01 a RA02-04 da spec v0.8. Identificados PDV D+, Sampa TI, participação anterior como sócio e apoio administrativo remoto atual. O autor aponta a virada de revenda para software house como início e adia a história completa; pede condução por perguntas para manter interesse e concisão.

**Conferido:** síntese relida contra as respostas. A primeira orienta a colaboração editorial, sem responder à autonomia técnica de Q02-01. A finalidade do projeto não foi convertida em implantação ou resultado; participação societária passada não foi convertida em afirmação sobre situação formal atual. Menção a nomes não foi tratada como autorização de publicação.

**Resultado e limites:** retorno parcial registrado; T02-002 permanece em execução. Q02-02 parcialmente respondida, Q02-01 e Q02-03 ainda abertas. Próxima pergunta: motivo principal para desenvolver software próprio. Não há alteração de requisitos ou estratégia; plano v0.1 permanece aplicável. Spec v0.7 e tasks v0.2 preservadas, com hashes iguais, em `spec editorial/historico/2026-10-14-antes-do-retorno-autoral-T02-002/`. Conferência pela mesma IA, com acesso ao histórico; não é verificação externa da empresa ou do produto.

### T02-002 — motivos da decisão — 2026-10-14

**Executado / evidência:** registrado RA02-05 na spec v0.9 a partir da resposta autoral sobre custo, suporte dos parceiros, melhorias não atendidas e intenção de melhorar o atendimento com software mais robusto e atualizado. Outros pontos foram mencionados sem detalhamento.

**Conferido / resultado:** síntese confrontada com a resposta; objetivos não foram apresentados como resultados alcançados. Não foram inventados valores, parceiros, acontecimentos ou hierarquia entre motivos. Retorno parcial atende ao registro da motivação; T02-002 permanece em execução. Próxima pergunta: participação do autor na decisão. Autonomia, cronologia e exposição permanecem pendentes. Conferência pela mesma IA com acesso ao histórico, sem verificação externa. Versões de partida preservadas em `spec editorial/historico/2026-10-14-antes-dos-motivos-T02-002/`, com igualdade de hashes conferida. Plano v0.1 segue aplicável.

### T02-002 — busca da base fiscal — 2026-10-14

**Executado / evidência:** RA02-06 registrado na spec v0.10 a partir da resposta autoral: tentativas em Delphi com freelancers, demora ou pouca evolução, busca de emissor fiscal mais atual e encontro com “phpnfe” como base para refazer em Dart.

**Conferido / resultado:** síntese relida contra a resposta. A experiência relatada não foi generalizada para Delphi ou freelancers; não se inferiram implementação concluída, uso de IA, datas, identidade exata da biblioteca ou autoria individual da decisão. Sequência relativa recebida; T02-002 continua em execução. Próxima pergunta: primeiro passo e participantes depois de encontrar a base. Conferência pela mesma IA, com histórico disponível, sem verificação técnica externa. Spec v0.9 e tasks v0.4 preservadas com hashes iguais em `spec editorial/historico/2026-10-14-antes-da-base-fiscal-T02-002/`. Sem mudança de requisito ou estratégia; plano v0.1 aplicável.

### T02-002 — primeiro MVP e homologação — 2026-10-14

**Executado / evidência:** RA02-07 registrado na spec v0.11 com a resposta do autor: primeiro MVP feito sozinho com “vibecode”, sucesso na emissão de NFC-e em homologação e decisão posterior de estruturar o software.

**Conferido / resultado:** síntese confrontada com a resposta; ambiente de homologação preservado, sem promoção a produção, homologação integral, robustez ou arquitetura concluída. Há agora ação, resultado relatado e decisão subsequente; a ausência de caso concreto da leitura anterior é parcialmente suprida. Não foram atribuídas emoções, datas, ferramentas ou competências não informadas. T02-002 permanece em execução; próximo esclarecimento é o significado prático de estruturar. Plano v0.1 continua aplicável. Spec v0.10 e tasks v0.5 preservadas com hashes iguais em `spec editorial/historico/2026-10-14-antes-do-mvp-T02-002/`. Conferência editorial pela mesma IA, com acesso ao histórico; sem validação técnica da emissão.

### T02-003 — primeira análise das amostras — 2026-10-15

**Executado / evidência:** encontrado o arquivo de amostras preenchido, em vez de criar ou sobrescrever um modelo. Lidos os quatro textos; registradas VOZ02-01 a VOZ02-04 e análise comparativa na spec v0.12, conforme `editorial-preparar` v0.1. Nenhuma ficha final do piloto produzida.

**Conferido / resultado:** títulos, datas exibidas, trechos, proximidade, exemplos, humor, ritmo e intensidade promocional confrontados com a cópia local. Participação de IA e preferências permanecem desconhecidas; hipótese de combinação identificada como proposta. Não foram validados fatos técnicos ou links externos. T02-003 em execução; retorno autoral necessário para concluir R02-03. Conferência pela mesma IA com histórico disponível, sem apreciação humana presumida.

**Preservação / impacto:** spec v0.11 e tasks v0.6 copiadas para `spec editorial/historico/2026-10-15-antes-da-analise-de-voz/`, com igualdade de hashes conferida. Fonte das amostras mantida intacta. Plano v0.1 aplicável; sem alteração de requisitos. A próxima conversa passa às preferências de voz; a pendência factual de T02-002 permanece registrada.

### T02-003 — confirmação das referências — 2026-10-15

**Executado / evidência:** registrada na spec v0.13 a aceitação autoral da combinação das três primeiras amostras e do quarto texto como apoio para listas. Participação recebida: 01/02 escritos pelo autor; 03 escrito pelo autor com ajuda de IA no contexto e palavras para Portugal; 04 formatado pela IA com termos ajustados pelo autor. Origem do conteúdo anterior à formatação de 04 não detalhada.

**Conferido / resultado:** síntese relida contra a resposta, sem atribuir IA às amostras 01/02 ou autoria exclusivamente humana ao texto 04. Autor considera o conjunto suficiente; não foram exigidas novas amostras. D02-09 atendida no recorte, D02-04 parcialmente definida; T02-003 em execução até escolha explícita da variante. Nenhum texto do piloto aprovado por essa escolha de referências.

**Preservação / limites:** spec v0.12 e tasks v0.7 preservadas com hashes iguais em `spec editorial/historico/2026-10-15-antes-da-confirmacao-de-voz/`. Amostras não alteradas. Conferência pela mesma IA, com histórico; reconhecimento das referências recebido do autor, sem avaliação do futuro texto. Plano v0.1 continua aplicável.

### T02-003 — fechamento da referência de voz — 2026-10-15

**Executado / evidência:** registrada a resposta autoral “portugues brasileiro mesmo” na spec v0.14 e consolidada a orientação com a combinação de amostras já aceita.

**Conferido / resultado:** critério de T02-003 relido integralmente: origem e participação conhecida de IA identificadas; trechos e características examinados; combinação reconhecida pelo autor; variante e direção de humor definidas; limites e escolhas não recebidas explicitados. Resultado atende à preparação da referência de voz; T02-003 concluída. R02-03 tem evidência utilizável, a ser retomada no parecer final de T02-007. T02-004 continua pendente por depender também de T02-002. Não houve redação ou aprovação do piloto.

**Responsável / preservação:** mesma IA responsável pelo registro, com acesso ao histórico; a escolha de variante e das referências veio do autor. Spec v0.13 e tasks v0.8 preservadas com hashes iguais em `spec editorial/historico/2026-10-15-antes-do-fechamento-de-voz/`. Amostras mantidas intactas. Plano v0.1 aplicável.

### T02-002 — estudo e evolução do processo — 2026-10-15

**Executado / evidência:** RA02-08 registrado na spec v0.15 a partir do retorno sobre início do estudo de engenharia junto com o desenvolvimento, experiência prática maior que a base teórica, uso inicial intenso de vibecoding e incorporação de regras, harness, skills, MCP, testes, “ssd”, TDD e BDD nos últimos dez meses aproximadamente.

**Conferido / resultado:** síntese confrontada com a resposta, preservando a falta teórica ainda atual. Não se inferiu domínio dos métodos, data exata, ordem individual de adoção ou resolução definitiva da lacuna. “ssd” permanece identificado como termo a confirmar antes de uso técnico. Há contexto suficiente para discutir um recorte de abertura; exposição dos nomes/percurso ainda precisa de confirmação. T02-002 em execução; próxima pergunta focaliza D02-06, sem prolongar o levantamento da história completa. Diagnóstico de competências não é exigido se o recorte não alegar essas competências.

**Responsável / preservação:** mesma IA responsável pela edição, com acesso ao histórico; relatos não validados tecnicamente. Spec v0.14 e tasks v0.9 preservadas com hashes iguais em `spec editorial/historico/2026-10-15-antes-da-jornada-de-estudo/`. Plano v0.1 continua aplicável, sem alteração de requisitos ou estratégia.

### T02-002 — exposição e fechamento do recorte factual — 2026-10-15

**Executado / evidência:** RA02-09 e delimitação factual registrados na spec v0.16. Autor autorizou Sampa TI e PDV D+ e informou exposição anterior no LinkedIn. Nenhuma publicação foi efetuada ou canal do piloto escolhido por essa resposta.

**Conferido / resultado:** critério integral de T02-002 confrontado com RA02-01 a RA02-09: intenção atual e lacuna teórica confirmadas; MVP individual, emissão em homologação e decisão seguinte relatados; duração aproximada recebida; nomes consultados autorizados. Diagnóstico abrangente, datas exatas, terceiros, comparação técnica e explicação das metodologias excluídos do recorte de apresentação da origem/intenção. T02-002 concluída nesse limite; mudança de promessa em T02-004 exige reexaminar a base afetada. R02-02 tem evidência para o recorte, não validação técnica. T02-004 iniciada para discutir leitor e contribuição, com demais condições ainda abertas.

**Responsável / limites / preservação:** mesma IA com acesso ao histórico; autorização e relatos vieram do autor, sem verificação externa do LinkedIn ou da emissão. Spec v0.15 e tasks v0.10 preservadas com hashes iguais em `spec editorial/historico/2026-10-15-antes-da-exposicao-autoral/`. Plano v0.1 aplicável; piloto permanece em 03.

### T02-004 — público e contribuição — 2026-10-15

**Executado / evidência:** RA02-10 e decisão vigente de D02-02 registrados na spec v0.17. Público inclui pessoas com dúvidas/dificuldades que querem desenvolver com IA, tanto profissionais de TI quanto pessoas sem essa experiência. Contribuição: mostrar a necessidade de estudo para construir base, a partir do percurso declarado pelo autor.

**Conferido / resultado:** síntese relida contra a resposta. Bagagem técnica tratada como vantagem de partida na orientação autoral, sem garantia universal; nenhum currículo, prazo ou diagnóstico de competência inventado. D02-02 resolvida; T02-004 continua em execução pelas condições de uso ainda abertas. Proposta histórica de restringir o leitor a profissionais experientes não é a decisão vigente.

**Responsável / preservação:** mesma IA com histórico disponível. Spec v0.16 e tasks v0.11 preservadas com hashes iguais em `spec editorial/historico/2026-10-15-antes-da-definicao-do-leitor/`. Plano v0.1 aplicável. Nenhuma redação ou publicação do piloto realizada.

### T02-004 — início do registro — 2026-10-15

**Executado / evidência:** RA02-11 registrado na spec v0.18; plano ajustado para v0.2 antes da execução operacional. Reutilizados índice, método e modelo de sessão de `registro da autoridade/`; criada SS-2026-10-15-001 sobre organização efetivamente realizada e vinculada à ficha 01. Fontes e amostras preservadas; nenhuma história reescrita.

**Conferido / resultado:** prioridade de registrar antes de pesquisar/estudar representada na spec e na orientação. Conteúdo mínimo, IDs, destinos e vínculos compatíveis com o método; sessão distingue preparação documental de estudo técnico e resultado do produto. T02-004 concluída nesse recorte. D02-01/D02-03/D02-05/D02-07 definidas para iniciar registros, com condições do futuro texto explicitamente adiadas. T02-005 a T02-007 permanecem pendentes; não há fechamento da spec 02 ou liberação automática de 03.

**Procedimentos e limites:** `sdd-editorial-especificar` para prioridade, `sdd-editorial-planejar` para estratégia, `sdd-editorial-tarefas` para acompanhamento e `editorial-redigir` para o registro operacional, todos v0.1. Uso real delimitado não equivale a exercício controlado ou cobertura de todos os modos. Conferência pela mesma IA com acesso ao histórico; sem pesquisa, estudo técnico ou apreciação do piloto.

**Preservação:** spec v0.17, plano v0.1, tasks v0.12, índice do registro e ficha 01 preservados com hashes iguais em `spec editorial/historico/2026-10-15-antes-do-inicio-do-registro/`. Alterações anteriores e staging mantidos.

**Conferência final da rodada:** sete documentos ativos examinados na navegação, com 96 referências locais e nenhum destino ausente; `git diff --check` sem erros. Sessão relida contra o pedido e o método: atividade de organização, fontes, limites e próximo passo identificados; nenhuma pesquisa ou aprendizagem técnica atribuída ao autor. Conferência documental, sem prova de utilidade futura ou aceitação do piloto.

## 5. Pendências e exercícios

| Origem | Tarefas afetadas | Responsável / momento | Situação |
| --- | --- | --- | --- |
| A02-02/A02-03; D02-06/D02-08 | T02-002/T02-004/T02-007. | Retornos RA02-01 a RA02-09 e delimitação na spec v0.16. | Resolvida no recorte preparatório de origem/intenção; aspectos técnicos e exposição adicional exigem reconferência se incluídos. |
| A02-04; D02-04/D02-09 | T02-003/T02-004/T02-007. | Autor confirmou referências, participação conhecida de IA e português brasileiro; spec v0.14. | Resolvida para a preparação do recorte; reconhecimento da voz no piloto será avaliado em 03. |
| D02-02 | T02-004/T02-007. | Público e contribuição definidos pelo autor em RA02-10; spec v0.17. | Resolvida; leitor inclui pessoas com e sem experiência em TI. |
| D02-03/D02-07 | T02-004/T02-005/T02-007. | RA02-16, spec v0.26 e plano v0.9. | Resolvidas: extensão livre/proporcional e prontidão para leitura autoral definidas. |
| A02-05; D02-10 | T02-005/T02-006/T02-007. | Matriz RA02-16 e EX02-A/B. | Resolvida no recorte; complementos conferidos, limites e gatilhos de reavaliação recebidos por 03. |

EX02-A/B foram definidos, executados e conferidos, complementando a [cobertura histórica](../../avaliacoes/T01-016/README.md). Entradas/critério, saídas e pareceres estão vinculados no registro de fechamento. Material sintético permanece separado das vivências do autor; limitações de uso real continuam em 03.

## 6. Cobertura e retomada

| Entrega | Tarefas | Cobertura prevista |
| --- | --- | --- |
| ENT02-01 | T02-001/T02-002. | Inventário conferido, confirmação factual e exposição. |
| ENT02-02 | T02-003. | Seleção, análise e retorno sobre referências de voz. |
| ENT02-03 | T02-004. | Decisões sobre recorte e condições de uso. |
| ENT02-04 | T02-005/T02-006. | Seleção fundamentada e complementação necessária conferida. |
| ENT02-05 | T02-007. | Parecer sobre os cinco critérios e versão de passagem. |

**Revisão da decomposição:** conferida documentalmente contra o plano v0.1; entregas, dependências e critérios cobertos. Não comprova execução.

**Próximo trabalho:** selecionar 03 e elaborar seu plano/tasks, recebendo a preparação conferida. Ficha, artigo/chamada e apreciação pertencem ao piloto; estudo técnico, Pages e publicação não foram executados.

**Situação da iniciativa:** encerrada em concluida; preparação suficiente no recorte. Piloto 03 permanece em backlog, sem execução.

## 7. Histórico

| Versão / data | Alteração | Base |
| --- | --- | --- |
| 0.1 — 2026-10-14 | Decomposição inicial conferida; sete tarefas pendentes e abertura registrada, sem execução retroativa das análises históricas. | Spec 02 v0.6 e plano 02 v0.1. |
| 0.2 — 2026-10-14 | T02-001 concluída com inventário e perguntas; T02-002 iniciada, aguardando confirmação; demais tarefas pendentes. | Spec 02 v0.7 e plano v0.1, com impacto da atualização examinado. |
| 0.3 — 2026-10-14 | Primeiro retorno autoral registrado e conferido; T02-002 permanece em execução. Condução por perguntas curtas e história completa adiada. | Spec 02 v0.8; plano v0.1 permanece aplicável. |
| 0.4 — 2026-10-14 | Motivos registrados em RA02-05 e conferidos; T02-002 continua em execução, com pergunta sobre participação do autor como próxima ação. | Spec 02 v0.9; plano v0.1 permanece aplicável. |
| 0.5 — 2026-10-14 | Sequência da busca fiscal registrada em RA02-06 e conferida; primeiro passo e participantes ainda por esclarecer. | Spec 02 v0.10; plano v0.1 permanece aplicável. |
| 0.6 — 2026-10-14 | MVP individual, emissão em homologação e decisão seguinte registrados em RA02-07; confirmação parcial de história, sem validação técnica do resultado. | Spec 02 v0.11; plano v0.1 permanece aplicável. |
| 0.7 — 2026-10-15 | T02-003 iniciada com análise de quatro amostras já existentes, preservadas; preferências e participação de IA aguardam retorno. | Spec 02 v0.12; plano v0.1 permanece aplicável. |
| 0.8 — 2026-10-15 | Combinação das referências e participação conhecida de IA recebidas e conferidas; D02-09 atendida no recorte; variante ainda pendente em T02-003. | Spec 02 v0.13; plano v0.1 permanece aplicável. |
| 0.9 — 2026-10-15 | Português brasileiro confirmado; referência consolidada e T02-003 concluída após conferência de seu critério. | Spec 02 v0.14; plano v0.1 permanece aplicável. |
| 0.10 — 2026-10-15 | RA02-08 liga estudo e desenvolvimento e registra cerca de dez meses de evolução com lacuna teórica persistente; próxima confirmação é de exposição. | Spec 02 v0.15; plano v0.1 permanece aplicável. |
| 0.11 — 2026-10-15 | Uso dos nomes autorizado em RA02-09; T02-002 concluída no recorte factual delimitado; T02-004 iniciada para discutir leitor e finalidade. | Spec 02 v0.16; plano v0.1 permanece aplicável. |
| 0.12 — 2026-10-15 | Público e contribuição recebidos em RA02-10; D02-02 resolvida, sem restringir a profissionais de TI; condições de uso ainda abertas. | Spec 02 v0.17; plano v0.1 permanece aplicável. |
| 0.13 — 2026-10-15 | Prioridade de iniciar registro recebida em RA02-11; estratégia ajustada, sessão operacional criada e T02-004 concluída nesse recorte. | Spec 02 v0.18 e plano v0.2; etapas de procedimentos/suficiência continuam pendentes. |
| 0.14 — 2026-10-15 | Correção de escopo autorizada: primeira publicação como foco; T02-004 reaberta e decisões vigentes reconciliadas. | Spec v0.19 e plano v0.3; evidência operacional anterior preservada, sem valer como prontidão editorial. |
| 0.15 — 2026-10-15 | Estudo de canais e formatos registrado, com fontes oficiais consultadas e recomendação identificada como proposta. | Spec v0.20 e plano v0.3; T02-004 permanece em execução. |
| 0.16 — 2026-10-15 | Estratégia autoral e primeira publicação com artigo/chamada confirmadas; GitHub pretendido e Pages opcional registrados. | Spec v0.21 e plano v0.4; T02-004 em execução, sem publicação ou infraestrutura criada. |
| 0.17 — 2026-10-15 | Textos na jornada e estudos em `capitulos estudos/` definidos; destinos futuros e revisões da primeira publicação registrados. | Spec v0.22 e plano v0.5; T02-004 aguarda extensão e prontidão. |

### T02-004 — destinos locais — 2026-10-15

**Executado / evidência:** RA02-13 na spec v0.22 e destinos no plano v0.5. Conferidas as pastas existentes `jornada do heroi/` e `capitulos estudos/`; definidos caminhos futuros de ficha/artigo/chamada com revisões, preservando texto-base e fontes.

**Conferido / resultado:** orientação corresponde ao retorno; não criada pasta antiga, artefato de 03, pesquisa ou migração. D02-05 definida para a primeira publicação; extensão e prontidão ainda pendentes em T02-004. Mesma IA responsável pelo registro, com histórico disponível. Spec v0.21, plano v0.4 e tasks v0.16 preservados com hashes iguais em `spec editorial/historico/2026-10-15-antes-dos-destinos-editoriais/`.

### T02-004 — escolha de canais e formatos — 2026-10-15

**Executado / evidência:** RA02-12 na spec v0.21 e estratégia correspondente no plano v0.4. Aceitos artigo no LinkedIn com chamada para primeira publicação/textos maiores, post único para atualizações, Substack com chamada no LinkedIn para estudos documentados futuros, GitHub como acervo e Pages ou links como opção de apresentação/acompanhamento.

**Conferido / resultado:** síntese relida contra o retorno. Pages tratado como opcional; GitHub como destino pretendido, sem alegar sincronização/visibilidade; estudo técnico adiado. Decisão não foi convertida em publicação autorizada ou criação de contas/site. T02-004 permanece em execução por arquivos, extensão e prontidão. O planejamento futuro de 03 deverá receber dois artefatos: artigo e chamada.

**Preservação / limites:** spec v0.20, plano v0.3 e tasks v0.15 preservados com hashes iguais em `spec editorial/historico/2026-10-15-antes-da-estrategia-de-publicacao/`. Mesma IA com histórico disponível; nenhuma verificação de conta ou implantação realizada.

### T02-004 — estudo de canais — 2026-10-15

**Executado / evidência:** releitura de `registro da autoridade/CANAIS_E_AUTORIDADE.md` e consulta pública a quatro páginas oficiais do LinkedIn/Substack, ligadas na seção “Estudo de canais e formatos” da spec v0.20. Comparadas plataformas e formatos; recomendação artigo no LinkedIn com post de apresentação identificada como proposta, com alternativa de post único.

**Conferido / resultado:** capacidades separadas da avaliação editorial. Não foram inferidos alcance, vantagem algorítmica, preferência autoral, publicação autorizada ou disponibilidade de recursos na conta. Comparação disponível para a decisão; T02-004 em execução. Nenhuma pesquisa técnica ou redação do piloto realizada.

**Responsável / preservação:** mesma IA com histórico disponível. Spec v0.19 e tasks v0.14 preservadas com hashes iguais em `spec editorial/historico/2026-10-15-antes-do-estudo-de-canais/`. Plano v0.3 aplicável; conjunto artigo/post só entra na execução de 03 depois de escolha e planejamento próprios.

## 8. Reabertura por correção de escopo — 2026-10-15

**Origem e ação:** análise apresentada ao autor e correção autorizada por “ok continue”. Spec v0.19 → plano v0.3 → tasks v0.14 reconciliados nessa ordem. Cinco entregas, R02-01 a R02-05 e IDs das tarefas preservados.

**Evidência invalidada para a publicação:** conclusão de T02-004 na v0.13, baseada no registro operacional SS-2026-10-15-001. A sessão continua sendo registro real; não demonstra finalidade, canal, formato ou versões da publicação. T02-004 retorna a em execução. T02-001 a T02-003 não dependem desse erro e permanecem mantidas em seus limites.

**Dependentes:** T02-005/T02-006/T02-007 permanecem pendentes até recorte e percurso pertinentes. O arquivo de entrada do complemento operacional em `spec editorial/avaliacoes/T02/01-complemento-registro-operacional.md` não tem saída/conferência e não conta como avaliação executada; não será usado para concluir T02-006 da publicação.

**Preservação e limites:** versões de partida copiadas com hashes iguais para `spec editorial/historico/2026-10-15-antes-da-correcao-de-escopo-02/`. Nenhum registro, fonte ou exercício excluído; staging anterior preservado. Conferência pela mesma IA autora com histórico disponível, sem redação, pesquisa técnica ou publicação. Próximo resultado necessário: condições da publicação registradas e conferidas em T02-004.

## Reconciliação v0.18 — 2026-10-16

**Executado:** síntese atual da spec v0.23, plano v0.6 e spec 03 v0.4 reconciliados com RA02-14. Artigo e chamada previstos sob `registro da autoridade/publicacoes/01-novo-mundo-bagagem-antiga/`, vinculados ao índice e às fontes; nenhuma peça nova produzida. Destino anterior preservado como histórico.

**Conferência:** canais, leitor, voz, fatos e limites comparados com decisões já registradas; as pendências atuais são extensão/prontidão (T02-004), procedimentos/cobertura (T02-005/T02-006) e suficiência (T02-007). Guia v0.6 e ficha v0.2 exigem confronto da interface atual em T02-005, sem alegar nova cobertura sintética. T02-001 a T02-003 mantidas no recorte; T02-004 em execução e demais pendentes. Mesma IA com acesso ao histórico. Preservação e conferência transversal nas tasks 04; estudo técnico e piloto não executados.

## Ajuste de clareza v0.18.1 — 2026-10-16

**Executado:** aplicada a autorização do autor após a nova análise de coerência. AGENTS.md recebeu o caminho `.obsidian/` e sua função opcional de apoio à navegação; Markdown, índices e acompanhamento SDD continuam como fontes editoriais. ENT02-03 no plano v0.6.1 e T02-004 nesta versão identificam v0.19 como origem histórica, mantendo spec v0.23 como base vigente. Atualizados apenas os rótulos dos documentos associados na spec.

**Conferência e preservação:** comparação com as cópias anteriores em `spec editorial/historico/2026-10-16-antes-do-ajuste-obsidian/`, com manifesto SHA-256; referências locais dos quatro documentos e `git diff --check` conferidos. Configurações `.obsidian/` e staging preservados. Mesma IA com acesso ao histórico; revisão documental dirigida, sem nova validação editorial ou autoral.

**Limites e próximo passo:** nenhum requisito, estado de tarefa ou critério de prontidão alterado. T02-004 continua em execução por extensão e prontidão da primeira publicação; piloto e estudo técnico não executados.

## Integração da direção pessoal — v0.19 / 2026-10-16

**Executado:** RA02-15/spec v0.24 registrada antes da atualização do plano v0.7. Reconciliados AGENTS, README, jornada/universo, entrada de estudos/base do livro, método/acervo/modelos, guia v0.7, ficha v0.3, skills preparar/redigir/revisar v0.2 e spec 03 v0.5. T02-003 recebeu reconferência documental da preferência explícita, preservando amostras e limites.

**Critérios:** identidade pessoal em primeira pessoa; humor/retórica/cotidiano autorizados sem fatos inventados; capítulos legíveis independentemente da autobiografia; organização pessoal apoiada por SDD; tom profissional restrito às finalidades pertinentes. Revisão dirigida pela mesma IA com acesso ao histórico, sem parecer independente. Fontes, transcrições, amostras e corpos de publicações anteriores permanecem intactos; PUB-000 exige reconferência de voz antes de reutilização.

**Preservação:** cópias anteriores e manifesto em `spec editorial/historico/2026-10-16-antes-da-direcao-pessoal/`. Conferência final de links, versões e diff registrada no manifesto.

**Limites e retomada:** alteração documental não comprova comportamento das skills nem voz reconhecida. T02-004 segue em execução por extensão/prontidão; T02-005 selecionará contratos e cobertura atuais; T02-006/T02-007 pendentes. Novos detalhes pessoais serão coletados conforme o texto exigir, sem questionar novamente a direção já decidida. Piloto não executado.

## Fechamento — v0.21 / 2026-10-16

**T02-004:** retorno autoral literal registrado em RA02-16; extensão livre, proporcional à história. Critérios de entrega para leitura autoral, recorte e limites consolidados; canais e direção de voz não foram perguntados novamente.

**T02-005:** percurso completo proporcional para artigo, ficha curta vinculada para chamada; modos/perfis e versões confrontados com E01–E07. Justificada a seleção de EX02-A/B e a dispensa de modos fora do recorte. Não imposta entrevista adicional sobre família ou pet.

**T02-006:** [entradas e critérios r01](../../avaliacoes/T02/02-complementos-voz-e-artigo/01-entradas-e-criterios.md) salvos antes das [saídas r01](../../avaliacoes/T02/02-complementos-voz-e-artigo/02-fichas-e-redacao.md); [pareceres, integração r02 e conferência](../../avaliacoes/T02/02-complementos-voz-e-artigo/03-pareceres-e-integracao.md) atendem A1–A6/B1–B7. Cenário fictício distinto do piloto. D1 é proposta defeituosa deliberada, recusada; não falha omitida da skill.

**T02-007:** R02-01 a R02-05 confrontados com as decisões, fontes e saídas efetivas. Parecer suficiente para preparar 03, com destino de cada pendência na spec v0.26. Não foi preciso mudar requisitos do método. Sem apreciação humana da voz ou prova de eficácia geral; mesma IA com histórico e critérios disponíveis.

**Preservação:** versões anteriores em `spec editorial/historico/2026-10-16-antes-do-fechamento-02/`, manifesto de hashes e conferência final. Staging preservado. A movimentação para concluida atualiza links sem reescrever o histórico das decisões. A próxima tarefa é planejar 03, que continua sem plano/tasks e sem artefatos reais produzidos.
