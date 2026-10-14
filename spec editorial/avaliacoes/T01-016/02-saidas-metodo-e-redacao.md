# Saídas dos exercícios E01 a E05

Execução de 2026-10-14. Entradas e condições em [01-entradas-e-criterios.md](01-entradas-e-criterios.md). Todas as entidades abaixo pertencem ao exercício, sem efeito sobre decisões editoriais reais.

## E01 — análise da spec sintética v0.1

Procedimento: `sdd-editorial-especificar` v0.1, analisar e revisar consistência.

ACH-01, impeditivo: “exatamente 100 palavras” contradiz “no máximo 60 palavras” para o mesmo texto. É preciso escolher uma extensão ou atribuir os limites a entregas diferentes. Ganho: critério executável; possível perda: uma das intenções de extensão precisará ser revista. A decisão pertence ao solicitante.

ACH-02, proposta: o narrador dragão foi apresentado como possibilidade, não como regra. Manter a alternativa em aberto preserva a escolha; defini-la agora restringiria a voz sem autorização.

Resultado: necessita ajustes antes de planejar a redação. Spec original preservada. Análise encerrada sem elaborar entregas de fases seguintes.

## E02 — plano sintético v0.1

Procedimento: `sdd-editorial-planejar` v0.1, elaborar. Base: spec sintética v0.2 do cenário E02; não é continuação aprovada de E01.

| Entrega | Requisito | Procedimento e critério | Dependência |
| --- | --- | --- | --- |
| EX-ENT-A: modelo de registro, caminho proposto `exercicio/modelo.md` | REQ-A | Elaborar campos fonte/data e conferir se permitem identificar a origem e a data do registro. | Nenhuma escolha de canal. |
| EX-ENT-B: ficha, caminho proposto `exercicio/ficha.md` | REQ-B | Preparar campos; finalizar e conferir destino/formato após receber a escolha. | Escolha do canal pelo autor antes da finalização. |

Os caminhos são propostas do cenário; nenhum desses arquivos foi criado. Não há dependência circular nem obrigação de aguardar o canal para preparar EX-ENT-A. Pendente DEC-A: canal, responsável autor, necessária para fechar EX-ENT-B. Revisão do plano: cobertura dos dois requisitos e dependências explícitas; apto para decomposição, com a dependência preservada. Sem escolha presumida de plataforma ou frequência.

## E03 — decomposição e acompanhamento simulado

Procedimento: `sdd-editorial-tarefas` v0.1, decompor, acompanhar e conferir. Base: E02/plano v0.1.

| ID sintético | Entrega | Conclusão exigida | Estado inicial |
| --- | --- | --- | --- |
| EX-T01 | EX-ENT-A | Modelo com fonte/data, seguido de conferência identificada. | Pendente. |
| EX-T02 | EX-ENT-B | Ficha com destino definido e conferido. | Bloqueada para finalização por DEC-A; preparação dos campos possível. |

Linha do tempo de EX-T01, baseada exclusivamente nos eventos fornecidos:

1. Modelo r01 criado: produzida/aguardando conferência. Arquivo existente não demonstra critério atendido.
2. Conferência de r01 verificou fonte/data: concluída no cenário, com evidência fornecida pelo enunciado, não por inspeção real de arquivo.
3. Edição r02 removeu fonte: reaberta, em execução. A conferência de r01 permanece no histórico, mas não valida r02. Restaurar o campo e reconferir antes de concluir. Impacto em EX-T02: se usar o modelo r02, verificar também o campo de origem; não declarar esse uso sem evidência.

## E04 — ficha EX-TXT-A / f01

Procedimento: `editorial-preparar` v0.1, ficha curta. Percurso leve: uma nota curta com uma fonte e uma ressalva, sem arco completo de episódio.

- Intenção/leitor: mostrar a iniciantes o que uma observação pequena permite afirmar.
- Destino/formato: nota interna de treino, até 150 palavras, conforme C1 fictício. Sem data de publicação.
- Base: S1, no arquivo de entradas. Regra lida antes das três apresentações de A; resultado de uma entrada; nenhum outro caso observado.
- Voz: primeira pessoa, português brasileiro, humor discreto; fragmento “Sem fanfarra.” permitido por C1. Fidelidade à voz do usuário não avaliada, pois não há amostras reais.
- Liberdade: imagem breve de contagem; não inventar emoção, fracasso ou diálogo.
- Organização proposta: dúvida inicial → regra e observação → limite da conclusão.
- LAC-01: motivo pessoal não registrado. Pergunta ao autor fictício: “O que levou você a começar esse estudo?” Permite rascunho sem esse trecho; se o motivo virar a promessa central, será necessário responder antes de redigir essa parte.
- Revisões pertinentes ao pequeno texto: P02, P07 e P09; C1 orienta preservação da voz. Outros perfis serão exercitados separadamente em D1, sem impor nove leituras a esta nota.

Conferência: base suficiente para rascunho com pendência delimitada. Sem inventar resposta a LAC-01. Fatos e ressalva devem acompanhar a redação.

## E05 — esboço e rascunho EX-TXT-A / r01

Procedimento: `editorial-redigir` v0.1, esboçar e redigir. Base: f01; pedido E05 retira motivação do escopo do texto, mantendo LAC-01 na ficha.

Esboço: não saber tratar a repetição; ler a regra local; observar A três vezes e uma entrada; terminar com o alcance limitado do exercício.

### Texto r01 — preservado

Antes de ler a regra, eu não sabia o que fazer com um identificador repetido. A instrução da lista de treino era manter uma única entrada por identificador. Apresentei A três vezes. No fim, havia uma entrada A.

Sem fanfarra. Três apresentações, uma entrada: foi o que observei nessa lista. Ainda não testei outros identificadores ou situações. Esse pequeno resultado não é uma garantia para outros casos.

### Entrega

Rascunho identificado, dentro do limite de C1. A repetição da contagem no segundo parágrafo faz a ponte para a ressalva; pode ser apreciada na leitura, sem obrigação de cortá-la. Não há derrota, motivo pessoal ou emoção acrescentados. A interpretação continua limitada a S1. Leitura inicial do redator não equivale a revisão independente. LAC-01 continua na ficha e não impede este escopo reduzido.
