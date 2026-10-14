# Modelo de plano editorial

**Versão do modelo:** 0.1  
**Entrega de origem:** ENT-02 / T01-003  
**Orientação:** [Guia de operação](../GUIA_DE_OPERACAO.md) · [Modelo de spec](spec.md).

## Como usar este modelo

Copie a estrutura abaixo para o plano da iniciativa. Substitua os campos entre chaves, ajuste os caminhos ao destino e remova estas instruções da cópia. Linhas demonstrativas não são decisões nem entregas concluídas.

Parta de uma spec identificada e de seu parecer de prontidão. Se a spec tiver mudado depois da revisão, reconfira os pontos afetados antes de reutilizar o parecer. Planeje somente o escopo com contexto suficiente e explicite dependências futuras. Se o objetivo ou um requisito central continuar contraditório, devolva a questão à spec.

O plano decide como organizar as entregas. Análise e requisitos permanecem na spec; execução, estados e evidências ficam nas tasks. Dimensione o plano à iniciativa: não criar uma entrega por frase nem impor skills ou fases sem utilidade. Seções condicionais podem receber “não se aplica” com motivo.

---

# Plano — {nome da iniciativa}

**ID:** {identificação estável do plano}  
**Versão:** {versão deste plano}  
**Data:** {data da atualização}  
**Base:** {ID, caminho e versão da spec}  
**Parecer de origem:** {localização e versão examinada; situação das pendências relevantes}  
**Responsável:** {pessoa ou IA/papel}  
**Estado:** em elaboração  
**Tasks associadas:** {não geradas / caminho existente e versão}

## 1. Resultado e fronteiras da implementação

**Resultado pretendido:** {como as entregas materializam o objetivo da spec}.

**Escopo a executar:** {requisitos e frentes cobertos, sem introduzir objetivos novos}.

**Limites desta implementação:** {o que fica fora, com referência à spec; dúvidas de escopo retornam a ela}.

**Base disponível:** {artefatos existentes a reutilizar, com caminhos e versões; indicar os que precisam ser conferidos}.

## 2. Decisões de implementação

| ID | Escolha | Motivo e referência à spec | Consequência ou condição de revisão |
| --- | --- | --- | --- |
| DP-01 | {forma de organizar, produzir ou revisar} | {requisito/decisão de origem e justificativa} | {impacto e limite} |

Escolhas sobre caminhos, agrupamento de procedimentos e sequência pertencem ao plano. Uma alteração de intenção, público obrigatório ou regra central exige atualizar a decisão na spec e depois reconciliar este plano.

## 3. Entregas, locais e critérios

**Base dos caminhos:** {pasta a partir da qual os caminhos relativos são interpretados}.

| ID | Entrega e função | Saída / caminho previsto | Requisitos relacionados | Papel responsável | Critério de conferência |
| --- | --- | --- | --- | --- | --- |
| ENT-01 | {resultado verificável e sua utilidade} | {arquivo, conjunto de arquivos ou registro de resultado} | {IDs da spec} | {papel} | {como avaliar a entrega e qual evidência será registrada nas tasks} |

Identifique o que será criado, atualizado ou reaproveitado. Um caminho previsto não comprova a existência de um arquivo. Não criar links para arquivos inexistentes como se já fossem entregues. Conferência, retorno humano e publicação são acontecimentos distintos.

## 4. Sequência e dependências

| Ordem | Entrega | Depende de | Condição de início | Resultado necessário para liberar a próxima passagem |
| --- | --- | --- | --- | --- |
| {ordem} | {ENT} | {ENT anteriores, decisão externa ou nenhuma} | {o que precisa estar disponível} | {saída e conferência pertinente} |

Verifique se há dependências circulares ou referências a entregas não definidas. Se um procedimento estiver sendo criado pela primeira vez, descreva como o trabalho inicial será realizado sem depender da ferramenta ou modelo ainda inexistente. Possibilidades de trabalho paralelo não obrigam usar agentes simultâneos.

## 5. Procedimentos e contexto de execução

Preencha esta seção conforme a iniciativa. Se não houver criação de skills, registre apenas quais procedimentos existentes serão usados. Não transformar o plano de uma postagem em um projeto de novas skills.

| Procedimento ou skill | Situação de uso e modo | Entrada mínima | Saída e destino | Limite / retorno à etapa anterior |
| --- | --- | --- | --- | --- |
| {nome existente ou proposto} | {pedido a que responde} | {spec, ficha, fontes, versões ou contexto} | {artefato ou parecer} | {o que não decide e quando precisa de esclarecimento} |

**Referências compartilhadas:** {guias, modelos e fontes; indicar quando cada recurso é necessário}.

**Se houver skills novas:** definir agrupamento, caminhos dos pacotes, modo de acesso no ambiente, estrutura de referências e orientação de autoria aplicável. Distinguir pacote criado, recurso acessível e acionamento automático verificado. A descrição do procedimento não equivale a uma skill implementada.

**Passagem de contexto:** {quem entrega qual versão e quais informações ao próximo papel; como preservar fatos, ressalvas e pendências}.

## 6. Cobertura dos requisitos

| Requisito da spec | Entrega responsável | Como será conferido | Evidência esperada e momento |
| --- | --- | --- | --- |
| {REQ-ID} | {ENT-ID} | {critério adequado ao requisito} | {parecer, artefato, exercício observado ou retorno humano} |

Mapear todos os requisitos do escopo. Requisito sem entrega ou critério precisa ser resolvido antes de declarar o plano pronto. Se um requisito deixar de se aplicar, registrar a decisão na spec em vez de omiti-lo da cobertura. A tabela representa cobertura planejada, não atendimento comprovado.

## 7. Conferência das entregas

**Conferência documental:** {estrutura, fontes, coerência, linguagem, links e contratos pertinentes}.

**Avaliação de comportamento, se aplicável:** {situações representativas, entradas preservadas, resultados observáveis e limites da avaliação; não impor exercícios artificiais a uma simples edição}.

**Avaliação autoral ou de leitores, se necessária:** {aspectos que dependem de apreciação humana, quem participa e o que permanece pendente sem esse retorno}.

**Registro:** {como as tasks guardarão artefato/versão, resultado, evidência, achados e reconferência}.

**Encerramento:** {condições para concluir cada entrega e o conjunto, distinguindo produção, revisão, validação em uso e publicação}.

Skills e modelos podem estar estruturalmente corretos sem terem demonstrado utilidade. Pareceres devem apontar evidências e limites. Quando houver revisão literária, examinar trechos e efeitos sobre voz, clareza e ritmo; evitar transformar preferências em aprovação automática.

## 8. Pendências e dependências externas

| ID / origem | Informação ou decisão ausente | Entregas afetadas | Quem ou qual fonte resolve | Momento necessário | Efeito sobre o avanço |
| --- | --- | --- | --- | --- | --- |
| {PEN da spec ou referência} | {lacuna} | {ENT-IDs} | {autor, fonte ou outra iniciativa} | {antes de qual entrega; data apenas se definida} | {impede finalizar o plano / permite tasks mas impede iniciar entrega específica} |

Uma definição editorial ainda ausente pode impedir o piloto sem impedir a preparação de modelos genéricos. Explique essa distinção para cada pendência relevante, sem assumir a decisão nem bloquear partes independentes. Se faltar uma escolha indispensável à decomposição das entregas, resolva-a antes das tasks.

## 9. Revisão do plano e passagem às tasks

**Versão examinada:** {versão}  
**Revisor e contexto disponível:** {papel, referências e acesso ao histórico}  
**Limitações:** {o que não foi conferido ou não pode ser afirmado}.

| Achado | Entrega / trecho | Problema e importância | Decisão e correção | Situação / evidência |
| --- | --- | --- | --- | --- |
| RP-01 | {localização} | {problema e efeito na execução} | {alteração ou justificativa} | {aberto, resolvido ou encaminhado} |

Se não houver achados, registrar o resultado e seu escopo, removendo a linha demonstrativa. Não criar problemas fictícios para preencher a tabela.

**Parecer:** não avaliado. Após revisão, substituir por “apto para tasks” ou “necessita ajustes”, com fundamento.

**Conferir antes do parecer:** vínculo com a versão vigente da spec; entregas e caminhos definidos; requisitos cobertos; dependências possíveis; contexto e procedimentos suficientes; critérios proporcionais; pendências com destino e momento de resolução.

**Próximo passo:** {gerar tasks vinculadas a este plano ou resolver achados específicos}.

Prontidão para tasks não declara implementação nem validação do resultado. O documento de tasks deve permitir acompanhar produção e conferência separadamente, sem renumerar IDs já existentes.

## 10. Mudanças e impactos

| Versão / data | Alteração e motivo | Base da spec | Entregas e tasks afetadas | Reconferência necessária |
| --- | --- | --- | --- | --- |
| {versão / data} | {mudança} | {versão / requisito / decisão} | {IDs ou ainda não geradas} | {o que a mudança invalida ou nenhuma, com motivo} |

Manter decisões de estratégia neste plano e evidências de execução nas tasks. Se uma mudança afetar requisitos, atualizar primeiro a spec e registrar a nova base usada pelo plano.
