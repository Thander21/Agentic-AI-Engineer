# Preparação editorial — CAP-10: Execução, runtime e memória

**ID:** FIC-CAP-10 (anteriormente FIC-CAP-01). **Revisão:** r03 — 19/10/2026. **Origem:** estudo.
**Contrato:** pedido “ok inicie” para a preparação delimitada do CAP-10 (antigo CAP-01), após recomendação de selecionar pergunta, ambiente e fontes. Preparar não autoriza redigir o capítulo ou executar experiências.
**Acompanhamento:** [mapa de estudos](../MAPA_DE_ESTUDOS.md#acompanhamento-e-vínculos). **Base:** [orientação do livro](../BASE_DO_LIVRO.md) e [S01/Parte V](../README.md#1-visão-geral-das-partes).

## Intenção e recorte

**Pergunta central proposta:** quando uma função chama outra e cria um objeto, o que precisamos compreender sobre execução, stack, heap e gerenciamento de memória para explicar a vida desse objeto e os limites dessa explicação?

**Leitor:** pessoa que usa IA para produzir código e precisa compreender o que acontece durante a execução. Ponto de partida declarado pelo autor em 18/10/2026: não consegue explicar runtime, stack, heap ou coleta de lixo; consegue avaliar “chamadas, ifs, funções, waits”. É autodeclaração, sem diagnóstico por exercício. “Waits” foi mantido como termo do autor; não presume domínio de `await`, assincronismo ou concorrência. Não pressupor equivalência entre bagagem de TI e domínio desses conceitos.

**Contribuição pretendida:** construir um modelo inicial de chamadas, objetos, referências e memória, distinguindo explicação conceitual, descrição do runtime e observação de um caso. É preparação técnica; não há cena autobiográfica necessária.

**Formato/tom:** nota de estudo inicial que poderá alimentar capítulo técnico autônomo, em português brasileiro, com termos explicados e sem exigir leitura da jornada. Canal público, extensão final e publicação não definidos nesta entrega.

**Incluído:** papel do runtime; chamadas e retorno; stack versus heap no ambiente selecionado; referências, alcançabilidade e gerenciamento de memória; limites de inferir comportamento a partir de código ou gráfico.

**Fora deste recorte:** concorrência, threads e I/O de CAP-02; profiling aprofundado de CAP-04; diagnóstico de vazamento do ERP; comparação abrangente entre linguagens; arquitetura de aplicação. Não acrescentar código, scripts ou ferramentas ao repositório para organizar o estudo.

## Ambiente escolhido e caso de preparação

**Decisão autoral — 18/10/2026:** Dart no desktop. Para adequar o recorte ao ponto de partida, a preparação usa como caso didático um fluxo síncrono de chamadas, condição e retorno, acrescentando um objeto referenciado após apresentar objeto e referência. Essa seleção didática não é uma experiência já realizada. Flutter, interface gráfica, acesso a dados e código de produção são dispensáveis.

**Profundidade inicial:** partir da leitura de fluxo familiar e introduzir runtime, quadro de chamada, objeto, referência, heap e coleta de lixo com definições e limites. Não exigir conhecimento prévio desses conceitos. O primeiro caso dispensa `await`; assincronismo terá preparação própria quando necessário. A identificação de chamadas não comprova compreensão de stack ou gerenciamento de memória.

Identificar versão do SDK, sistema operacional e modo de execução antes de qualquer observação prática. Não foi executado Dart ou DevTools, nem inspecionado projeto externo. A versão instalada é desconhecida. Não generalizar detalhes da VM para Dart Web ou outras linguagens.

## Fontes para o recorte introdutório

Consultadas em 18/10/2026 para delimitar a opção Dart; páginas vivas, sem correspondência ainda com SDK local. Ambiente agora confirmado. TEC01-01/02 e TEC01-04/05 sustentam a preparação introdutória; TEC01-03 permanece aprofundamento candidato, sem detalhes internos liberados para uso como afirmações do capítulo.

| ID | Fonte e trecho selecionado | Contribuição e limite |
| --- | --- | --- |
| TEC01-01 | [Dart overview](https://dart.dev/overview), “Dart: The platforms”, “Dart Native” e “The Dart runtime” | Distingue plataformas, compilação e responsabilidades do runtime. Fonte de visão geral; não prova disposição física de cada variável na memória. |
| TEC01-02 | [Use the Memory view](https://docs.flutter.dev/tools/devtools/memory), “Basic memory concepts”, “Root object, retaining path, and reachability” e “Memory leaks happen in Dart?” | Candidata para objetos, alcançabilidade e retenção; separa conceitos da ferramenta. Não foi feita observação de alocações ou teste de vazamento. |
| TEC01-03 | [Dart VM — Garbage collection](https://github.com/dart-lang/sdk/blob/main/runtime/docs/gc.md), documento de implementação no ramo main | Aprofundamento candidato da VM, dependente de versão. Antes de usar detalhes como afirmação didática, selecionar revisão imutável compatível e trecho exato. Não substitui apresentação inicial de stack e chamadas. |

| TEC01-04 | [Functions](https://dart.dev/language/functions), exemplo inicial, “The main() function” e “Return values”; consultada em 18/10/2026 | Base para entrada, chamada e retorno; selecionar apenas exemplos simples, sem exigir funções de ordem superior ou closures. Página viva, não teste de compreensão. |
| TEC01-05 | [Use the debugger](https://docs.flutter.dev/tools/devtools/debugger), “The call stack and variable areas” e “Stepping through source code”; consultada em 18/10/2026 | Base para apresentar chamadas ativas, quadros e variáveis observáveis. Não usar a visualização do debugger como prova do endereço físico ou localização de toda variável; nenhuma sessão de depuração foi executada. |

S01/F079 rastreia a origem do assunto na conversa; não é comprovação técnica. Não incorporar os exemplos históricos sem conferência própria.

## Evidência e critérios previstos

Resultado esperado do estudo: fluxo comentado de um caso pequeno, indicando chamadas/retornos, referências e o que sustenta a explicação de memória. Se houver observação futura, registrar ambiente, versão, procedimento, resultado e limite; uma previsão não será apresentada como medição.

Conferência técnica futura: cada afirmação importante deve ter fonte/trecho; não assumir que toda variável local ocupa uma posição fixa na stack ou que sair de uma função determina imediatamente uma coleta. O tratamento específico dessas questões depende da fonte de implementação e do ambiente aceito.

Conferência didática futura: apresentar os pré-requisitos necessários, permitir acompanhar o caso sem autobiografia e propor uma pergunta de transferência para outro caso. Resposta escrita pela IA não comprova compreensão do autor ou do leitor.

**Lacunas remanescentes e efeito:** ambiente e ponto de partida foram recebidos. SDK, sistema operacional, modo de execução e revisão imutável de TEC01-03 continuam desconhecidos; impedem afirmações específicas de implementação e relato de experimento, mas não uma explicação conceitual inicial apoiada em TEC01-01/02/04/05. Não usar descrições de implementação da VM nem números de memória até resolver essas lacunas. Uma dúvida concreta diante de código gerado por IA ainda não foi relatada; o caso será explicitamente didático, sem atribuir incidente ao autor.

**Conferência desta preparação:** aplicada editorial-preparar v0.4, com histórico do projeto disponível, sem revisão independente. Pergunta, recorte, fontes e critérios confrontados com CAP-01, a base do livro e o retorno de 18/10/2026. Fonte de chamadas/quadros complementada e profundidade ajustada à autodeclaração. Nenhuma nova entrevista é necessária para preparar o recorte conceitual. Não há estudo concluído, capítulo redigido ou aprendizagem comprovada. Prontidão e próxima ação ficam exclusivamente no mapa de estudos.
