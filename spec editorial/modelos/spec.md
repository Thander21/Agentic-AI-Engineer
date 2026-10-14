# Modelo de spec editorial

**Versão do modelo:** 0.1  
**Entrega de origem:** ENT-02 / T01-002  
**Orientação:** [Guia de operação](../GUIA_DE_OPERACAO.md).

## Como usar este modelo

Copie a estrutura abaixo para a spec da iniciativa. Substitua os campos entre chaves, ajuste os caminhos dos links ao destino e remova estas instruções da cópia. Os campos vazios e exemplos deste modelo não representam decisões ou resultados do projeto.

Mantenha análise, especificação e revisão no mesmo documento. O plano descreverá como implementar; as tasks registrarão execução e conferência. Não é necessário preencher aqui uma lista de arquivos ou tarefas. Para uma entrega textual dentro de uma iniciativa já definida, use a ficha editorial quando disponível, sem criar outra spec completa por rotina.

Dimensione o preenchimento ao trabalho. Seções sem pertinência podem receber “não se aplica” com motivo breve; decisões necessárias que faltam recebem “pendente”, com impacto e momento de resolução. Não invente fontes, público, voz ou vivências para completar o modelo. Conserve IDs dos requisitos e decisões quando revisar a spec.

---

# Spec — {nome da iniciativa}

**ID:** {identificação estável da spec}  
**Versão:** {versão desta spec}  
**Data:** {data da atualização}  
**Estado:** em elaboração  
**Responsável pela elaboração:** {pessoa ou IA/papel}  
**Origem:** {pedido e documentos de referência, com localização recuperável}  
**Plano e tasks associados:** {não gerados / caminhos existentes e versões}

## 1. Contexto e necessidade

**Situação atual:** {o que existe e qual dificuldade motivou o trabalho}.

**Pedido do autor:** {intenção expressa e restrições recebidas; distinguir da interpretação da IA}.

**Público ou usuário da entrega:** {quem utilizará o resultado, seu contexto e pré-requisitos conhecidos; indicar o que falta definir}.

**Pergunta central:** {qual problema esta iniciativa precisa resolver}.

**Contribuição esperada:** {o que deve melhorar para quem recebe ou utiliza a entrega}.

## 2. Base de informação e análise inicial

| ID da fonte ou registro | Localização / versão / trecho | O que sustenta | Natureza e situação da informação | Limites ou conferência necessária |
| --- | --- | --- | --- | --- |
| {ID existente ou referência local} | {caminho ou URL e localização pertinente} | {afirmação, contexto ou decisão} | {relato do autor, fonte consultada, transcrição, hipótese, interpretação ou exemplo fictício; situação da conferência} | {limite conhecido} |

**O que já está estabelecido:** {fatos e decisões confirmadas, ligados à origem}.

**O que ainda é proposta ou hipótese:** {interpretações que não devem ser tratadas como decisões}.

**Lacunas e conflitos encontrados:** {questões a registrar nas decisões ou pendências abaixo}.

Uma informação arquivada não se torna verdadeira apenas por estar preservada. Distinguir a fidelidade de uma transcrição da validade do que ela afirma. Registrar a ausência de evidência quando relevante.

## 3. Objetivo, escopo e limites

**Resultado pretendido:** {entrega ou comportamento esperado, com utilidade identificável}.

**Incluído:** {frentes que fazem parte do pedido}.

**Fora do escopo atual:** {frentes relacionadas que não serão executadas nesta iniciativa}.

**Restrições confirmadas:** {tempo, formato, recursos ou decisões que realmente condicionam o trabalho; indicar origem}.

**Dependências externas:** {informações, materiais ou decisões de outra iniciativa; não antecipar escolhas de implementação do plano}.

## 4. Requisitos e critérios de aceitação

| ID | Resultado ou comportamento exigido | Motivo / origem | Evidência adequada para avaliar | Momento da avaliação |
| --- | --- | --- | --- | --- |
| REQ-01 | {enunciado concreto, sem múltiplas obrigações desconexas} | {necessidade ou decisão relacionada} | {observação, fonte, artefato, parecer ou apreciação humana pertinente} | {conferência documental, uso inicial ou avaliação autoral, por exemplo} |

Use critérios que permitam examinar o resultado. Para aspectos literários, indicar a dimensão, os trechos a observar e quem fará a apreciação; evitar promessas de agradar a todos ou notas automáticas de humanidade. Um critério futuro ainda não é evidência de atendimento.

## 5. Regras e liberdade de execução

| ID | Regra ou convenção | Origem / situação | Onde se aplica e limite |
| --- | --- | --- | --- |
| REG-01 | {regra necessária ao resultado} | {decisão confirmada, requisito ou proposta ainda em avaliação} | {escopo concreto} |

**Liberdade preservada:** {decisões de organização, escrita ou abordagem que podem variar sem descumprir a intenção}.

**Referência editorial:** {vínculo com público, voz, tom e convenções definidos na spec editorial pertinente; não copiar toda a referência}.

**Limites factuais e autorais:** {como separar vivência real, interpretação, metáfora e exemplo quando aplicável}.

## 6. Alternativas e decisões

| ID | Questão | Alternativas e consequências relevantes | Situação / decisão | Motivo e origem da decisão | Condição para reconsiderar |
| --- | --- | --- | --- | --- | --- |
| DEC-01 | {questão} | {opções reais, quando houver} | {aberta / decidida / substituída; decisão vigente} | {quem decidiu e onde a decisão está registrada} | {nova evidência ou mudança relevante} |

Não transformar uma sugestão da IA em decisão aceita sem base no pedido ou nas decisões do autor. Decisões rotineiras dentro do escopo podem ser justificadas pelo responsável pela elaboração; preferências e vivências pessoais continuam pertencendo ao autor.

## 7. Pendências e condições de avanço

| ID | Informação ou decisão ausente | Impacto | Quem ou qual fonte pode resolver | Até quando precisa estar resolvida | Impede elaborar o plano? |
| --- | --- | --- | --- | --- | --- |
| PEN-01 | {lacuna concreta} | {o que não pode ser concluído sem ela} | {autor, fonte ou outra iniciativa} | {antes de qual atividade; data somente se definida} | {sim/não, com motivo} |

Pendência de voz para um piloto não impede necessariamente planejar modelos genéricos. Uma intenção contraditória ou requisito central sem definição pode impedir planejar a parte afetada. Nomear a dependência e avançar apenas onde houver base suficiente.

## 8. Revisão de consistência desta spec

**Versão examinada:** {versão}  
**Revisor e escopo:** {quem revisou e quais aspectos}  
**Contexto recebido:** {fontes, documentos e pareceres anteriores disponíveis}  
**Limitações:** {o que não foi examinado; informar acesso ao histórico e ausência de revisão independente quando pertinente}.

| Achado | Trecho / requisito afetado | Problema e fundamento | Importância | Decisão e alteração | Situação e evidência da resolução |
| --- | --- | --- | --- | --- | --- |
| REV-01 | {localização} | {contradição, ambiguidade, omissão ou dependência circular, por exemplo} | {impeditivo, revisão necessária ou sugestão} | {corrigir, manter com motivo ou encaminhar} | {aberto / resolvido / encaminhado, com evidência} |

Uma revisão sem achados pode registrar esse resultado com seu escopo e limites; remova a linha demonstrativa em vez de fabricar um achado. Problemas de estratégia encontrados depois voltam ao plano; problemas de intenção ou regra voltam a esta spec.

### Parecer para elaborar o plano

**Resultado:** não avaliado. Substituir após revisão por “apta para plano” ou “necessita ajustes”, com fundamento.

**Fundamento:** {verificar objetivo e escopo, requisitos e critérios, coerência das regras, destino das pendências e ausência de impeditivos de planejamento abertos}.

**Pendências que permanecem:** {IDs, impacto e momento de resolução; ou nenhuma identificada no escopo examinado}.

**Próximo passo:** {gerar plano da versão identificada ou resolver achados específicos}.

O parecer indica suficiência documental para planejar. Não declara implementação, validação em uso, apreciação autoral ou publicação. Se mudar um requisito relevante depois do parecer, revisar o ponto afetado antes de reutilizá-lo.

## 9. Mudanças e impactos

| Versão / data | Alteração e motivo | Requisitos ou decisões afetados | Impacto nos documentos derivados | Responsável pelo registro |
| --- | --- | --- | --- | --- |
| {versão / data} | {criação ou mudança relevante} | {IDs} | {plano/tasks/artefatos a reconferir; ou ainda não gerados} | {papel ou pessoa} |

Preservar o raciocínio necessário para compreender mudanças. A execução e a conferência das entregas serão acompanhadas nas tasks, sem transformar esta tabela em outra lista de tarefas.
