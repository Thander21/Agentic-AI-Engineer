# Spec 03 — Piloto editorial e avaliação do método

**ID:** SPEC-EDITORIAL-003. **Versão:** 1.4 — 17/10/2026.
**Estado:** em changes; ficha, esboço e artigo r01 produzidos. Progresso e próxima ação somente nas [tasks 03](03-tasks-piloto-editorial.md). [Plano vigente](03-plano-piloto-editorial.md).
**Método vigente:** [guia](../../GUIA_DE_OPERACAO.md), reconciliado pela [iniciativa 05](<../../concluida/05-ajuste-fluxo-sdd-editorial/05-spec-ajuste-fluxo-sdd-editorial.md>). A implementação de 05 não é revisão da prosa do piloto.

## 1. Intenção, contexto e entradas

Aplicar o método a material real: [01 — Novo mundo, bagagem antiga](<../../../jornada do heroi/01-novo-mundo-bagagem-antiga.md>), comparar versões, receber retorno do autor e avaliar o texto e o esforço editorial. A etapa é contexto, não relato pronto; a cena no Reino dos Agentes é metáfora proposta.

Receber a [preparação 02 v0.26](../../concluida/02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md), plano v0.9, tasks v0.21 e [EX02-A/B](../../avaliacoes/T02/02-complementos-voz-e-artigo/03-pareceres-e-integracao.md). Essas entradas prepararam o recorte e modos necessários; exercícios não comprovam eficácia do piloto.

Decisões recebidas de RA02-10/14/15/16: artigo no LinkedIn sobre a origem do percurso e necessidade de fundamentos, acompanhado de post de chamada; pessoas com dúvidas ao desenvolver com IA, com ou sem bagagem de TI; primeira pessoa, português brasileiro, humor/retórica e extensão livre/proporcional. Família, furão e repertório são possibilidades, sem cenas ou emoções inventadas e sem presença obrigatória. A jornada é pessoal; capítulos técnicos têm leitura independente. Não repetir essas decisões ao retomar.

Base factual, fontes e ressalvas estão na [FIC03-001 r01](<../../../registro da autoridade/publicacoes/01-novo-mundo-bagagem-antiga/ficha-editorial.md>). Relato de NFC-e em homologação não demonstra emissão em produção ou validação técnica nesta iniciativa. Detalhes pessoais novos exigem fonte; limitar recorte quando forem dispensáveis.

<a id="2-trabalho-recebido-e-rastreabilidade"></a>

## 2. Entregas e origem preservada

| Origem | Trabalho recebido | Destino e critério |
| --- | --- | --- |
| ENT-07 / T01-018 | Ficha final e referência de partida | T03-001: fontes/limites, voz, leitor e modos identificados, sem inventar fatos. |
| ENT-07 / T01-019 | Esboço, redação, revisão e integração do piloto | T03-002/003/004 e T03-009: artigo/chamada identificados, decisões de revisão e prova final da versão resultante do retorno/ajustes. |
| ENT-07 / T01-020 / PEN-03 | Apreciação autoral e ajustes | T03-005: retorno real sobre voz, clareza, interesse e esforço; ajustes e reconferência pertinentes. Ausência permanece pendente. |
| ENT-07 / T01-021 | Avaliação do método em uso | T03-006: ganhos/perdas, retrabalho e utilidade; distinguir contexto, procedimento, texto e retorno real. |

Os [REQ-01–20 da spec 01](../../concluida/01-sdd-editorial/01-especificacao-sdd-editorial.md#5-requisitos-do-método-e-critérios-de-avaliação-futura) continuam como critérios herdados; cobertura no plano, resultado nas tasks. Transferência não é execução ou dispensa.

## 3. Sequência, preservação e limites

Seguir o guia: preparar → esboço condicional → redigir → revisar → integrar → reconferir → autor → ajustes condicionais → prova final. Reconhecer a ficha, esboço e rascunho já produzidos pelas evidências, sem reiniciar por rotina. Conferir aspectos afetados pela mudança de método; parecer antigo não valida versão nova. Prova anterior ao autor, se houver, é apenas conferência técnica preliminar.

Versões de texto que precisem ser preservadas usam D05-01: conferir recuperação no Git, solicitar commit do autor se faltar e aguardar a edição dependente; continuar partes independentes. Não criar snapshots ou commits/pushes automáticos. Fontes, anexos e PUB-000 ficam preservados. Cada peça tem ID próprio no [índice](<../../../registro da autoridade/PUBLICACOES.md>); artigo/chamada em `registro da autoridade/publicacoes/01-novo-mundo-bagagem-antiga/`.

Revisores entregam parecer; integrador aplica decisões fundamentadas. Declarar contexto e histórico; papéis distintos não implicam independência. Uma rodada completa e outra dirigida podem ser proporcionais; instabilidade retorna ao esboço/spec em vez de polimento indefinido.

Avaliar a alteração que preserva sentido e a que exige reconsiderar a spec, herdadas de 01 seções 15.7/15.8, sem inventar vivências para produzi-las. Se um caso não ocorrer, individualizar cobertura ausente e destino antes de fechar a avaliação; não confundir preservação sem mudança de E07 com refatoração exercitada.

Estudo técnico, capítulos, calendário, GitHub/Pages e publicação ficam fora do piloto. Publicar exige instrução específica, revisão exata e destino. Não condicionar correção documental de 05 à apreciação deste texto.

## 4. Decisões de organização e vigência

**RA03-01 — 16/10/2026:** por pedido do autor, quinze fichas e EP-000 foram consolidados na jornada; publicações continuaram no acervo. T03-007 preserva essa execução como ocorrida; não é tarefa refeita em 05.

**RA03-02 — 16/10/2026:** retiradas sessões administrativas e modelo, mantendo RA02-11 na preparação 02 e decisões de consulta no mapa das ferramentas; versões anteriores no Git. T03-008 conserva resultado e limites originais. Evolução do método e reconciliação posteriores são trabalho de 05.

**Revisão v1.0 — 17/10/2026:** mesma IA com histórico, sem independência. Reconciliados escopo, origem e sequência com 05, retirados estados concorrentes e próximos passos antigos. Preservadas decisões de leitor/voz, IDs, critérios e fontes. T03-009 explicita a prova final posterior ao autor, sem apagar a origem T01-019. Esta revisão não aprovou a prosa, produziu chamada ou recebeu apreciação autoral. Próxima ação e liberação do método na tabela de tasks.

**RA03-03 — retorno e autorização de 17/10/2026:** o autor considerou o artigo frio/descritivo, com pouco humor, emoção, mundo paralelo e crescimento; solicita reescrita apoiada na direção narrativa já aceita. A chamada só será examinada depois do artigo. Autor dispensa commit da versão em andamento: não considera relevante guardar este rascunho ainda não aprovado e autoriza evoluir diretamente. Pode-se recomendar preservação quando uma mudança arriscar trabalho que valha comparar, mas uma decisão explícita do autor de não guardar permite continuar. Esta autorização prevalece sobre a espera local de D05-01 para a edição em questão; não autoriza commit automático ou inventar fatos. A sequência de apreciação passa a ser por peça, começando pelo artigo; acompanhamento nas tasks.

**RA03-04 — ponto de vista e próximo percurso, 17/10/2026:** o autor considerou r02 melhor e esclareceu que o narrador é o eu atual contando os dez meses iniciais. Aprender a iniciar com IA, harnesses e SDD já integra o percurso realizado; a etapa futura aprofunda a base teórica para compreender a prática e evoluir em engenharia agêntica. Propõe nível 10 como metáfora de iniciante que conhece parte da masmorra e precisa estudar para descer mais; o velho ermitão/sênior que aponta um erro com o nariz representa conhecimento amadurecido. Não são graduação, TCC realizado, competência medida ou cena autobiográfica. Ajustes diretos do artigo fornecem Misturador de Código, XP, perguntas da IA que não consegue decidir sozinho e intenção de compreender além do negócio/partes. Reescrita mantém autorização de evolução sem commit e chamada após artigo. Esta decisão amplia a base factual disponível e corrige o foco temporal; não inicia currículo, capítulo técnico ou publicação.

**RA03-05 — cronologia e motivo do aprofundamento, 17/10/2026:** autor esclarece que já usava IA muito antes em aplicações pessoais, scripts, integrações e automações pequenas; os dez meses referem-se ao início de uma aplicação grande para uso real. Quer abertura explicitamente pessoal, humor integrado e distinção entre contar/publicar material do percurso já realizado e registrar estudos futuros. A dimensão fiscal motiva teoria além do primeiro funcionamento: guardrails, segurança, auditoria, prevenção de falhas e recursos computacionais pouco visíveis. Registrar como objetivo e preocupação relatados, sem prontidão técnica ou controles implementados presumidos. Mantidos canal, fontes privadas protegidas, chamada posterior e evolução sem commit autorizada.

**RA03-06 — chamada autônoma, 17/10/2026:** autor rejeita PUB-002 r02 como resumo sem contexto e atrativo; solicita equipe editorial e um texto próprio que convide à história completa. A chamada deve desenvolver uma tensão pessoal com contexto e humor, deixando percurso/resultados para o artigo. Não precisa repetir dez meses, nível 10, métodos ou conclusões. Participação de agentes autorizada para esta rodada; não implica revisão cega ou aprovação por consenso. Artigo r05 apreciado permanece fora da reescrita.
