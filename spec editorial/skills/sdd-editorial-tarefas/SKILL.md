---
name: sdd-editorial-tarefas
description: Decompõe planos editoriais revisados em tasks e acompanha implementação, evidências, conferência e reabertura de tarefas existentes. Use para organizar ou atualizar a execução de uma iniciativa editorial com spec e plano identificados. Não use para definir requisitos iniciais, substituir o planejamento ou redigir automaticamente os artefatos das tarefas.
metadata:
  version: "0.1"
---

# Elaborar e acompanhar tarefas editoriais

Mantenha uma ligação verificável entre o trabalho previsto, o que foi produzido e o que foi efetivamente conferido. O documento de tasks concentra execução e evidências; a spec conserva intenção e regras, e o plano conserva estratégia e entregas.

## Escolher o modo pelo pedido

| Modo | Entrada mínima | Saída |
| --- | --- | --- |
| Decompor | Spec e plano identificados, com parecer suficiente para tasks. | Tarefas delimitadas, dependências, resultados e critérios de conclusão. |
| Acompanhar | Tasks existentes, base vigente, artefatos e evidências disponíveis. | Estados atualizados, resultados, pendências e próximo trabalho executável. |
| Conferir acompanhamento | Tasks, critérios e evidências referenciadas. | Achados de inconsistência e encaminhamento; correções somente quando incluídas no pedido. |

Uma solicitação de listar ou revisar tarefas não inicia sua execução. Se o pedido também autorizar implementação, encaminhe a produção à capacidade apropriada e mantenha estas regras de acompanhamento; esta skill não substitui procedimentos de autoria ou revisão especializados.

## Consultar referências e versões

- [Guia de operação](../../GUIA_DE_OPERACAO.md): consulte para fases, responsabilidades, estados e encerramento.
- [Modelo de tasks](../../modelos/tasks.md): use ao criar ou conferir o documento; preserve IDs e organização existente quando adequados.
- [Modelo de parecer](../../modelos/parecer-editorial.md): consulte quando a conferência exigir achados detalhados, sem impor outro arquivo.

Resolva caminhos a partir desta pasta e confirme a disponibilidade dos recursos. A skill depende do conjunto local; copiar só seu arquivo não garante acesso aos modelos. Declare referências ausentes e seu impacto, sem inventar conteúdo ou evidência.

Identifique versões de spec, plano e tasks. Se mudaram depois do parecer ou da execução, examine o impacto antes de reutilizar uma conclusão. Leia apenas os artefatos necessários ao escopo solicitado, preservando fontes e originais.

## Decompor o plano

1. Relacione todas as entregas do escopo às tarefas e aos requisitos de origem. Não introduza requisitos novos: dúvidas sobre intenção retornam à spec; mudanças de estratégia retornam ao plano.
2. Delimite cada tarefa por resultado verificável. Separe saídas independentes ou condições de conclusão diferentes; não crie uma tarefa para cada vírgula a corrigir nem uma única tarefa genérica para melhorar tudo.
3. Defina ID estável, entrega/requisitos, dependências, papel responsável, saída e caminho previsto, critério de conclusão, estado inicial e próximo passo. Na execução, acrescente versão produzida e conferida, evidência, resultado e limites.
4. Inclua produção e conferência nos critérios. Quando o retorno autoral for necessário, separe sua dependência de atividades já executáveis; não declare a entrega completa antes de recebê-lo.
5. Confira IDs de dependências, ciclos e cobertura das entregas. Uma dependência de informação externa deve indicar quem ou qual fonte a resolve e quando será necessária.
6. Use o mesmo ID na definição e no acompanhamento. Preserve IDs existentes, mesmo ao reorganizar a apresentação; novas tarefas recebem IDs novos.

Ao construir a própria metodologia, o primeiro documento pode ser elaborado manualmente a partir do contrato da spec e do plano. Não exigir que o modelo ou a skill ainda inexistente já tenham sido usados. Preveja sua reconciliação posterior sem reiniciar o histórico.

## Atualizar por evidências

| Estado | Condição |
| --- | --- |
| Pendente | Trabalho não iniciado, inclusive quando há dependências futuras. |
| Em execução | A atividade efetivamente começou. |
| Produzida/aguardando conferência | A saída existe, mas o critério ainda não foi integralmente conferido. |
| Concluída | Critério atendido, versão examinada e evidência registradas, sem impeditivo aberto para a tarefa. |
| Bloqueada com motivo | Uma tentativa de avanço encontrou impedimento concreto; motivo e condição de retomada estão registrados. |

Não inferir conclusão pela existência do arquivo ou por uma marcação anterior. Localize a versão e a conferência que sustentam o estado. Se só houver declaração não corroborada, registre a lacuna e solicite ou realize a conferência pertinente dentro do escopo autorizado.

Para cada atualização relevante, registre ação realizada, artefato e versão, critério examinado, resultado observado, evidência recuperável, responsável, limitações e próximo passo. Vincule registros extensos existentes em vez de copiá-los. Não reescreva uma conferência antiga como se tivesse examinado uma versão nova.

Se uma tarefa conclui somente construção documental, deixe explícito que comportamento ou uso real ainda serão avaliados em outra tarefa. Não extrapole um resultado estrutural de `SKILL.md` para qualidade da escrita ou decisões da skill.

## Tratar achados e reabertura

Encaminhe falhas ao ponto responsável: entrega para sua tarefa, estratégia para o plano, regra ou intenção para a spec. Quando uma alteração invalidar evidência anterior, registre motivo, versão afetada e aspecto a reconferir; retorne a tarefa ao estado adequado, preservando o histórico.

Examine dependentes quando o contrato ou resultado que utilizam mudar. Não reabra todas as tarefas indiscriminadamente nem ignore efeitos de uma mudança de sentido. Correções locais podem exigir apenas reconferência localizada.

Um impeditivo aberto impede concluir a tarefa afetada. Revisão necessária requer resolução ou justificativa explícita; preferência expressiva pode ser recusada com motivo. Não transferir requisito obrigatório para uma lista de melhorias futuras apenas para encerrar o trabalho.

Pendência futura não é automaticamente bloqueio atual. Registre quais partes independentes podem continuar e indique a próxima tarefa com dependências satisfeitas. A ausência de escolha de voz para um piloto não impede criar modelos genéricos.

## Registrar avaliações sem simular execução

Quando houver exercícios previstos, registrar pedido exato, entradas recuperáveis, procedimento/versão, modo ou perfil, comportamento esperado, saída observada, evidência e limites. Defina o esperado antes de examinar o resultado; um exemplo escrito na skill não é exercício realizado.

Distinga conferência documental, avaliação de comportamento, uso integrado e apreciação humana. Informe acesso a resultados esperados ou pareceres anteriores quando isso limitar independência. Não preencha tempos, modelo utilizado ou retorno humano por suposição.

Se uma avaliação detectar falha, encaminhe a correção e registre a reconferência pertinente. Cobertura parcial deve permanecer parcial; um exercício de língua não valida todos os perfis editoriais.

## Entregar o acompanhamento

Ao criar tasks, retire exemplos do modelo e confira caminhos, IDs, cobertura e dependências. Ao atualizar, registre versão e histórico relevantes. Não altere outros documentos silenciosamente quando o pedido estiver limitado ao acompanhamento.

Informe o que foi produzido, o que foi conferido, o que permanece pendente e qual tarefa pode começar. Conclusão das tasks não implica publicação, aprovação autoral ou capacidades além das evidências registradas. Se a conferência não ocorreu, mantenha essa ausência explícita.

## Exemplo de decisão — ilustrativo

Um rascunho foi salvo, mas ainda não recebeu revisão: registre produzido/aguardando conferência. Depois de uma conferência concluída, a conclusão factual do texto é alterada: preserve o resultado antigo, reabra a verificação afetada e indique a nova versão. Não declarar a nova conclusão validada pela revisão anterior.

Este exemplo não representa avaliação de comportamento já executada.
