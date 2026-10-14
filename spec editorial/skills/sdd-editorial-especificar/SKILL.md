---
name: sdd-editorial-especificar
description: Analisa necessidades, elabora ou revisa specs de iniciativas editoriais, reunindo contexto, requisitos, decisões e parecer de prontidão no documento inicial. Use para definir ou avaliar uma metodologia de escrita ou uma iniciativa editorial antes do plano. Não use para redigir capítulos, revisar apenas a linguagem de um texto ou executar tarefas de implementação.
metadata:
  version: "0.1"
---

# Especificar uma iniciativa editorial

Produza uma base suficiente para planejar, preservando a intenção do autor e distinguindo requisitos, propostas e informação ainda não confirmada. A análise e a revisão pertencem à própria spec; plano e tasks são etapas separadas.

## Selecionar o modo

Identifique o modo pelo pedido e informe qual será executado. Um pedido pode autorizar mais de um modo; não avance para outra fase apenas porque terminou a anterior.

| Modo | Pedido típico | Entrega |
| --- | --- | --- |
| Analisar | Examinar contexto, lacunas ou possibilidades. | Análise localizada, questões e alternativas. Atualize a spec quando a edição fizer parte do pedido; em análise somente, entregue o parecer sem modificar arquivos. |
| Elaborar | Criar ou ajustar uma spec. | Spec criada ou atualizada, com requisitos, decisões e pendências explícitas. |
| Revisar | Verificar se a spec está coerente e pronta para o plano. | Achados, correções autorizadas e parecer fundamentado sobre a versão examinada. Registre na spec quando autorizado; em revisão somente, apresente o parecer. |

Elaboração não equivale a prontidão: se não houve revisão de consistência suficiente, mantenha o parecer não avaliado. Não gerar plano, tasks, skills ou textos narrativos como efeito automático desta skill.

## Receber e selecionar contexto

1. Localize o pedido atual, decisões anteriores pertinentes e a spec existente, se houver. Identifique caminho, ID e versão antes de alterar.
2. Reúna apenas as fontes necessárias ao escopo: objetivo, público conhecido, acervo relevante, restrições e documentos relacionados. Preserve referências recuperáveis às afirmações e decisões centrais.
3. Distinga relato do autor, fonte consultada, transcrição histórica, interpretação, hipótese e exemplo fictício. Informação arquivada não se torna fato validado ou decisão vigente por estar no acervo.
4. Identifique lacunas que impedem definir a intenção e as que podem ser resolvidas depois. Pergunte pelo ponto essencial e avance nas partes independentes. Não inferir vivência, voz, variante linguística ou canal de publicação para preencher campos.

## Usar os recursos do projeto

Os caminhos abaixo são relativos à pasta desta skill. Confirme sua existência e leia apenas o que for pertinente:

- [Guia de operação](../../GUIA_DE_OPERACAO.md): consulte para regras de fluxo, contexto, responsabilidades e encerramento.
- [Modelo de spec](../../modelos/spec.md): use ao criar uma spec ou conferir seus campos. Não reformatar uma spec existente apenas para fazê-la parecer com o modelo.
- [Modelo de parecer](../../modelos/parecer-editorial.md): consulte se a revisão exigir achados detalhados. Incorpore os campos necessários à seção de revisão da spec, sem impor outro documento.

Esta skill depende do conjunto local. Se um recurso necessário estiver ausente, informe qual e o impacto; não invente seu conteúdo. A leitura explícita deste arquivo não prova instalação ou descoberta automática pelo ambiente.

## Analisar e elaborar

- Explicite problema, contribuição esperada, público conhecido, escopo e limites. Relacione-os ao pedido, evitando expandir uma ideia de escrita para um sistema maior sem necessidade.
- Transforme necessidades em requisitos identificáveis com critério observável. Separe obrigações diferentes quando isso ajudar a avaliá-las; evite metas como agradar a todos ou garantir autoridade.
- Para qualidade literária, indique aspectos e trechos a apreciar e quem poderá avaliar. Não transformar voz e prazer de leitura em pontuações automáticas.
- Registre alternativas somente onde exista uma escolha relevante. Diferencie decisão recebida do autor, decisão operacional justificada e proposta ainda aberta. Uma sugestão anterior não conta como aceitação.
- Vincule fontes às afirmações que sustentam. Se houver conflito, exponha-o e registre a necessidade de decisão ou pesquisa antes de consolidar uma conclusão.
- Mantenha pendências com impacto, fonte ou responsável por resolvê-las e momento necessário. Uma preferência de voz pendente pode impedir avaliar um piloto sem impedir planejar modelos genéricos.
- Ao alterar uma spec existente, conserve IDs, registre a nova versão e o motivo. Identifique planos, tasks e textos afetados, sem modificá-los silenciosamente quando o pedido estiver limitado à spec.

## Revisar consistência

Examine a versão identificada, não apenas o parecer anterior. Procure:

- Contradições entre pedido, objetivo, escopo e regras.
- Requisitos vagos, sem base ou sem critério adequado de avaliação.
- Decisões pessoais assumidas como fatos ou propostas apresentadas como confirmadas.
- Dependências circulares ou informação indispensável sem encaminhamento.
- Mistura entre intenção da spec, estratégia do plano e evidência de execução.
- Critérios que restringem a criatividade sem contribuir para o resultado.

Cada achado aponta trecho ou ID, problema, fundamento, importância e encaminhamento. Ao sugerir mudança expressiva, explicite ganho e possível perda. Também é válido recomendar manter uma passagem; não há quantidade mínima de correções.

Use impeditivo para algo que comprometa a intenção central ou impeça planejar a parte necessária; revisão necessária para falha que requer correção ou justificativa; sugestão para alternativa não obrigatória. Não classifique toda pendência futura como impeditivo atual.

Se você escreveu a spec ou recebeu pareceres anteriores, declare isso. Não alegue independência por assumir um novo papel na mesma conversa.

## Emitir o resultado

Na spec, mantenha contexto, fontes, requisitos, regras, alternativas, decisões, pendências, revisão e histórico juntos. Remova linhas demonstrativas do modelo da cópia final; conserve pendências reais identificadas. Ajuste caminhos dos links ao local do documento gerado.

O parecer pode ser:

- **Apta para plano:** objetivo e escopo claros, requisitos avaliáveis, regras coerentes e ausência de impeditivos de planejamento abertos. As pendências restantes têm destino e momento de resolução.
- **Necessita ajustes:** identifique os achados que impedem avançar e a próxima ação necessária.
- **Não avaliada:** quando o pedido não incluiu revisão ou a base disponível não permitiu realizá-la.

Conclua informando documento e versão, mudanças relevantes, pendências e próximo passo. Não confundir prontidão documental com implementação, validação prática, apreciação autoral ou publicação. Se um requisito relevante mudar após o parecer, reconfira o impacto antes de reutilizar a conclusão.

## Exemplo de decisão — ilustrativo

Pedido: analisar uma spec que exige humor em todo parágrafo e também proíbe humor nas explicações técnicas.

No modo analisar, aponte o conflito e proponha delimitar onde cada regra vale. Não escolha a intensidade pelo autor, não redija o episódio e não declare a spec pronta enquanto a contradição central permanecer. Uma preferência de canal ainda aberta pode ser registrada separadamente, com seu momento de resolução.

Este exemplo orienta a decisão; não representa exercício executado nem prova de comportamento da skill.
