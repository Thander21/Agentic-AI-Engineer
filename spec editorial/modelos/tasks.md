# Modelo de tasks editoriais

**Versão do modelo:** 0.1  
**Entrega de origem:** ENT-02 / T01-004  
**Orientação:** [Guia de operação](../GUIA_DE_OPERACAO.md) · [Modelo de plano](plano.md).

## Como usar este modelo

Copie a estrutura abaixo para as tasks da iniciativa. Preencha os campos entre chaves, ajuste os caminhos e remova estas instruções da cópia. Linhas demonstrativas não são trabalho executado. Use o plano revisado para decompor entregas em tarefas verificáveis; não crie requisitos novos nesta etapa.

Mantenha os IDs estáveis e use os mesmos IDs nas tabelas de definição e acompanhamento. Cada tarefa deve ter uma saída delimitada e um critério de conclusão. Resultados independentes podem ser separados; pequenas correções de uma mesma entrega podem permanecer juntas. Para iniciativas pequenas, reduza o número de linhas e de registros, preservando a rastreabilidade.

Este documento acompanha implementação e conferência. Reutilize pareceres e registros existentes por referência, sem copiá-los integralmente. A ausência de resultados no início deve permanecer explícita.

---

# Tasks — {nome da iniciativa}

**ID:** {identificação estável das tasks}  
**Versão:** {versão deste documento}  
**Data:** {data da atualização}  
**Spec de referência:** {ID, caminho e versão}  
**Plano de referência:** {ID, caminho e versão; localização do parecer para tasks}  
**Responsável pelo acompanhamento:** {pessoa ou IA/papel}  
**Estado geral:** tarefas em elaboração; execução não iniciada.

## 1. Escopo da execução

**Entregas previstas:** {IDs do plano e resumo do trabalho}.

**Base dos caminhos:** {pasta a partir da qual os caminhos relativos são interpretados}.

**Materiais existentes a preservar:** {fontes, registros e versões de partida}.

**Condições de início:** {dependências satisfeitas e decisões ainda necessárias; não presumir prontidão apenas pela existência dos arquivos}.

Mudanças de intenção ou requisitos retornam à spec. Mudanças de estratégia ou dependências retornam ao plano. Reconciliar as tarefas afetadas e registrar a nova base, sem renumerar ou apagar o histórico.

## 2. Definição das tarefas

| ID | Entrega / requisitos de origem | Dependências | Papel responsável | Resultado e caminho previsto | Critério de conclusão |
| --- | --- | --- | --- | --- | --- |
| T{iniciativa}-001 | {ENT e REQ do plano/spec} | {tarefas anteriores, fonte ou decisão externa} | {papel executor e responsável pela conferência, se diferente} | {artefato ou resultado observável; caminho quando pertinente} | {o que produzir, o que conferir e qual evidência registrar} |

Incluir atividades de conferência e retorno humano quando fizerem parte do plano. Uma tarefa pode conter produção e revisão, mas o acompanhamento precisa distinguir esses acontecimentos. Se a apreciação do autor for necessária para concluir a entrega, seu retorno não pode ser substituído por avaliação da IA.

## 3. Estados e regras de atualização

| Estado | Quando usar | Próxima ação |
| --- | --- | --- |
| Pendente | Ainda não começou; pode ter dependências futuras. | Conferir dependências e iniciar quando houver contexto e escopo autorizado suficientes. |
| Em execução | Trabalho efetivamente iniciado. | Produzir ou corrigir a saída e registrar o andamento relevante. |
| Produzida/aguardando conferência | Saída disponível, mas critério ainda não conferido integralmente. | Conferir a versão identificada e registrar resultado e limites. |
| Concluída | Critério atendido e evidência registrada, sem impeditivos abertos para a tarefa. | Preservar o resultado e liberar as dependências pertinentes. |
| Bloqueada com motivo | Uma tentativa de avanço encontrou impedimento concreto. | Registrar motivo, parte afetada, responsável pela resolução e condição de retomada. |

Uma dependência planejada para mais tarde não exige marcar bloqueio antes de tentar executar. Uma tarefa concluída pode ser reaberta: retorne ao estado adequado, explique a causa e preserve o resultado da conferência anterior com sua versão.

Estados das tasks não substituem maturidade do conteúdo, apreciação autoral ou publicação. “Texto revisado”, “autor avaliou” e “texto publicado” são registros distintos.

## 4. Acompanhamento atual

| Tarefa | Estado | Artefato / versão produzida | Conferência: versão, resultado e evidência | Pendências / próximo passo |
| --- | --- | --- | --- | --- |
| T{iniciativa}-001 | Pendente | Não produzido. | Não realizada. | {dependência ou primeira ação} |

Substituir os campos somente após os acontecimentos. Identificar caminhos reais e versões recuperáveis. Ao atualizar uma linha após correção ou reabertura, preservar a evidência anterior na seção 5. Se ainda não houve conferência, manter “não realizada”.

## 5. Registro de execução e conferência

Repetir o bloco abaixo por conferência relevante, ou referenciar um registro existente que contenha esses dados. Não criar um resultado fictício para preencher o modelo.

### {Tarefa} — {data / identificação do registro}

- **Base usada:** {versões de spec e plano, se diferentes das do cabeçalho; indicar o que mudou}.
- **Executado:** {ação realmente realizada, arquivo e versão produzida}.
- **Conferido:** {versão exata, critério examinado e como foi examinado}.
- **Evidência:** {trecho, caminho, parecer ou observação recuperável que sustenta o resultado}.
- **Resultado:** {atende / precisa de ajuste / não avaliado, por aspecto quando necessário}.
- **Achados e decisão:** {impeditivos, revisões necessárias e sugestões; resolução ou encaminhamento}.
- **Responsável e limites:** {quem conferiu, contexto disponível, acesso a pareceres anteriores e aspectos não avaliados}.
- **Efeito no acompanhamento:** {estado resultante, dependências liberadas ou tarefas reabertas}.
- **Próximo passo:** {ação concreta ou informação necessária}.

Produzir um arquivo ou receber resposta de ferramenta não demonstra, isoladamente, qualidade editorial. Conferência estrutural, exercício de comportamento, uso real e apreciação humana devem ser identificados pelo que efetivamente ocorreu. Uma revisão pela mesma IA autora não será apresentada como independente.

## 6. Pendências, bloqueios e reaberturas

| ID do registro | Tarefa afetada | Motivo / origem | Impacto e parte que pode continuar | Quem resolve / condição de retomada | Estado da pendência |
| --- | --- | --- | --- | --- | --- |
| {ID} | {tarefa} | {fato observado, parecer ou mudança na spec/plano} | {o que impede e o que não impede} | {pessoa, fonte ou entrega necessária} | {aberta / resolvida; referência à resolução} |

Ao reabrir, indicar qual evidência deixou de valer e por quê. Reconferir os aspectos afetados; não reiniciar toda a iniciativa por uma alteração localizada. Mudanças de sentido precisam da revisão pertinente mesmo quando a redação parece apenas mais fluida.

## 7. Exercícios de avaliação, quando previstos

Se o plano não exigir avaliação de comportamento, registrar “não se aplica” com motivo. Se exigir, usar os casos previstos e acrescentar apenas os necessários às dúvidas encontradas.

| Caso / tarefa | Procedimento, modo/perfil e versão | Entrada recuperável | Comportamento esperado | Resultado observado / saída | Evidência e limitações | Ajuste / reconferência |
| --- | --- | --- | --- | --- | --- | --- |
| {ID} | {skill ou procedimento} | {pedido exato e arquivos/versões usados} | {definido antes de examinar a saída} | {não executado até haver resultado real} | {onde conferir; contexto e modelo quando conhecido} | {ação necessária ou nenhuma identificada} |

Indicar quais modos ou perfis foram conferidos documentalmente, exercitados ou permanecem não avaliados. Um único exercício não valida toda a cadeia. Declarar quando o resultado esperado ou pareceres anteriores estavam disponíveis durante a execução. Não converter preferência literária em aprovação automática.

## 8. Cobertura e próximo trabalho

| Entrega do plano | Tarefas relacionadas | Cobertura do escopo e pendências |
| --- | --- | --- |
| {ENT-ID} | {IDs} | {confirmar que produção e conferência estão contempladas; indicar ausência se houver} |

**Revisão desta decomposição:** não avaliada. Após conferir vínculos, critérios, dependências e cobertura, registrar resultado e limites.

**Próxima tarefa executável:** {ID e justificativa pelas dependências; ou pendência que impede avançar}.

**Situação da iniciativa:** {o que está produzido, conferido e pendente; não declarar conclusão por quantidade de arquivos}.

## 9. Histórico do acompanhamento

| Versão / data | Alteração | Tarefas afetadas | Base e evidência relevante |
| --- | --- | --- | --- |
| {versão / data} | {decomposição, execução, correção ou reabertura} | {IDs} | {spec/plano/registro de conferência} |

Ao fechar a iniciativa, conferir os critérios do plano e as pendências humanas ou externas. Propostas futuras podem ficar registradas separadamente, mas requisitos ainda não atendidos não devem ser reclassificados como melhorias opcionais para simular conclusão.
