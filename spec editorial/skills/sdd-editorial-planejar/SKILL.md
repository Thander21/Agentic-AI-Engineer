---
name: sdd-editorial-planejar
description: Elabora, ajusta ou confere um plano separado a partir de uma spec editorial revisada, definindo entregas, caminhos, dependências e cobertura dos requisitos. Use na passagem da especificação ao planejamento de uma iniciativa editorial. Não use para definir a intenção inicial, gerar tasks, implementar skills ou redigir o texto final.
metadata:
  version: "0.1"
---

# Planejar uma iniciativa editorial

Transforme uma spec revisada em uma estratégia executável e proporcional ao trabalho. O plano descreve entregas e condições de conferência; não executa essas entregas nem registra resultados futuros como concluídos.

## Delimitar a atuação

Identifique se o pedido é criar, ajustar ou apenas conferir um plano. Para conferência somente, apresente achados sem modificar arquivos. Quando a edição estiver incluída no pedido, registre correções e histórico no plano. Não iniciar outra fase automaticamente.

Receba a spec com ID, caminho e versão, seu parecer de prontidão, as decisões pertinentes e o plano existente, se houver. Um parecer antigo não basta quando a spec mudou: examine o impacto das alterações antes de reutilizá-lo. Se faltar revisão suficiente para planejar, exponha a lacuna e encaminhe à spec; não emita uma aprovação implícita para contornar a dependência.

## Consultar o contexto necessário

- [Guia de operação](../../GUIA_DE_OPERACAO.md): consulte para fases, estados e critérios de passagem.
- [Modelo de plano](../../modelos/plano.md): use na criação ou para conferir os campos necessários; preserve a organização de um plano existente quando ela já funcionar.
- [Modelo de parecer](../../modelos/parecer-editorial.md): consulte quando precisar estruturar achados detalhados de revisão, incorporando os campos pertinentes ao próprio plano.

Resolva referências a partir desta pasta e confirme sua existência. Recursos ausentes não devem ser substituídos por conteúdo inventado. O pacote depende do conjunto local; sua leitura explícita não demonstra descoberta automática pelo ambiente. Não carregar o acervo inteiro ou todos os modelos quando bastarem os documentos pertinentes.

## Converter requisitos em entregas

1. Identifique o resultado pretendido, o escopo e as restrições confirmadas. Diferencie material existente de material a produzir e de decisões ainda abertas.
2. Agrupe resultados em entregas verificáveis. Uma entrega pode reunir arquivos relacionados, mas não deve ocultar resultados independentes com critérios diferentes. Não criar um arquivo por requisito apenas para preencher a cobertura.
3. Para cada entrega, defina ID estável, função, requisitos de origem, caminho ou destino previsto, papel responsável e critério de conferência. Diferencie arquivo produzido, qualidade examinada e retorno humano recebido.
4. Defina a base dos caminhos e a preservação dos materiais existentes. Mostre caminhos futuros como previstos, sem apresentá-los como links para arquivos já entregues.
5. Registre escolhas de implementação e seus motivos. Se uma escolha mudar público, intenção, obrigação ou limite da spec, devolva a questão à especificação; não a introduza silenciosamente no plano.

Se o plano incluir novas skills, defina agrupamento, entrada, saída, limites, localização dos pacotes, referências e modo de acesso. Se a iniciativa for apenas produzir um texto com procedimentos existentes, não ampliar o escopo para criar uma coleção de skills.

## Ordenar sem criar dependências artificiais

Relacione entregas por entradas necessárias e resultados que liberam a etapa seguinte. Confira referências a IDs inexistentes, ciclos e dependências externas sem encaminhamento.

Quando o método estiver sendo construído, explique como produzir os primeiros artefatos antes de existirem suas próprias skills ou modelos. Uma orientação manual baseada na spec pode resolver o início; não exigir uma skill pronta para criar essa mesma skill.

Para cada pendência relevante, registre impacto, entregas afetadas, quem ou qual fonte resolve e momento necessário. Uma preferência de voz pode impedir o piloto sem impedir modelos genéricos. Já uma contradição central que altera as entregas precisa voltar à spec antes de declarar o plano pronto.

Planeje as partes independentes quando houver base suficiente. Não decida preferências pessoais pelo autor nem bloqueie todo o trabalho por uma dependência que só afeta a última etapa. O plano pode indicar atividades separáveis, sem exigir agentes paralelos.

## Definir cobertura e conferência

Mapeie cada requisito do escopo para uma ou mais entregas e indique a evidência adequada. Requisito sem destino ou critério é uma lacuna; não removê-lo da tabela para aparentar cobertura completa. Se deixar de se aplicar, a decisão deve constar na spec.

Escolha a conferência conforme o resultado: estrutura e links para documentos; comportamento observado para procedimentos; fontes para afirmações factuais; apreciação do autor para sua voz. Não declarar prazer de leitura, competência ou autoridade comprovados por uma lista de verificações automáticas.

Quando houver exercícios, descreva situações que revelem decisões úteis ou falhas relevantes. Uma avaliação de comportamento não se reduz a comparar títulos e palavras esperadas. Identifique como registrar entradas, versões, resultados e limitações nas tasks, sem impor uma suíte de software a uma iniciativa de escrita.

Preveja o retorno dos achados: correção de entrega nas tasks; mudança de estratégia no plano; mudança de regra ou intenção na spec. Apreciação humana necessária deve ter seu momento e critério próprios, sem aprovação presumida.

## Ajustar ou revisar o plano

Conserve IDs existentes das entregas. Registre nova versão, motivo da mudança, base da spec e impacto sobre tasks e artefatos. Não editar esses documentos derivados silenciosamente quando o pedido estiver limitado ao plano.

Antes do parecer, confira:

- Correspondência entre plano e versão da spec usada.
- Entregas, caminhos, procedimentos e critérios suficientes para decompor em tasks.
- Cobertura de todos os requisitos do escopo.
- Dependências possíveis e pendências com destino e momento definidos.
- Separação entre planejamento, implementação e evidência de validação.
- Proporcionalidade do esforço e respeito à liberdade editorial.

Cada achado aponta localização, problema, fundamento, importância e encaminhamento. Uma revisão sem problemas pode registrar esse resultado com seus limites; não fabricar achados. Declare se a revisão teve acesso ao histórico ou foi feita pela mesma IA autora.

## Entregar e encerrar

O plano deve indicar versões de referência, decisões de implementação, entregas, sequência, procedimentos, cobertura, conferências, pendências e histórico. Remova campos demonstrativos da cópia final e ajuste seus links.

Use **apto para tasks** quando houver base suficiente para decompor o trabalho e nenhum impeditivo de planejamento aberto. Use **necessita ajustes** com achados específicos quando faltar essa base. Mantenha **não avaliado** se a revisão não foi realizada.

Informe o documento e a versão, as decisões tomadas dentro do escopo, as pendências e o próximo passo. O parecer não cria tasks nem comprova implementação. Interrompa a passagem apenas no ponto dependente de informação essencial, continuando o planejamento independente autorizado.

## Exemplo de decisão — ilustrativo

Uma spec revisada pede modelos editoriais e um piloto, mas o autor ainda não definiu a intensidade de humor. Planeje a criação dos modelos com campos abertos e registre a definição de humor como condição para o piloto. Não escolha o tom pelo autor, não bloqueie a produção dos modelos e não escreva o episódio durante o planejamento.

Este exemplo não representa uma avaliação executada nem prova de comportamento da skill.
