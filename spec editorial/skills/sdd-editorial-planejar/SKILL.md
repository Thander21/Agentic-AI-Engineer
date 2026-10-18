---
name: sdd-editorial-planejar
description: Elabora, ajusta ou confere o plano separado de uma iniciativa editorial com spec suficientemente revisada. Organiza entregas, documentos afetados, dependências e evidências proporcionais; não redefine intenção nem redige as peças.
metadata:
  version: "0.3"
---

# Planejar uma iniciativa editorial

## Entrada e referências

Receber pedido/fase autorizada, spec e versão, parecer e lacunas; plano existente se houver. Usar [guia](../../GUIA_DE_OPERACAO.md) e [modelo de plano](../../modelos/plano.md) conforme necessidade. Parecer antigo não valida mudança posterior: conferir o impacto antes de planejar. Falta de intenção essencial volta à spec; planejar partes independentes possíveis.

## Ação

- Definir entregas verificáveis com ID, função, requisito de origem, documento/artefato previsto, dependência e critério. Caminho futuro é texto previsto, não link de entrega já existente.
- Mapear todos os requisitos a entregas, sem criar um arquivo por requisito. Verificar ciclos, referências inexistentes e informação externa sem responsável/momento.
- Para texto, organizar a sequência do guia: preparação, esboço condicional, redação, revisão, integração, reconferência, autor, ajustes condicionais e prova. Distinguir a cadeia da iniciativa da produção das peças. Não criar outra spec/plano/tasks para cada peça breve.
- Selecionar skills/perfis por questão real. Plano coordena; skill executa; task acompanha. Definir quais versões/fontes passam entre papéis, sem exigir todo o acervo. Uma mesma IA pode assumir papéis, sem independência alegada ou delegação automática.
- Definir preservação conforme D05-01 no guia: texto que precisa ser preservado e não está no Git depende de commit do autor antes da edição, salvo dispensa explícita para a versão em andamento; registrar seu alcance, conforme o guia. Não criar cópia paralela ou commit automático.
- Propor conferência proporcional: documento por coerência/referências, texto por fatos/sentido/legibilidade, apreciação por retorno real. Validação de skill não demonstra eficácia editorial. Definir cobertura não exercitada e seu destino, sem simular resultados.

## Saída e limites

Plano separado com base, entregas/cobertura, ordem, decisões operacionais, pendências e parecer **apto para tasks**, **necessita ajustes** ou **não avaliado**. Declarar quem conferiu e o contexto; não fabricar achados. Mudar intenção/requisito retorna à spec; estratégia fica no plano; execução/evidência nas tasks.

Aptidão para tasks não inicia execução por consequência. Se o pedido autoriza toda a implementação, continuar a decomposição e execução independentes no escopo, sem nova confirmação por arquivo. Retorno autoral e envio público continuam ações distintas. Não impor motor, RED/GREEN ou infraestrutura ao texto.
