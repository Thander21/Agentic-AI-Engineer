# Modelo de integração e avaliação editorial

**Versão do modelo:** 0.1  
**Entrega de origem:** ENT-03 / T01-007  
**Orientação:** [Guia de operação](../GUIA_DE_OPERACAO.md) · [Ficha editorial](ficha-editorial.md) · [Parecer editorial](parecer-editorial.md).

## Como usar

Copie a estrutura abaixo para acompanhar a integração de uma entrega. Substitua os campos entre chaves e ajuste os caminhos. Linhas demonstrativas não representam decisões nem validações realizadas. Para trabalho breve, reduza o preenchimento aos dados pertinentes, mantendo versões, destino dos achados, evidências e limites.

Este registro liga pareceres à versão resultante. A ficha mantém intenção e contexto; os pareceres preservam suas observações; as tasks registram execução e conclusão. Referencie esses documentos em vez de copiá-los integralmente. Avaliação do método e das skills é necessária quando o trabalho tiver essa finalidade, como no piloto; em uma revisão comum, pode ser declarada não aplicável com motivo.

Não editar sem uma versão de partida recuperável. Não confundir sugestão acolhida com alteração já aplicada, nem alteração aplicada com correção conferida.

---

# Integração e avaliação — {texto ou artefato}

**ID deste registro:** {identificação estável}  
**Versão/data:** {versão e data da atualização}  
**Editor responsável:** {pessoa ou IA/papel}  
**Tarefa e base:** {ID da tarefa; versões da spec/plano quando pertinentes}  
**Ficha:** {caminho e versão / contrato da entrega operacional}  
**Texto de partida:** {ID, caminho e revisão exata}  
**Versão de partida preservada em:** {cópia identificada ou histórico verificado que permita recuperá-la}  
**Versão resultante:** ainda não produzida.  
**Estado da integração:** não iniciada.

## 1. Objetivo e elementos a preservar

**Intenção da entrega:** {pergunta, contribuição e público, referenciando a ficha}.

**Escopo desta rodada:** {trechos e mudanças que serão examinados}.

**Elementos a preservar:** {fatos, argumento, ressalvas, fontes, função narrativa e traços de voz}.

**Limites de alteração:** {decisões que exigem retorno ao autor, à ficha ou à spec}.

Reorganizar ou cortar pode melhorar a leitura sem alterar a intenção. Se mudar a tese, o escopo ou uma interpretação factual relevante, registrar a mudança editorial e sua origem antes de tratá-la como simples polimento.

## 2. Pareceres e contexto recebidos

| Parecer / versão | Perfil e revisor | Versão do texto examinada | Escopo e limites declarados | Aplicabilidade à versão de partida |
| --- | --- | --- | --- | --- |
| {ID e caminho} | {papel e autoria} | {revisão exata} | {contexto, fontes ausentes ou acesso a pareceres anteriores} | {aplicável / exige reexame do trecho; motivo} |

**Decisões autorais recebidas:** {localização e conteúdo pertinente; nenhuma quando não recebidas}.

Parecer desatualizado não deve ser aplicado automaticamente. Examine o trecho atual e registre o que continua pertinente. Se faltar base para resolver um achado, mantenha a pendência explícita.

## 3. Destino dos achados e passagens a preservar

| Referência completa | Importância / tipo | Decisão e motivo | Ganho esperado e possível perda | Aplicação e versão resultante | Conferência / pendência |
| --- | --- | --- | --- | --- | --- |
| {ID do parecer + ACH-ID ou PRE-ID} | {impeditivo, revisão necessária, sugestão ou preservação} | {acolhido, recusado com motivo ou pendente} | {efeito pretendido e cuidado necessário} | {não aplicada / alteração localizada ou preservação confirmada; revisão} | {evidência, encaminhamento ou não conferida} |

Identificar o parecer junto do achado evita confundir dois ACH-01 de revisores diferentes. Achados equivalentes podem ser agrupados desde que todas as referências permaneçam recuperáveis. Recomendações de preservação também recebem destino quando afetadas pela integração.

## 4. Conflitos e decisões

| Conflito | Pareceres/achados envolvidos | Alternativas e consequências | Base da decisão | Resolução ou pergunta necessária |
| --- | --- | --- | --- | --- |
| {problema} | {referências} | {opções reais} | {intenção, fonte, voz ou decisão do autor} | {escolha fundamentada ou pendência} |

Não decidir por maioria de agentes. Uma sugestão de ritmo não autoriza eliminar uma ressalva factual. Impasses sobre vivência, posicionamento ou mudança de tese retornam ao autor. Sem conflito, registrar que nenhum foi identificado no escopo, removendo a linha demonstrativa.

## 5. Alterações e comparação entre versões

| Mudança | Antes: versão/localização | Depois: versão/localização | Motivo e achados relacionados | O que foi preservado ou mudou de sentido | Impacto em outros textos/documentos |
| --- | --- | --- | --- | --- | --- |
| {ID ou descrição} | {trecho recuperável} | {trecho resultante} | {fundamento} | {fatos, ressalvas, voz e função} | {referências afetadas e ação necessária / nenhum identificado} |

**Versão integrada e localização:** {preencher depois de produzi-la}.

**Condição de recuperação da versão anterior:** {como foi verificada; não presumir histórico automático}.

Se a intenção mudar, atualizar a ficha ou spec pertinente e identificar planos/tasks afetados. Evitar duplicar registros de origem para cada texto derivado; manter vínculos com a experiência e as fontes.

## 6. Reconferência e leitura do conjunto

| Alteração / aspecto | Perfil ou pessoa necessária | Versão e trecho conferidos | Resultado observado / evidência | Limites e pendências |
| --- | --- | --- | --- | --- |
| {mudança} | {factual, didática, continuidade, voz, língua ou autor} | {referência} | {não realizada até haver observação; depois registrar resultado} | {o que falta} |

Direcionar a reconferência ao impacto: nova conclusão exige exame factual; reorganização pode afetar a progressão didática; alteração de metáfora pode afetar continuidade. Não reiniciar todos os perfis por uma correção localizada sem efeito no sentido.

**Leitura final do conjunto:** não realizada. Quando ocorrer, registrar versão, responsável, leitura silenciosa ou em voz alta efetivamente realizada, e observações sobre transições, repetições, ritmo e efeitos das alterações.

**Prova final:** {não realizada / versão examinada, achados e resolução; verificar que corresponde à versão integrada vigente}.

## 7. Avaliação separada dos resultados

### 7.1. Orientação documental — spec, ficha e contexto

**Situação:** não avaliada; ou não se aplica, com motivo.

{O contexto foi suficiente? Quais ambiguidades, campos ausentes ou desnecessários causaram dúvidas? Indicar exemplos, documento e versão. Separar falha da orientação de falha ao segui-la.}

### 7.2. Funcionamento das skills ou procedimentos

**Situação:** não avaliado; ou não se aplica, com motivo.

| Procedimento e versão | Entrada / saída examinada | Resultado observado | Limites da avaliação | Ajuste e evidência necessária depois |
| --- | --- | --- | --- | --- |
| {skill e modo/perfil, ou execução manual} | {referências recuperáveis} | {comportamento e efeito concreto} | {o que não foi demonstrado} | {mudança localizada ou nenhuma identificada} |

Registrar a passagem de fatos, ressalvas e pendências entre os papéis. Conferência estrutural de arquivos não demonstra comportamento, e um exercício isolado não prova qualidade geral. Não atribuir uma execução manual a uma skill que ainda não existe.

### 7.3. Qualidade do texto e apreciação humana

| Aspecto | Quem avaliou e em qual contexto | Versão / trecho | Observação e evidência | Situação / encaminhamento |
| --- | --- | --- | --- | --- |
| {voz, clareza, precisão, ritmo ou prazer de leitura} | {autor, leitor, revisor ou IA; distinguir as origens} | {referência} | {retorno realmente recebido ou percepção identificada} | {funciona / precisa de ajuste / não avaliado} |

**Retorno do autor:** pendente até ser recebido. Registrar data, versão avaliada, percepção e escolhas, sem interpretar silêncio como aprovação.

**Retorno de leitores:** {não recebido / referência ao retorno efetivo}.

### 7.4. Esforço e utilidade

{Registrar o esforço observado ou relatado, retrabalho, pareceres úteis, campos dispensáveis e perdas de voz ou clareza. Tempos só devem ser informados quando medidos ou explicitamente estimados. Indicar se a avaliação é da IA ou do autor.}

## 8. Encerramento e retorno às tasks

**Versão a que este encerramento se refere:** {revisão exata}.

- **Impeditivos:** {abertos com IDs / nenhum identificado no escopo conferido}.
- **Revisões necessárias:** {resolvidas, justificadas ou pendentes, com referências}.
- **Prova e reconferências:** {resultado efetivo e aspectos não examinados}.
- **Apreciação autoral:** {pendente / recebida e decisões encaminhadas}.
- **Resultado da rodada:** não avaliado. Após conferir, indicar necessita ajustes, pronta para leitura autoral ou rodada encerrada no escopo, com fundamento.
- **Tarefas a atualizar ou reabrir:** {IDs, estado adequado e motivo}.
- **Próxima ação:** {ação delimitada ou encerramento do escopo realizado}.
- **Publicação:** {não realizada / registro de publicação efetivamente ocorrida, com destino e versão}.

Uma rodada pode terminar com o texto pronto para leitura autoral, mas a tarefa que exige essa avaliação permanece pendente. Publicação exige decisão própria e não ocorre automaticamente. Não transformar impeditivos em melhorias futuras para encerrar a tarefa.

## 9. Histórico

| Data / versão deste registro | Acontecimento | Versões do texto envolvidas | Decisão e evidência |
| --- | --- | --- | --- |
| {data/versão} | {integração, retorno, correção ou reabertura} | {referências} | {o que ocorreu e onde conferir} |

Preservar os resultados anteriores em seu contexto. Uma alteração posterior pode invalidar uma conferência sem tornar falso o registro de que ela foi realizada naquela versão.
