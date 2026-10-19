# Spec 03 — Piloto editorial e avaliação do método

**ID:** SPEC-EDITORIAL-003. **Versão:** 1.7 — 18/10/2026.
**Estado:** encerrada em concluida; avaliação e limites no acompanhamento. Progresso e próxima ação somente nas [tasks 03](03-tasks-piloto-editorial.md). [Plano vigente](03-plano-piloto-editorial.md).
**Método vigente:** [guia](../../GUIA_DE_OPERACAO.md), reconciliado pela [iniciativa 05](<../../concluida/05-ajuste-fluxo-sdd-editorial/05-spec-ajuste-fluxo-sdd-editorial.md>). A implementação de 05 não é revisão da prosa do piloto.

## 1. Intenção, contexto e entradas

Aplicar o método a material real: [01 — Novo mundo, bagagem antiga](<../../../registro da autoridade/Template jornada do heroi/01-novo-mundo-bagagem-antiga.md>), comparar versões, receber retorno do autor e avaliar o texto e o esforço editorial. A etapa é contexto, não relato pronto; a cena no Reino dos Agentes é metáfora proposta.

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

## RA03-07 — Learn do piloto e propostas de melhoria — 18/10/2026

Pedido: fechar a sessão consolidando lições e aproveitar a skill learn do PDV D+, com cópia local quando útil. Consultada a fonte `.claude/skills/learn/SKILL.md`, sem executar automações do ERP ou alterar aquele projeto. Adaptada em [learn local](../../skills/learn/SKILL.md), com roteamento no AGENTS; aprendizado e encaminhamento permanecem aqui/nas tasks, não dentro da skill como diário. A regra da origem exige propor mudanças de orientação antes de aplicar; propostas abaixo foram autorizadas e aplicadas após o pedido “aplique as melhorias”; a adaptação/roteamento já estavam autorizados.

**Âncora:** commit `7bf9a221e46b6c9f7e927c024c435e2ef6ed0d7e`, identificado na conversa e conferido com `git show`, mais retornos autorais e PAR03-001. Artigo r05 e chamada r04 foram apreciados/provados; isso não apaga as rejeições intermediárias ou prova eficácia geral. Rascunhos evoluíram sem commits por decisão do autor: a comparação integral entre todas as revisões não é recuperável pelo Git e não será simulada.

### Lições observadas

| ID | Evidência e causa | Ganho observado / limite | Destino |
| --- | --- | --- | --- |
| LE03-01 | Artigo inicialmente considerado pronto pela IA foi rejeitado como frio e descritivo. A revisão privilegiou fidelidade e estrutura nominal, sem examinar suficientemente a intenção narrativa. | Retorno autoral levou a reescrita com progressão e imagens; satisfação só veio após ajustes. Não há medida de prazer de leitura do público. | Proposta A, preparar/revisar. |
| LE03-02 | Narrador inicialmente parecia começar agora; autor esclareceu presente após dez meses do projeto grande, uso anterior de IA e material já produzido ainda a publicar (RA03-04/05). | Separar presente do narrador, percurso passado e próxima formação corrigiu o foco, sem negar crescimento. É decisão desta peça; a regra reutilizável é conferir esses tempos. | Proposta A, preparar. |
| LE03-03 | Ficha da chamada r02 mandava percorrer usos menores, projeto, nível e teoria; texto foi rejeitado como resumo sem atrativo. A r03 ganhou tensão, mas precisou de contexto do protagonista/renascimento para chegar à r04 apreciada (RA03-06). | Função de convite exige contexto e curiosidade próprios; não basta reduzir o artigo. A equipe contribuiu com proposta/parecer, sem evidência causal de que mais agentes sempre melhoram texto. | Proposta B, redigir/revisar. |
| LE03-04 | D05-01 bloqueou evolução de rascunho que o autor não queria preservar. RA03-03 autorizou seguir sem commit e manter recomendação quando a comparação importar. | A exceção explícita permitiu continuar; a revisão não ficou recuperável integralmente. A autorização não deve virar dispensa automática de preservação em toda peça. | Proposta C, alinhar preservação. |
| LE03-05 | AGENTS/READMEs repetiam contexto/progresso. Foram simplificados e os textos finais perderam blocos de trabalho, mantendo apoio/fonte no lugar próprio. | Organização mais direta e peças prontas para leitura; navegação conferida. Instruções de leitura não foram medidas em outra sessão. | Já atendido; não criar outra regra ou relatório. |

### Propostas antes/depois — aprovadas e aplicadas em 18/10/2026

**A — preparação e revisão de narrativa**

- `editorial-preparar/SKILL.md`, ação 2. Antes: “Definir leitor, pergunta/contribuição, natureza [...] tom, formato/canal e limites conhecidos.” Depois, acrescentar: “Para relato retrospectivo, situar de quando o narrador conta, o que já aconteceu e o que ainda é intenção; definir a experiência de leitura desejada, além da informação a transmitir.”
- `editorial-revisar/SKILL.md`, parecer proporcional. Antes: “Mínimo: fidelidade à intenção/fontes/ressalvas, coerência e legibilidade.” Depois, acrescentar: “Em narrativa, examinar também o ponto de vista, a progressão e a função do humor ou emoção pedidos, com trechos; fidelidade factual isolada não atende à intenção narrativa. Se a vivência necessária não estiver disponível, delimitar a falta, sem inventá-la.”
- Ganho: orientar seleção e revisão pelo efeito solicitado. Custo: não transformar toda peça operacional em narrativa nem impor arco dramático.

**B — chamada como peça com função própria**

- `editorial-redigir/SKILL.md`, redação. Antes: orientação geral de transformar ficha/fontes em prosa. Depois, acrescentar: “Quando a chamada tiver função de convite, construir uma entrada com contexto, voz e motivo para seguir à peça completa. Não condensar mecanicamente os eixos do artigo; resumo só quando essa for a finalidade pedida.”
- `editorial-revisar/SKILL.md`, critério da chamada. Antes: “chamada não promete além da peça de origem”. Depois: “chamada não promete além da peça de origem e cumpre sua função particular; se for convite, examinar contexto do leitor e curiosidade preservada, sem exigir sinopse.”
- Ganho: corrigir a causa na ficha/redação e na revisão. Custo: não proibir resumo em peças cuja finalidade efetiva seja resumir, nem impor fórmula de gancho.

**C — preservação proporcional com decisão autoral explícita**

- AGENTS, guia seção 6 e cláusulas de preservação das skills preparar/redigir/integrar. Antes: se faltar recuperação no Git, solicitar commit e aguardar a edição dependente. Depois, acrescentar à regra aplicável: “Se o autor disser explicitamente que não quer preservar essa versão em andamento, registrar o alcance e continuar sem commit; não criar backup substituto nem presumir recuperação. Recomendar preservação quando a comparação tiver valor, sem repetir a decisão já recebida.”
- Ganho: reconciliar os pontos que ainda mandam aguardar com a decisão RA03-03. Custo: não extrapolar a dispensa para outra versão ou apagar trabalho considerado valioso sem autorização. O roteamento e o detalhe devem permanecer proporcionais, sem copiar um relato de sessão em todos os arquivos.

### Pendências e preferências

T03-006 continua responsável pela avaliação consolidada REQ-01–20, ganhos/perdas e cobertura; este learn fornece evidências parciais, não encerra a iniciativa. Não abriu backlog duplicado. Não houve achado pessoal privado que exigisse memória externa: voz é decisão editorial já na ficha/spec, e preservação é decisão operacional RA03-03. Nenhum arquivo de memória do Claude Code/Codex foi escrito. Sem novo commit, push ou publicação neste learn.

### Aplicação autorizada e adequação da learn — 18/10/2026

Pedido autoral explícito de aplicar A/B/C e conferir adequação ao projeto editorial. Preparar/redigir v0.4, revisar/integrar v0.5 e planejar v0.3 incorporam as orientações; AGENTS e guia v1.2 reconciliam a dispensa de preservação. Modelos de plano v0.3 e integração v0.5 foram alinhados para não restar espera incondicional de commit. Não foi aplicada nova direção às peças já aprovadas.

Learn v0.2 é específica para fluxo, regras, skills, coordenação e produção/revisão de texto. Explicita conhecimento de conteúdo com destino na jornada/estudos e distingue-o de regra operacional. Não exige aplicação, build, deploy, testes de software ou gate do PDV, não reescreve peça aprovada e não inicia estudo/pesquisa por consequência. Git é meio de rastreabilidade, não condição para diagnóstico; validação estrutural da skill não comprova eficácia editorial. A fonte do PDV permanece apenas referência histórica; nenhuma regra daquele projeto foi importada como obrigação.

A execução atual exercita o modo de aplicar melhorias identificadas após autorização, antes ainda pendente. Conferência documental dirigida prevista: narrativa retrospectiva versus documento operacional; convite versus resumo solicitado; preservação requerida versus dispensa específica; aprendizado de conteúdo versus regra do fluxo. Resultado estrutural e limites nas tasks. T03-006 continua em execução para matriz/parecer global, sem novo commit ou publicação automáticos.


**Parecer de encerramento — 18/10/2026:** escopo e critérios herdados examinados na matriz T03-006 das [tasks](03-tasks-piloto-editorial.md). Entregas concluídas com limites de cobertura individualizados; peças apreciadas e provadas, sem publicação. Não se declara eficácia geral do método. Preservadas decisões e evidências históricas acima; pendências antigas são lidas no contexto de sua data, com estado atual exclusivamente nas tasks.
