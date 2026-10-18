---
name: sdd-editorial-especificar
description: Analisa, elabora ou revisa uma spec editorial, reunindo contexto, requisitos, decisões, lacunas e parecer no mesmo documento. Use no refinamento ou mudança de intenção; não inicia plano ou produção por consequência automática.
metadata:
  version: "0.2"
---

# Especificar uma iniciativa editorial

## Entrada e modo

Receber pedido/limite, iniciativa e versão quando existente, decisões autorais e fontes selecionadas. Identificar modo: analisar (diagnóstico), elaborar (criar/ajustar spec) ou revisar (parecer sobre a versão). Análise/revisão sem autorização de edição entrega parecer; quando o registro na spec fizer parte do pedido, atualizá-la sem outro relatório. Refinar no backlog não seleciona a iniciativa nem autoriza implementar.

Consultar o [guia](../../GUIA_DE_OPERACAO.md) para fases/autoridade e o [modelo de spec](../../modelos/spec.md) apenas para campos necessários. Sem tasks, parecer/próxima ação da spec orientam a retomada.

## Ação

1. Conferir o estado real: documentos, decisões vigentes, material existente e lacunas. Não transformar proposta antiga ou transcrição de IA em fato técnico, vivência ou escolha aceita.
2. Definir problema, resultado, leitor da entrega, escopo e limites. Para iniciativa editorial já definida, não criar outra spec por peça pequena.
3. Redigir requisitos identificáveis com critério observável. Relacionar cada requisito à fonte/decisão pertinente; não inventar preferências, aprendizados ou resultados do autor.
4. Distinguir informação essencial para a intenção de detalhamento que pode esperar o plano. Perguntar só pela lacuna concreta, continuar partes independentes e registrar resposta no lugar pertinente.
5. Rever contradições, critérios vagos, dependências circulares, interpretação indevida de história e mistura de intenção com execução. Preservar IDs e fatos úteis; não reformatar por rotina.

## Saída e passagem

Spec identificada, requisitos/decisões, pendências com efeito/momento e parecer: **apta para plano**, **necessita ajustes** ou **não avaliada**. Achado identifica trecho, fundamento, importância e destino; ausência de achados não exige inventá-los. Declarar autoria, histórico disponível e limites da revisão.

Apta para plano significa contexto suficiente e nenhum impeditivo de planejamento; não implementação, eficácia editorial ou aprovação de texto. Mudança de requisito exige reconferir o aspecto e seus derivados. Seleção para changes e elaboração do plano dependem da fase pedida; “continue” segue o escopo já autorizado, não para mecanicamente por documento nem cria autorização de publicação.
