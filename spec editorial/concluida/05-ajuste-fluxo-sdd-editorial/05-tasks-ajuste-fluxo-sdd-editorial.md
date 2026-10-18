# Tasks 05 — Ajuste do fluxo SDD editorial

**ID:** TASKS-EDITORIAL-005  
**Versão:** 0.2 — 17/10/2026  
**Base:** [spec v0.6](05-spec-ajuste-fluxo-sdd-editorial.md) e [plano v0.1](05-plano-ajuste-fluxo-sdd-editorial.md).  
**Responsável:** mesma IA autora, implementadora e conferente, com histórico disponível; sem revisão independente.

| ID / entrega | Dependência | Critério de conclusão | Estado / evidência / próxima ação |
| --- | --- | --- | --- |
| T05-001 / ENT05-01 | Spec e plano conferidos | Entrada, autoridade, fases, preservação e sequência coerentes em AGENTS/README/guia. | Concluída: guia 1.0, README de navegação e AGENTS lidos entre si; fases e sequência 4.4/4.5 da spec atendidas. |
| T05-002 / ENT05-02 | T05-001 | Sete skills e seis modelos com contexto, ação, saída e limite; prova após retorno/ajustes; conferência estrutural e documental. | Concluída: skills de gestão v0.2 e editoriais v0.3, seis modelos simplificados e P09 v0.2. Sete validações estruturais PASS; contratos examinados conforme os casos abaixo. |
| T05-003 / ENT05-03 | T05-001/002 | Estado de 03 centralizado; IDs/resultados preservados; responsabilidades e prova final reconciliadas sem editar os corpos dos textos. | Concluída: spec 03 v1.0, plano v0.4, tasks v0.7, metadados da ficha e índice v0.5. T03-001–008 preservadas; T03-009 separa prova posterior ao autor. Notas de vigência em 01/04, sem reabrir aceitação histórica. |
| T05-004 / ENT05-04 | T05-001–003 | V05-01–08 conferidos no alcance disponível, referências válidas, pendências com destino e dependência de 03 atualizada. | Concluída: oito casos documentais conferidos com limites/destinos abaixo, 1.068 referências e 425 âncoras sem falha, sete skills válidas e 42 arquivos protegidos idênticos. Dependência de método da 03 liberada. |

**Pré-execução — 17/10/2026:** seleção de 05 e implementação autorizadas pelo pedido atual. Conferidos spec v0.6, plano v0.1 e esta decomposição: quatro entregas/tarefas, doze requisitos com destino, oito casos definidos previamente, sem ciclos ou arquivo de prosa previsto para edição. Fase muda de refinamento para implementação sem importar motor/gates de software. Não houve commit ou alteração do staging. Próxima ação: T05-001.

## Conferência operacional

| Caso | Resultado observado e evidência | Limite / destino |
| --- | --- | --- |
| V05-01 | Refinamento de 05 nas versões v0.1–0.6 permaneceu no backlog; o pedido atual selecionou execução e a mesma pasta foi movida para changes antes do plano/tasks. Guia seção 2 e README agora distinguem as fases. | Observação do fluxo desta iniciativa e conferência das instruções; não é autorização genérica de implementação após qualquer análise. |
| V05-02 | Entrada real para T03-003: tabela 03 → PUB-001 r01 e FIC03-001 r01 → decisões particulares RA02-10/14/15/16 e fontes que a ficha já seleciona. Próxima tarefa e espera por T05-004 localizadas sem ler quinze etapas; chamada inexistente, não redigida aqui. | Conferência documental de retomada; execução da chamada continua em 03. |
| V05-03 | Preparar v0.3/modelo ficha 0.4 separam pedido geral e escolha da peça; 02 é referência do piloto, não leitor/canal obrigatório. Para uma peça ainda não definida, a entrada pede intenção/material antes de escolher conteúdo. | Interface conferida; comportamento em nova peça real não exercitado. Destino: preparação da próxima peça, sem pretender eficácia geral. |
| V05-04 | A correção pontual de âncoras foi dirigida à navegação, sem nove pareceres; a mudança estrutural do guia foi examinada por sequência, autoridade e contratos antes de acabamento. Guia 5/6 e revisar v0.3 explicitam o mínimo e o aprofundamento. | Uso documental nesta correção; efeito em cadência/voz de artigo não examinado, permanece no piloto. |
| V05-05 | D05-01 aparece coerente em AGENTS, guia, integração, redação, planejamento e modelos. Os 42 Markdown protegidos de jornada/estudos e peças/esboço foram comparados antes/depois e permaneceram idênticos; a ficha recebeu só metadados de navegação/contexto histórico. Nenhuma revisão de prosa exigiu solicitar commit nesta execução. | Protocolo conferido; pedido real de commit para preservar uma revisão não exercitado. Destino: primeira edição dependente em 03 ou texto posterior, com solicitação ao autor se faltar versão no Git. |
| V05-06 | 01/04 receberam nota de vigência, conservando a aceitação histórica; 05 implementa o procedimento atual. T03-007/008 permanecem concluídas como ocorridas. A referência antiga de preservação ausente em 04 foi mantida como caminho histórico, sem recriar backup. | Evolução observada; aceitação invalidada por defeito não ocorreu. Se surgir, identificar evidência/aspecto e reabrir conforme o índice, sem afirmar cobertura desse caso em uso. |
| V05-07 | Guia 4 tem nove etapas na ordem acordada; ficha define natureza/tom, redação estrutura; reconferência precede autor e P09 sucede ajustes. Tasks 03 preservam os resultados e separam T03-009; modelos e perfis P09 apontam à versão resultante. | Conferência das orientações para história/técnica/mista; nenhuma peça nova ou leitura autoral simulada. Uso editorial completo será avaliado em 03. |
| V05-08 | Sete skills têm entrada, ação, saída e limite. Revisar entrega parecer; integrar decide/aplica; reconferir exige versão nova; lacuna tem retorno à fonte/spec/autor. Guia 5 centraliza a coordenação no plano/tasks, sem log intermediário. | Contratos documentais conferidos, sem alegar execução de todos os modos ou reação humana. Destino do uso real: etapas seguintes de 03. |

## Conferência e limites

Sete skills passaram no `quick_validate.py` com leitura UTF-8; PyYAML usado apenas como dependência temporária do validador fora do repositório. A primeira tentativa de leitura padrão encontrou problema de codificação, resolvido com `-X utf8`; não foi falha de conteúdo. Conferência estrutural não prova qualidade editorial.

Guia/README/AGENTS e interfaces foram lidos contra R05-01–12; nenhum requisito ficou sem entrega/tarefa. T05-001–004 concluídas no escopo documental. Varredura final: 1.068 referências locais e 425 âncoras, nenhum destino/âncora ausente; `git diff --check` dirigido passou. Duas âncoras antigas foram mantidas como aliases, evitando romper fontes históricas. Comparação dos 42 arquivos protegidos confirmou igualdade antes/depois, sem copiar suas versões para backup. Coberturas não exercitadas têm destino acima, sem impeditivo documental transferido. Não houve commit, push, motor do kit, script novo no repositório ou alteração de dados privados. Prosa e fontes transcritas preservadas; apreciação humana, chamada e eficácia editorial permanecem no piloto.

**Encerramento — 17/10/2026:** R05-01–12 cobertos pelas quatro entregas/tarefas e oito casos, sem impeditivo documental aberto. Cobertura não exercitada possui destino explícito na tabela, sem depender da leitura autoral para concluir 05. Método reconciliado; liberar a espera de 03 e retomar T03-003 no escopo autorizado de produção. A iniciativa é movida para concluida com seus links, sem commit, push ou publicação. Encerramento pela mesma IA implementadora/conferente, sem independência alegada.

**Pós-movimentação:** 1.068 referências locais e 425 âncoras válidas após o archive; 05 tem uma única localização em concluida. As quatro tasks estão concluídas, os doze requisitos mantêm cobertura e os oito casos têm resultado/limite. Os 42 arquivos protegidos continuam idênticos ao estado de entrada; nenhuma alteração de staging ou commit.
