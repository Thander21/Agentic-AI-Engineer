# Tasks de implementação do SDD editorial

**ID:** TASKS-EDITORIAL-001  
**Versão:** 0.22 — auditada e arquivada como concluída
**Data da atualização:** 2026-10-14    
**Base:** [spec 01 — versão 0.7](01-especificacao-sdd-editorial.md) e [plano 01 — versão 0.5](01-plano-sdd-editorial.md)

**Estado:** iniciativa 01 encerrada no escopo autorizado de construção e avaliação inicial do método. T01-001 a T01-017 concluídas nos limites registrados; T01-018 a T01-021 transferidas, não executadas, para a spec 03. Próximo trabalho: análise da spec 02.

**Leitura do histórico:** registros anteriores descrevem a situação e o escopo da sua data. A decisão de separação abaixo substitui a obrigação de executar o piloto dentro de 01, preservando critérios e evidências.

## 1. Como acompanhar

Este documento reúne tarefas, execução, conferência e pendências. Foi elaborado manualmente antes da existência do modelo e da skill de tarefas. Sua compatibilidade com essas entregas foi conferida em T01-017, preservando IDs e histórico. O registro datado está na seção 6.

Todos os caminhos de saída em código continuam relativos a `spec editorial/`, salvo indicação contrária. Spec, plano e tasks foram arquivados em `spec editorial/concluida/01-sdd-editorial/`; os links Markdown foram ajustados ao local atual. Caminhos planejados não significam arquivos existentes. Os requisitos citados são os REQ da spec; as entregas ENT pertencem ao plano.

Estados: **pendente**, **em execução**, **produzida/aguardando conferência**, **concluída** ou **bloqueada com motivo**. Dependências futuras mantêm a tarefa pendente; ao tentar avançar e encontrar um impedimento, registrar o bloqueio concreto.

Nesta redistribuição autorizada, **transferida (não executada)** é uma situação administrativa: identifica saída do escopo e destino verificável, sem conclusão do trabalho. Não altera os estados de execução dos modelos ou das skills.

Cada tarefa só termina depois de produzir sua saída, conferir o critério e registrar evidência. A execução deve atualizar sua linha na seção 5 com artefato/versão, resultado, achados e próximo passo. Se uma alteração invalidar a conferência, reabrir a tarefa e preservar o registro anterior. Mudanças nos requisitos retornam à spec; mudanças de estratégia retornam ao plano.

**Responsabilidade padrão:** IA colaboradora executa e confere o escopo documental, declarando limites e acesso ao histórico. O autor fornece decisões editoriais, confirma vivências e avalia sua voz. Os papéis abaixo não pressupõem agentes separados nem execução paralela.

## 2. Guia e modelos

| ID | Entrega / requisitos | Dependências | Responsável | Saída prevista | Critério de conclusão |
| --- | --- | --- | --- | --- | --- |
| T01-001 | ENT-01; REQ-07 a 12, 15, 17 a 20 | Spec e plano de referência. | Editor do método. | `GUIA_DE_OPERACAO.md` | Explica início, contexto, percursos, papéis, preservação de versões e encerramento. Distingue estados das tasks, maturidade do conteúdo, apreciação autoral e publicação; permite determinar o próximo passo sem criar decisões do autor. |
| T01-002 | ENT-02; REQ-01 a 03, 09, 17 | T01-001. | Editor do método. | `modelos/spec.md` | Reúne análise, requisitos, regras, alternativas, pendências e revisão; registra achados e prontidão sem exigir documento adicional para análise. |
| T01-003 | ENT-02; REQ-09, 18 | T01-001, T01-002. | Planejador. | `modelos/plano.md` | Vincula versão da spec, entregas, caminhos, dependências e cobertura. Distingue pendência de planejamento de dependência do piloto. |
| T01-004 | ENT-02; REQ-09, 10, 19, 20 | T01-001, T01-003. | Coordenador das tarefas. | `modelos/tasks.md` | Inclui ID, requisito, entrega, dependência, papel, estado, saída, versão conferida, critério, evidência e pendências. Permite reabrir tarefa e manter histórico. |
| T01-005 | ENT-03; REQ-01 a 05, 07, 08, 11, 16 | T01-001. | Preparador editorial. | `modelos/ficha-editorial.md` | Oferece formas curta e completa; identifica intenção, fontes, vínculos, voz, esboço, fatos confirmados e lacunas. Aceita referências Markdown selecionadas sem depender de Obsidian ou inventar voz autoral. |
| T01-006 | ENT-03; REQ-02, 03, 04, 06, 11, 13, 16, 20 | T01-001, T01-005. | Revisor editorial. | `modelos/parecer-editorial.md` | Identifica papel, versão e contexto; registra problema, critério, sugestão, ganho, possível perda, importância e passagens a preservar. Declara exposição a outros pareceres e aspectos não avaliados. |
| T01-007 | ENT-03; REQ-04, 09, 10, 14, 15, 16, 20 | T01-005, T01-006. | Editor integrador. | `modelos/integracao-e-avaliacao.md` | Registra destino dos achados, conflitos, versões, efeitos das mudanças e reconferências. Separa avaliação documental, funcionamento das skills e retorno humano. |

## 3. Construção das skills

Em cada tarefa desta seção, seguir o contrato da seção 5.2 do plano e a orientação de autoria de skills disponível no ambiente. Conferir frontmatter, nome, descrição, links, modos e ausência de instruções incompletas. O critério destas tarefas é a construção documental; a avaliação de comportamento ocorre em T01-016. Não declarar qualidade de uso comprovada ao concluir somente a construção.

As fontes de orientação e os limites de seus validadores estão na seção 8. Usar o guia de autoria do ambiente Codex como referência principal; consultar materiais complementares criticamente, sem importar ferramentas, campos ou fluxos de outro ambiente por simples cópia.

| ID | Entrega / requisitos | Dependências | Responsável | Saída prevista | Critério de conclusão |
| --- | --- | --- | --- | --- | --- |
| T01-008 | ENT-04; REQ-01, 02, 03, 09, 17 | T01-001 a T01-004, T01-006. | Autor de skills. | `skills/sdd-editorial-especificar/SKILL.md` | Distingue analisar, elaborar e revisar; conserva achados na spec; trata contradições, sugestões e decisões pendentes sem expandir a fase solicitada. |
| T01-009 | ENT-04; REQ-09, 18 | T01-001 a T01-004, T01-006. | Autor de skills. | `skills/sdd-editorial-planejar/SKILL.md` | Recebe spec identificada, reconfere mudanças relevantes, cobre requisitos e dependências e devolve alterações de escopo à spec. |
| T01-010 | ENT-04; REQ-09, 10, 19, 20 | T01-001 a T01-004, T01-006. | Autor de skills. | `skills/sdd-editorial-tarefas/SKILL.md` | Distingue decomposição e acompanhamento; exige resultado e evidência para conclusão, encaminha a produção e reabre conferências invalidadas. |
| T01-011 | ENT-05; REQ-01 a 05, 07, 08, 11 | T01-001, T01-005 a T01-007. | Autor de skills. | `skills/editorial-preparar/SKILL.md` | Seleciona contexto proporcional e fontes localizadas; produz ficha; pergunta por dados essenciais sem inventar vivências nem importar todo o acervo. |
| T01-012 | ENT-05; REQ-01 a 05, 08, 12, 16 | T01-001, T01-005 a T01-007. | Autor de skills. | `skills/editorial-redigir/SKILL.md` | Distingue esboço e rascunho, documento operacional e narrativa; respeita voz e fontes, permite descoberta e devolve mudanças de intenção à ficha. |
| T01-013 | ENT-05; REQ-02 a 06, 11 a 13, 16, 20 | T01-001, T01-005 a T01-007. | Autor de skills e revisor editorial. | `skills/editorial-revisar/SKILL.md` e `references/perfis.md` nessa pasta. | Define os nove perfis do plano, suas perguntas, contexto e limites; um perfil por leitura, parecer sem edição do original, preservação do que funciona e ausência de aprovação factual sem fontes. Referências são carregadas conforme necessidade. |
| T01-014 | ENT-05; REQ-04, 05, 09, 10, 14, 15, 20 | T01-001, T01-005 a T01-007. | Autor de skills. | `skills/editorial-integrar/SKILL.md` | Confere versão dos pareceres, resolve conflitos por intenção e evidência, preserva a versão anterior, registra decisões e encaminha reconferência de mudanças de sentido. |

## 4. Conferência integrada e piloto

T01-015 a T01-017 pertencem ao escopo encerrado. As definições de T01-018 a T01-021 abaixo são preservadas como contratos de origem, transferidos à spec 03. Suas antigas dependências recebem agora as definições e a análise de cobertura da spec 02.

| ID | Entrega / requisitos | Dependências | Responsável | Saída prevista | Critério de conclusão |
| --- | --- | --- | --- | --- | --- |
| T01-015 | ENT-06; REQ-01 a 20 | T01-001 a T01-014. | Revisor do conjunto. | Estado na seção 5; resultado e achados na seção 6. | Confere caminhos, referências, cobertura dos vinte requisitos e passagem de contexto entre artefatos. Verifica estrutura das skills com recurso disponível quando aplicável; distingue essa conferência de avaliação de comportamento. Resolve impeditivos ou reabre tarefas afetadas. |
| T01-016 | ENT-06; REQ-01 a 20 | T01-015. | Avaliador dos procedimentos. | Registro de exercícios e cobertura na seção 6. | Aplica os casos da seção 5.4 do plano, com entradas e resultados observados; registra limitações e cobre os modos/perfis destinados ao primeiro uso. Corrige e reconfere impeditivos antes de marcar as skills pertinentes como prontas para piloto. |
| T01-017 | ENT-06; REQ-17 a 20 | T01-010, T01-015, T01-016. | Coordenador das tarefas. | Este documento conferido contra modelo e skill produzidos. | Reconcilia o acompanhamento inicial com o procedimento implementado, preservando IDs, versões e evidências; confirma que as conferências exigidas estão registradas e não apenas marcadas como feitas. |
| T01-018 | ENT-07; REQ-01 a 05, 08, 11, 16 | T01-017 e decisões necessárias da spec 02. | Autor e preparador editorial. | Ficha do piloto, em local definido no 02; localização registrada aqui. | Confirma onde, como e quando, voz e fatos disponíveis; preserva o texto 01 de referência; identifica critérios e perfis escolhidos. Perfis não exercitados em T01-016 retornam para avaliação antes do uso. |
| T01-019 | ENT-07; REQ-01 a 16, 20 | T01-018. | Redator, revisores e editor integrador. | Rascunho, pareceres e versão integrada do piloto; locais registrados aqui. | Executa o ciclo previsto, registra ganho/perda das sugestões e trechos preservados, resolve impeditivos e compara versões. Resultado pronto para leitura autoral; sem presumir publicação ou aprovação. |
| T01-020 | ENT-07; REQ-04, 08, 16, 20 | T01-019 e retorno do autor. | Autor e editor integrador. | Avaliação autoral e decisões no registro de integração. | Registra percepção real de voz, clareza, prazer de leitura e esforço; encaminha ajustes solicitados. Enquanto o retorno não vier, a avaliação autoral permanece pendente e ENT-07 não está concluída. |
| T01-021 | ENT-07; REQ-09, 14, 15, 17 a 20 | T01-020. | Editor do método. | Síntese de avaliação e ajustes nos documentos afetados. | Separa suficiência da spec, funcionamento das skills e qualidade do texto. Incorpora correções necessárias e reconfere o que mudou; registra sugestões futuras separadamente e conclui somente o escopo efetivamente demonstrado. |

Os exercícios de T01-016 usam material sintético ou recortes permitidos, preservando os originais. Não antecipam a redação do piloto. A verificação de T01-018 recebe decisões do 02; não autoriza defini-las pelo autor nem exige concluir o calendário inteiro de postagens.

## 5. Estado, execução e evidências

O critério específico está nas seções 2 a 4. Ao executar, substituir “não produzido” pelo caminho real e versão examinada. Acrescentar histórico datado abaixo da tabela quando houver correção, reabertura ou múltiplas conferências; não apagar uma evidência anterior para simular uma execução sem falhas.

| Tarefa | Estado | Artefato / versão conferida | Conferência e evidência | Pendências / próximo passo |
| --- | --- | --- | --- | --- |
| T01-001 | Concluída | [GUIA_DE_OPERACAO.md](../../GUIA_DE_OPERACAO.md), v0.4. | Evidências anteriores preservadas; navegação do guia v0.4 reconferida no arquivamento, seção 11. | Percurso curto exercitado em T01-016; uso real transferido para 03. |
| T01-002 | Concluída | [modelos/spec.md](../../modelos/spec.md), v0.1. | Conferência documental de 2026-10-13 registrada abaixo; link para o guia válido. | Conjunto conferido em T01-015; exercícios e limites registrados em T01-016; uso real pendente. |
| T01-003 | Concluída | [modelos/plano.md](../../modelos/plano.md), v0.1. | Conferência documental de 2026-10-13 registrada abaixo; 2 links locais válidos. | Conjunto conferido em T01-015; exercícios e limites registrados em T01-016; uso real pendente. |
| T01-004 | Concluída | [modelos/tasks.md](../../modelos/tasks.md), v0.1. | Conferência documental de 2026-10-13 registrada abaixo; 2 links locais válidos. | Compatibilidade conferida em T01-017; ver registro na seção 6. |
| T01-005 | Concluída | [modelos/ficha-editorial.md](../../modelos/ficha-editorial.md), v0.1. | Conferência documental de 2026-10-13 registrada abaixo; 2 links locais válidos. | Conjunto conferido em T01-015; exercícios e limites registrados em T01-016; uso real pendente. |
| T01-006 | Concluída | [modelos/parecer-editorial.md](../../modelos/parecer-editorial.md), v0.1. | Conferência documental de 2026-10-13 registrada abaixo; 2 links locais válidos. | Conjunto conferido em T01-015; exercícios e limites registrados em T01-016; uso real pendente. |
| T01-007 | Concluída | [modelos/integracao-e-avaliacao.md](../../modelos/integracao-e-avaliacao.md), v0.1. | Conferência documental de 2026-10-13 registrada abaixo; 3 links locais válidos. | Conjunto conferido em T01-015; exercícios e limites registrados em T01-016; uso real pendente. |
| T01-008 | Concluída | [sdd-editorial-especificar/SKILL.md](../../skills/sdd-editorial-especificar/SKILL.md), v0.1. | Validador estrutural aprovado; 3 referências válidas; conferência documental de 2026-10-13 abaixo. | Comportamento exercitado em T01-016; consultar cobertura e limites por modo. |
| T01-009 | Concluída | [sdd-editorial-planejar/SKILL.md](../../skills/sdd-editorial-planejar/SKILL.md), v0.1. | Validador estrutural aprovado; 3 referências válidas; conferência documental de 2026-10-13 abaixo. | Comportamento exercitado em T01-016; consultar cobertura e limites por modo. |
| T01-010 | Concluída | [sdd-editorial-tarefas/SKILL.md](../../skills/sdd-editorial-tarefas/SKILL.md), v0.1. | Validador estrutural aprovado; 3 referências válidas; registro de conclusão em 2026-10-14 abaixo. | Comportamento exercitado em T01-016; consultar cobertura e limites por modo. |
| T01-011 | Concluída | [editorial-preparar/SKILL.md](../../skills/editorial-preparar/SKILL.md), v0.1. | Validador estrutural aprovado; 3 referências válidas; conferência documental de 2026-10-14 abaixo. | Comportamento exercitado em T01-016; consultar cobertura e limites por modo. |
| T01-012 | Concluída | [editorial-redigir/SKILL.md](../../skills/editorial-redigir/SKILL.md), v0.1. | Validador estrutural aprovado; 3 referências válidas; conferência documental de 2026-10-14 abaixo. | Comportamento exercitado em T01-016; consultar cobertura e limites por modo. |
| T01-013 | Concluída | [editorial-revisar/SKILL.md](../../skills/editorial-revisar/SKILL.md) e [perfis.md](../../skills/editorial-revisar/references/perfis.md), v0.1. | Validador estrutural aprovado; referências válidas e nove perfis conferidos; registro de 2026-10-14 abaixo. | Nove perfis exercitados em T01-016; avaliação guiada e limites registrados. |
| T01-014 | Concluída | [editorial-integrar/SKILL.md](../../skills/editorial-integrar/SKILL.md), v0.1. | Validador estrutural aprovado; 3 referências válidas; conferência documental de 2026-10-14 abaixo. | Comportamento exercitado em T01-016; consultar cobertura e limites por modo. |
| T01-015 | Concluída | Guia v0.2; seis modelos v0.1; sete skills e perfis v0.1; spec 0.5 e plano 0.3 com referências de navegação atualizadas. | Conferência de 2026-10-14 abaixo: 7 validações estruturais, 88 links locais válidos, cobertura documental de 20 requisitos. | Uso real e comportamento não comprovados por esta conferência. |
| T01-016 | Concluída | [Entradas, saídas e cobertura](../../avaliacoes/T01-016/README.md). | Exercícios E01–E07; correção dirigida de E03 no arquivo de saídas r1.1 e reconferência da seção 11; limites por modo preservados. | Conclusão restrita ao recorte exercitado, pela mesma IA. Modos adicionais exigem complemento antes do uso; ver PEN-02. |
| T01-017 | Concluída | Este documento, v0.22; modelo e skill de tasks v0.1. | Reconciliação histórica na seção 6; reexame dirigido após correção de E03 e arquivamento na seção 11. | Preparar definições da spec 02 para T01-018; ver PEN-01. |
| T01-018 | Transferida (não executada) | [Spec 03 v0.1, seção 2](../../changes/03-piloto-editorial/03-piloto-editorial.md#2-trabalho-recebido-e-rastreabilidade). | Contrato de preparação preservado; ficha não produzida. | Receber contexto e cobertura analisados na spec 02; executar na iniciativa 03. |
| T01-019 | Transferida (não executada) | [Spec 03 v0.1](../../changes/03-piloto-editorial/03-piloto-editorial.md). | Contrato de produção/revisão preservado; piloto não escrito. | Planejar e executar em 03 após preparação suficiente. |
| T01-020 | Transferida (não executada) | [Spec 03 v0.1](../../changes/03-piloto-editorial/03-piloto-editorial.md). | Critério de apreciação humana preservado; retorno ainda não obtido. | Autor avalia o piloto na iniciativa 03. |
| T01-021 | Transferida (não executada) | [Spec 03 v0.1](../../changes/03-piloto-editorial/03-piloto-editorial.md). | Avaliação aplicada e ajustes do método preservados como trabalho futuro. | Consolidar resultados e ajustes em 03, reabrindo aspectos de 01 se necessário. |

## 6. Registros de execução e conferência

### Conferência documental de T01-001 — 2026-10-13

Guia v0.1 elaborado e relido contra o critério da tarefa, o plano 0.3 e as regras da spec 0.5. Evidências: início e roteamento na seção 1; contexto e lacunas na 2; percursos na 3; papéis e passagens na 4; pareceres na 5; preservação de versões e integração na 6; estados separados na 7; encerramento na 8; condições do piloto e próximo passo na 9. Os estados do conteúdo foram confrontados com a base do livro. Os cinco links locais foram conferidos e seus destinos existem.

Resultado: critério documental atendido, sem impeditivo identificado. Conferência feita pela mesma IA que redigiu, com acesso ao histórico; não é avaliação independente nem aplicação real do guia. Modelos, skills e exercícios continuam pendentes. Esta evidência conclui somente T01-001.

### Conferência documental de T01-002 — 2026-10-13

Modelo v0.1 elaborado e relido contra a tarefa, a seção 17 da spec e o guia. A análise permanece nas seções 1 e 2 do modelo; escopo, requisitos e regras nas 3 a 5; alternativas e pendências nas 6 e 7; revisão e parecer na 8; mudanças e impactos na 9. Público e contribuição são explícitos, fontes têm localização e situação de conferência, propostas não são equiparadas a decisões e critérios literários não exigem nota automática.

A passagem ao plano depende de revisão registrada; o modelo começa com parecer não avaliado. Pendências de etapas posteriores podem permanecer sem impedir o plano quando seu impacto estiver identificado. Instruções de cópia alertam para ajustar caminhos e remover campos demonstrativos; o único link real aponta para o guia existente e foi conferido.

Resultado: critério documental atendido, sem impeditivo identificado. Revisão pela mesma IA que redigiu, com acesso ao histórico; não foi executada uma skill nem preenchida uma spec piloto. T01-002 concluída apenas no escopo de criação e conferência do modelo.

### Conferência documental de T01-003 — 2026-10-13

Modelo de plano v0.1 elaborado e relido contra o critério da tarefa, o guia e a passagem spec → plano definida no modelo de spec. Cabeçalho identifica versão e parecer de origem; seções 1 e 2 delimitam escopo e decisões de implementação; 3 e 4 definem entregas, caminhos, dependências e condições de avanço; 5 explicita contexto e procedimentos; 6 mapeia requisitos; 7 define conferências; 8 distingue pendências de planejamento das de execução/piloto; 9 registra revisão e prontidão; 10 trata impactos sobre documentos derivados.

O parecer começa não avaliado, a criação de skills é condicional e as evidências de execução ficam nas tasks. Os dois links do modelo foram conferidos e apontam para arquivos existentes. Resultado: critério documental atendido, sem impeditivo identificado. Conferência pela mesma IA autora, com acesso ao histórico; nenhuma avaliação de comportamento ou piloto foi executada. T01-003 concluída no escopo de criação e conferência do modelo.

### Conferência documental de T01-004 — 2026-10-13

Modelo de tasks v0.1 elaborado e relido contra o critério da tarefa, os estados do guia e a passagem plano → tasks. Cabeçalho identifica spec/plano e versões; seção 2 inclui ID, entrega, requisitos, dependências, papel, saída e critério; seções 3 e 4 distinguem produção, conferência e conclusão; seção 5 registra versão examinada, evidências, limites e decisões; seção 6 preserva motivo e condição de retomada nas reaberturas; seção 7 trata exercícios quando pertinentes; seções 8 e 9 registram cobertura, próximo trabalho e histórico.

Campos de execução começam não realizados e não há aprovação automática. Evidências anteriores devem ser preservadas ao mudar um estado. Os dois links locais foram conferidos e apontam para arquivos existentes. Resultado: critério documental atendido, sem impeditivo identificado. Revisão pela mesma IA autora, com acesso ao histórico; não foi executada skill nem avaliação comportamental. A reconciliação destas tasks com o modelo e a futura skill continua reservada a T01-017.

### Conferência documental de T01-005 — 2026-10-13

Ficha v0.1 elaborada e relida contra a tarefa, o guia e os contratos de contexto do plano. A forma curta reúne intenção, base, direção e critérios com identificação e pendências. A forma completa explicita destino, leitor, escopo, vínculos, fontes localizadas, natureza das afirmações, voz, amostras Markdown, esboço, liberdade criativa, perfis de revisão, lacunas e histórico. Ambas começam sem prontidão presumida.

Conferidos os limites: amostras do Obsidian não exigem integração, notas rápidas não viram estilo obrigatório, fatos pessoais ausentes não são preenchidos por invenção e o esboço não impõe derrota ou humor. Pendências distinguem informação essencial de lacuna compatível com rascunho marcado. Os dois links locais apontam para arquivos existentes.

Resultado: critério documental atendido, sem impeditivo identificado. Conferência pela mesma IA autora, com acesso ao histórico. Nenhuma ficha real foi preenchida, nenhuma preferência do documento 02 foi decidida e o piloto permanece pendente. Avaliação de comportamento e uso integrado ocorrerão posteriormente.

### Conferência documental de T01-006 — 2026-10-13

Parecer v0.1 elaborado e relido contra a tarefa, o guia e os critérios de revisão da ficha editorial. Cabeçalho e seção 1 identificam papel, versão, contexto, critérios, acesso a outros pareceres e limitações; seção 2 começa sem avaliação presumida; seção 3 contém problema, fonte/critério, sugestão, ganho, possível perda e importância; seção 4 permite preservar passagens; seção 5 distingue apreciação humana de percepção da IA; seções 6 e 7 encaminham integração e reconferências com versão identificada.

O modelo não autoriza modificar o original durante o parecer, não impõe quantidade de achados e distingue erro de preferência. Os dois links locais foram conferidos e seus destinos existem. Resultado: critério documental atendido, sem impeditivo identificado. Revisão pela mesma IA autora, com acesso ao histórico; nenhum parecer de texto real, exercício de skill ou piloto foi executado.

### Conferência documental de T01-007 — 2026-10-13

Modelo de integração v0.1 elaborado e relido contra a tarefa, o guia, a ficha e o contrato dos pareceres. Identificação e seção 1 delimitam versão recuperável, intenção e elementos a preservar; seções 2 a 4 verificam a aplicabilidade dos pareceres e registram destino dos achados e conflitos; seção 5 compara versões e impactos; seção 6 trata reconferência e leitura do conjunto; seção 7 separa orientação documental, funcionamento dos procedimentos, qualidade do texto, apreciação humana e esforço; seções 8 e 9 registram encerramento e histórico.

Referências a achados incluem ID do parecer para evitar colisões entre ACH-01 de revisores diferentes. Acolher, aplicar e conferir são acontecimentos distintos. Retorno humano ausente permanece pendente e publicação não é presumida. Os três links locais foram conferidos e seus destinos existem. Resultado: critério documental atendido, sem impeditivo identificado. Revisão pela mesma IA autora, com acesso ao histórico; nenhuma integração de texto real, skill ou piloto foi executada.

### Conferência documental de T01-008 — 2026-10-13

Skill v0.1 criada com frontmatter de nome, descrição e versão. Modos analisar, elaborar e revisar têm entradas, saídas e limites distintos; referências ao guia, ao modelo de spec e ao parecer são condicionais ao trabalho. Conferidos escopo, tratamento de conflitos e lacunas, preservação dos IDs, revisão de mudanças e critérios de prontidão. A descrição é não vazia e discrimina revisão de spec de redação ou edição linguística; o nome corresponde à pasta. Exemplo incluído como ilustração, não como resultado observado.

O primeiro comando do validador falhou por ausência do módulo `yaml`. Instalado PyYAML 6.0.3 somente em `%TEMP%/sdd-editorial-validator-deps`; o `quick_validate.py` do skill-creator foi reexecutado via Python com essa pasta no caminho de importação e retornou `Skill is valid!` (saída 0). Três referências locais foram conferidas e existem. Não houve instalação global da skill nem configuração de descoberta automática.

Resultado: construção e conferência documental atendidas, sem impeditivo identificado nesse escopo. Revisão pela mesma IA autora, com acesso ao histórico. Nenhum exercício comportamental foi executado; a skill ainda não foi declarada pronta para piloto. T01-016 verificará suas decisões em uso.

### Conferência documental de T01-009 — 2026-10-13

Skill de planejamento v0.1 criada e relida contra o contrato do plano, o modelo de plano e os limites da skill de especificação. Recebe spec e parecer identificados, reconfere mudanças relevantes, define entregas/caminhos/dependências, mapeia requisitos e devolve mudanças de intenção à spec. Distingue criar, ajustar e conferir; não gera tasks ou implementação automaticamente. O exemplo de dependência editorial futura está identificado como ilustrativo.

Frontmatter com nome e descrição não vazios, nome correspondente à pasta e versão identificada. `quick_validate.py` executado com a dependência YAML isolada já disponível em `%TEMP%/sdd-editorial-validator-deps`: resultado `Skill is valid!`, saída 0. Três referências locais conferidas e existentes. Nenhuma instalação global ou configuração de descoberta automática foi realizada.

Resultado: construção e conferência documental atendidas, sem impeditivo identificado nesse escopo. Revisão pela mesma IA autora, com acesso ao histórico. Exercícios comportamentais e prontidão para piloto continuam reservados a T01-016.

### Conferência documental de T01-010 — registro concluído em 2026-10-14

Skill de tarefas v0.1 criada antes da interrupção e seu arquivo confirmado na retomada. Os modos decompor, acompanhar e conferir acompanhamento têm entradas e saídas distintas. O procedimento exige versão e evidência para concluir, preserva IDs e histórico, diferencia dependência futura de bloqueio observado e reabre conferências afetadas por mudanças. Não inicia redação ou implementação apenas por receber um pedido de listar tarefas.

Na execução anterior à retomada, `quick_validate.py` retornou `Skill is valid!` com saída 0, usando a dependência YAML isolada em `%TEMP%/sdd-editorial-validator-deps`. As três referências locais foram conferidas e existem. Nome e descrição estão preenchidos, o nome corresponde à pasta e o exemplo está identificado como ilustrativo. Não houve instalação global nem configuração de descoberta automática.

Resultado: construção e conferência documental atendidas, sem impeditivo identificado nesse escopo. Revisão pela mesma IA autora, com acesso ao histórico. A retomada conclui o registro que faltava nas tasks; não representa nova avaliação comportamental. T01-016 continua pendente, e a reconciliação do acompanhamento com a skill será tratada em T01-017.

### Conferência documental de T01-011 — 2026-10-14

Skill de preparação editorial v0.1 criada e relida contra a tarefa, o contrato do plano e as formas da ficha. Define seleção proporcional de contexto, localização das fontes, distinção entre relato/hipótese/ficção, vínculos com a jornada e tratamento das amostras de voz. Lacunas são separadas por efeito na redação ou na revisão, com perguntas localizadas e sem invenção de fatos pessoais. O procedimento não inicia redação nem presume decisões pendentes do documento 02.

Nome e descrição preenchidos, nome correspondente à pasta e versão identificada. `quick_validate.py` executado com YAML isolado em `%TEMP%/sdd-editorial-validator-deps`: `Skill is valid!`, saída 0. As três referências locais foram conferidas e existem. Sem instalação global ou configuração de descoberta automática.

Resultado: construção e conferência documental atendidas, sem impeditivo identificado nesse escopo. Revisão pela mesma IA autora, com acesso ao histórico; exemplo apenas ilustrativo. Nenhuma ficha real ou exercício comportamental foi produzido com a skill. Avaliação em uso continua pendente em T01-016.

### Conferência documental de T01-012 — 2026-10-14

Skill de redação v0.1 criada e relida contra a tarefa e o contrato do plano. Distingue esboço, rascunho e trecho delimitado, além de narrativa, explicação técnica e documento operacional. Define entradas da ficha, preservação de fontes e ressalvas, voz baseada nas escolhas do autor, liberdade criativa sem invenção autobiográfica e encaminhamento de mudanças de intenção. Pendências ficam explícitas e a leitura de entrega não é apresentada como revisão especializada completa.

Nome e descrição preenchidos, nome correspondente à pasta e versão identificada. `quick_validate.py` executado com YAML isolado em `%TEMP%/sdd-editorial-validator-deps`: `Skill is valid!`, saída 0. As três referências locais foram conferidas, incluindo o caminho do universo narrativo. Sem instalação global ou configuração de descoberta automática.

Resultado: construção e conferência documental atendidas, sem impeditivo identificado nesse escopo. Revisão pela mesma IA autora, com acesso ao histórico. Nenhum episódio, rascunho do piloto ou exercício comportamental foi executado; exemplo apenas ilustrativo. A qualidade literária e o comportamento continuam sujeitos à avaliação posterior.

### Conferência documental de T01-013 — 2026-10-14

Skill de revisão e referência de perfis v0.1 criadas e relidas contra a tarefa, o contrato do plano e o modelo de parecer. Definidos P01 a P09: estrutura, fatos/fontes, didática, continuidade, voz/tom, linha/fluidez, preparação linguística, leitura crítica e prova. Cada perfil contém situação de uso, contexto, perguntas, saída específica e limites. A skill orienta um perfil por leitura, seleção proporcional, parecer sem edição direta, ganho/perda das sugestões e preservação do que funciona.

Nome e descrição preenchidos, nome correspondente à pasta e versões identificadas. `quick_validate.py` com YAML isolado retornou `Skill is valid!`, saída 0. As referências dos dois arquivos foram conferidas e existem; nove seções de perfis identificadas. Nenhuma instalação global ou configuração de descoberta automática.

Resultado: construção e conferência documental atendidas, sem impeditivo identificado nesse escopo. Revisão pela mesma IA autora, com acesso ao histórico. Perfis não foram exercitados em texto real ou sintético; a contagem e a leitura das seções não comprovam qualidade de revisão. T01-016 deverá registrar separadamente a cobertura de comportamento de cada perfil utilizado.

### Conferência documental de T01-014 — 2026-10-14

Skill de integração v0.1 criada e relida contra a tarefa, o contrato do plano e o modelo de integração. Define versão de partida recuperável, pertinência de pareceres, referência completa dos achados, decisões com ganho/perda, tratamento de conflitos por intenção/evidência/voz e refatoração proporcional. Distingue acolher, aplicar e conferir, preserva ressalvas e encaminha mudanças de sentido à revisão pertinente. Avaliação documental, comportamento, qualidade textual e apreciação humana permanecem separados.

Nome e descrição preenchidos, nome correspondente à pasta e versão identificada. `quick_validate.py` com YAML isolado retornou `Skill is valid!`, saída 0. Três referências locais conferidas e existentes. Nenhuma instalação global ou configuração de descoberta automática.

Resultado: construção e conferência documental atendidas, sem impeditivo identificado nesse escopo. Revisão pela mesma IA autora, com acesso ao histórico. Nenhuma integração de texto real ou avaliação comportamental foi executada. As sete skills estão construídas; a conferência integrada de T01-015 e os exercícios de T01-016 continuam pendentes.

### Conferência integrada de T01-015 — 2026-10-14

Escopo: guia, seis modelos, sete skills, nove perfis e sua ligação com spec/plano/tasks. Foram examinados contratos de entrada/saída, dependências, estados, referências e cobertura. Não houve execução dos exercícios de comportamento.

| Achado | Correção | Reconferência |
| --- | --- | --- |
| Dois links da spec apontavam para a pasta antiga `Livro`. | Destinos ajustados para `capitulos estudos/ESTRUTURA_E_ESTUDO.md`, presente no workspace. Nenhum arquivo do acervo foi movido. | Destinos existem; varredura de links passou. |
| A tabela do guia podia sugerir que revisores estruturais e de acabamento aplicavam mudanças diretamente. | Guia v0.2 explicita parecer → integração → nova versão antes da próxima passagem. | Releitura contra `editorial-revisar`, `editorial-integrar` e modelo de integração: responsabilidade coerente. T01-001 reconferida no aspecto afetado. |
| Guia e plano ainda indicavam recursos inexistentes e próximo trabalho T01-001/T01-002. | Guia aponta para perfis existentes; progresso fica nas tasks. Plano mantém sua estratégia e remete ao acompanhamento atual. | Sem mudança de requisitos, agrupamento ou estratégia; correções de situação e navegação. |

Os sete `SKILL.md` passaram no `quick_validate.py`, usando a dependência YAML isolada já registrada. Nomes e pastas foram confrontados. Após as correções, foram conferidos 19 documentos Markdown do conjunto e 88 referências locais, todas com destino existente. Confirmados seis modelos, sete skills, nove seções de perfis e vinte requisitos no mapeamento do plano. As contagens verificam estrutura e navegação, não qualidade literária.

#### Cobertura documental observada

Os caminhos de modelos são relativos a `modelos/`; nomes de skills referem-se a `skills/<nome>/SKILL.md`. Esta matriz registra instruções e campos existentes, não atendimento em uso.

| Requisito | Evidência localizada |
| --- | --- |
| REQ-01 | `ficha-editorial.md`, intenção/leitor; `editorial-preparar`, delimitar intenção. |
| REQ-02 | Ficha completa, seção 3; `editorial-preparar`, fontes; perfil P02. |
| REQ-03 | Ficha, natureza e situação das afirmações; `editorial-redigir`, verdade do relato. |
| REQ-04 | Ficha, voz e liberdade; `editorial-integrar`, preservação; integração, apreciação humana. |
| REQ-05 | Ficha, escopo e relações; perfil P04; integração, impactos. |
| REQ-06 | Parecer identifica perfil e escopo; `editorial-revisar`, uma leitura por perfil. |
| REQ-07 | Guia, identificação e vínculos; ficha, reaproveitamento sem duplicação de experiência. |
| REQ-08 | Guia, percurso leve/completo; ficha, formas curta/completa. |
| REQ-09 | Modelos de spec/plano/tasks, histórico e impactos; integração, comparação entre versões. |
| REQ-10 | Guia, estados separados; tasks, produção/conferência; integração, publicação e retorno autoral. |
| REQ-11 | Parecer, cabeçalho e contexto; skill de revisão, limites e versão. |
| REQ-12 | Guia v0.2, estrutura antes do acabamento com integração explícita; perfil P01. |
| REQ-13 | Perfis P05, P06 e P07; parecer, natureza do achado e preferência expressiva. |
| REQ-14 | Integração, versões e elementos a preservar; skill de integração, refatoração e reconferência. |
| REQ-15 | Guia, encerramento; integração, destino dos achados e conflitos. |
| REQ-16 | Parecer, apreciação qualitativa; perfil P08; integração, retorno humano distinto de percepção da IA. |
| REQ-17 | Modelo de spec, análise e revisão no mesmo documento; `sdd-editorial-especificar`. |
| REQ-18 | Modelo de plano, base/entregas/cobertura; `sdd-editorial-planejar`. |
| REQ-19 | Modelo de tasks, estados/evidências/reabertura; `sdd-editorial-tarefas`. |
| REQ-20 | Parecer e integração encaminham achados às tasks; skills distinguem revisão de documentos operacionais e narrativa. |

#### Passagens de contexto conferidas

Spec entrega versão, requisitos e parecer que o planejamento recebe. Plano entrega IDs, critérios e dependências que as tasks recebem. Preparação entrega ficha com fontes, voz e lacunas que a redação recebe. Redação identifica revisão e pendências; revisão recebe essa versão e devolve parecer com IDs e limites. Integração recebe pareceres e versão recuperável, registra destino dos achados e encaminha reconferências sobre a versão resultante. Esses campos e instruções estão definidos nos artefatos; ainda não foram exercitados como cadeia em uso.

Resultado: sem impeditivo documental remanescente no escopo conferido; T01-015 concluída. Revisão pela mesma IA participante da autoria, com acesso ao histórico. Guia ajustado e reconferido; modelos e skills não precisaram de mudança de conteúdo nesta rodada. A avaliação de comportamento permanece em T01-016, a reconciliação do acompanhamento em T01-017 e as escolhas editoriais necessárias ao piloto no documento 02.

### T01-016 — exercícios sintéticos de 2026-10-14

Entradas, critérios prévios, saídas, pareceres e versões preservados em [avaliações/T01-016](../../avaliacoes/T01-016/README.md). E01–E07 cobrem os oito casos previstos na seção 5.4 do plano, combinando seleção/limite de escopo com E01. A tabela de cobertura identifica cada skill v0.1, modo/perfil, resultado e limite. A cadeia E04–E07 preserva fonte, ressalva e lacuna; a integração manteve o rascunho após recusar cortes incompatíveis com o contrato.

Resultado: nenhum impeditivo observado nos percursos exercitados. Sete skills e nove perfis avaliados manualmente com contexto compartilhado e critérios conhecidos, sem independência ou comparação causal. Elaboração completa de spec, ficha completa, capítulo longo e refatoração substancial permanecem não exercitados. Antes de usá-los no piloto, complementar esta avaliação. T01-016 concluída neste recorte; T01-017 é a próxima tarefa. Piloto, apreciação autoral e decisões da spec 02 continuam pendentes.

### T01-017 — reconciliação do acompanhamento em 2026-10-14

**Base:** spec 0.5; plano 0.3; tasks 0.18 antes da revisão e 0.19 após correções; guia 0.2; modelo `modelos/tasks.md` e skill `skills/sdd-editorial-tarefas/SKILL.md`, ambos v0.1. Modos usados: conferir acompanhamento e acompanhar. Responsável: IA colaboradora, com histórico e acesso aos resultados anteriores; não é auditoria independente.

| Critério | Evidência examinada e resultado |
| --- | --- |
| Identificação, escopo e responsabilidades | Cabeçalho e seções 1 a 4 identificam base, caminhos, papéis, entregas e critérios. Acrescentada data de atualização; não foi necessário impor a organização visual do modelo. |
| IDs e dependências | 21 IDs únicos, mesmos IDs e ordem nas definições e acompanhamento. Dependências entre tasks apontam para IDs anteriores existentes, sem ciclos. Dependências externas do piloto explicitadas abaixo. |
| Evidência além da marcação | Registros individuais T01-001 a T01-014 identificam versão, aspectos conferidos e limites; artefatos citados existem com versões correspondentes. T01-015 registra correções e reconferência; T01-016 preserva entradas, saídas, pareceres e cobertura. As conferências estruturais históricas não foram reexecutadas nesta tarefa. |
| Separação entre níveis de conclusão | Construção documental, exercício sintético, piloto e apreciação autoral continuam distintos. T01-016 não comprova modalidades não exercitadas nem leitura humana. |
| Reabertura e preservação | Regras da seção 1 e registro T01-015 preservam evidência original e conferência localizada do guia v0.2. Não foi encontrada alteração de contrato que exigisse reabrir uma entrega nesta rodada. |
| Cobertura e situação atual | ENT-01 a ENT-06 cobertas por T01-001 a T01-017, com limites de T01-016. ENT-07 continua pendente, representada por T01-018 a T01-021. |

**Achados corrigidos:** cabeçalho ainda tratava os exercícios como futuros; linhas T01-001 a T01-007 conservavam próximos passos já realizados; T01-017 citava tasks 0.1 e dependências já atendidas; T01-015 indicava seção inadequada para o registro detalhado. Atualizados somente os campos de situação atual. O estado de T01-016 foi normalizado para “Concluída”, com a restrição de cobertura mantida nas colunas de evidência/pendência. A seção 6 passou a nomear também os registros documentais que já continha. O parecer inicial da decomposição foi explicitamente identificado como histórico.

**Resultado:** acompanhamento compatível com o modelo e a skill, após as correções; T01-017 concluída. Nenhum requisito, ID ou critério de conclusão foi reduzido. A conclusão de T01-016 vale para os percursos registrados; escolher modos adicionais no piloto aciona a complementação prevista, não aprovação automática.

### Destino vigente das pendências identificadas após T01-017

| ID | Tarefa afetada | Dependência e impacto | Quem resolve / momento | Situação |
| --- | --- | --- | --- | --- |
| PEN-01 | Origem T01-018 | Contexto editorial, história, fontes, voz e decisões de uso; análise ampliada na spec 02 v0.3. | Autor e IA na iniciativa 02, antes da execução de 03. | Transferida para spec 02; aberta no destino. |
| PEN-02 | Origem T01-016 / T01-018 / T01-019 | Analisar modos e perfis para o percurso pretendido; complementar avaliação se usar modos não exercitados. | IA na iniciativa 02; preservar T01-016 e registrar novas evidências separadamente. | Transferida para spec 02; condicional e aberta no destino. |
| PEN-03 | Origem T01-020 / T01-021 | Reconhecimento da voz, clareza, prazer de leitura e esforço exigem retorno real sobre o piloto. | Autor e IA na iniciativa 03, após produção/revisão. | Transferida para spec 03; não avaliada. |

**Próximo trabalho:** prosseguir na análise da [spec 02](../02-preparacao-editorial/02-resumo-editorial-onde-como-quando.md): acervo, história/contexto, referência de voz e adequação das skills. Receber decisões autorais depois de explicar as lacunas pertinentes. A iniciativa 01 está encerrada; o piloto e seu retorno autoral pertencem à iniciativa 03.

### Levantamento de PEN-01 — 2026-10-14

**Artefato:** spec 02, v0.1 → v0.2. **Base:** spec 01 v0.5, seção 15.8; plano 01 v0.3, seção 9; tasks v0.19; fontes locais indicadas no quadro da spec 02. Skills usadas: `sdd-editorial-especificar` v0.1, modo elaborar com conferência localizada; `sdd-editorial-tarefas` v0.1, modo acompanhar. Versões anteriores da spec 02 e destas tasks recuperáveis no commit `e931a1bbcd599c2337e576eb4bc6ad8a8f01c53d`, com presença no histórico e ausência de alterações locais verificadas antes da edição.

**Produção e critério conferido:** levantadas as propostas das fontes e organizadas sete decisões que cobrem o contexto mínimo de PEN-01. Leitura documental verificou origem, distinção entre proposta e decisão, preservação dos limites factuais e encaminhamento das lacunas. A sequência da spec 02 foi atualizada para refletir a implementação inicial já registrada. Links locais dos dois documentos alterados e integridade do diff conferidos após a edição.

**Resultado e limites:** levantamento concluído; PEN-01 continua aberta. Foram solicitadas escolhas sobre finalidade, leitor e voz, sem resposta registrada neste levantamento. As preferências não foram presumidas; ficha, redação, complementos de avaliação e apreciação autoral não foram executados. Conferência pela mesma IA autora das alterações, com acesso ao histórico, sem independência. T01-018 permanece pendente; requisitos da spec 01 e estratégia do plano 01 preservados.

### Protocolo dos exercícios de T01-016 — preservado para complementos

Após a separação de 2026-10-14, este protocolo permanece como referência. Novos complementos pertencem à preparação em 02 e não modificam a conclusão histórica de E01–E07; falha comprovada de uma skill exige correção e reconferência identificadas.

Ao executar T01-016, acrescentar uma linha por exercício com: identificação; skill e versão; modo/perfil; entrada ou localização do recorte; comportamento esperado; resultado observado; evidência; limitações; ajuste e reconferência, quando necessários.

Para permitir repetir a avaliação, preservar o pedido exato, os arquivos de entrada e saída ou seus caminhos/versionamentos recuperáveis, o modelo utilizado quando conhecido e quais instruções estavam disponíveis. Se essa informação não puder ser obtida, registrar como desconhecida. Definir o comportamento esperado antes de examinar a saída e não o alterar silenciosamente para acomodar um resultado ruim.

Incluir situações normais, lacunas relevantes e pedidos semelhantes que não devam acionar aquele procedimento. Reutilizar os casos do plano; não criar uma quantidade fixa de exercícios por skill sem necessidade. A seleção aqui é manual: acertar o procedimento em um exercício não comprova descoberta automática pelo ambiente.

Registrar cada dimensão como **atende**, **precisa de ajuste** ou **não avaliada**, com evidência: cumprimento da intenção, precisão e preservação das ressalvas, adequação da saída, tratamento de lacunas, voz/clareza quando pertinentes e esforço imposto pelo procedimento. Não converter prazer de leitura em uma nota automática.

Além dos exercícios individuais, acompanhar uma passagem curta de contexto entre preparação, redação, parecer e integração, usando material de avaliação. Conferir se fatos, ressalvas, versões e pendências sobrevivem à passagem. Essa verificação pertence a T01-016 e não antecipa o piloto da jornada.

Quando houver dúvida se uma instrução melhora o resultado ou apenas acrescenta burocracia, fazer uma comparação focal com a mesma entrada e condições semelhantes, sem a skill ou com a versão anterior. Registrar diferenças concretas e limitações; uma comparação isolada não comprova ganho geral. Esse recurso é diagnóstico, não uma bateria obrigatória de benchmarks.

**Situação inicial, anterior a 2026-10-14:** nenhum exercício executado. Situação atual: ver registro T01-016 e tabela de cobertura vinculada acima; modos não exercitados permanecem explicitamente não avaliados.

O registro de cobertura deve distinguir conferência documental de exercício realizado. Um mesmo recorte pode servir a perfis distintos, mas cada parecer identifica seu escopo. A ausência de pareceres anteriores só será declarada se efetivamente corresponder ao contexto utilizado.

## 7. Conferência desta decomposição

- ENT-01: T01-001.
- ENT-02: T01-002 a T01-004.
- ENT-03: T01-005 a T01-007.
- ENT-04: T01-008 a T01-010.
- ENT-05: T01-011 a T01-014.
- ENT-06: T01-015 a T01-017.
- ENT-07: T01-018 a T01-021.

As vinte exigências da spec têm tarefas relacionadas. Os sete pacotes de skills e os nove perfis previstos estão contemplados, sem exigir execução simultânea de agentes. A produção dos modelos e skills precede sua avaliação; a elaboração inicial destas tasks usa o contrato já definido na spec e no plano.

**Parecer inicial de decomposição, preservado como histórico da versão 0.1:** pronta para iniciar T01-001. Esta conferência é documental e foi feita com acesso ao histórico. Nenhuma tarefa de implementação está concluída pela criação deste documento. O texto 01 da jornada permanece reservado para o piloto posterior.

## 8. Orientações para criar e validar as skills

### Referência principal de autoria

O guia local [skill-creator do ambiente Codex](</C:/Users/Rahman/.codex/skills/.system/skill-creator/SKILL.md>) orienta escopo, descrição, estrutura de `SKILL.md`, carregamento progressivo de referências e validação. Foi consultado durante a preparação do plano. Seus princípios aplicáveis são:

- Escrever instruções que alterem decisões relevantes, evitando ensinar capacidades genéricas que o agente já possui.
- Definir descrições precisas, com fronteiras entre skills próximas.
- Dar liberdade a tarefas criativas e detalhar mais os pontos em que um desvio altera fatos, escopo ou rastreabilidade.
- Carregar referências somente quando necessárias e manter cada regra em uma fonte principal.
- Melhorar o procedimento a partir de falhas observadas, sem transformar cada caso isolado em regra universal.

O caminho identifica um recurso externo ao repositório e pode mudar em outro computador. Antes da implementação, localizar a versão disponível e registrar qual foi usada. Sua ausência não autoriza copiar instruções de outro ambiente sem avaliar compatibilidade.

### Validação estrutural

O [quick_validate.py local](</C:/Users/Rahman/.codex/skills/.system/skill-creator/scripts/quick_validate.py>) foi inspecionado: verifica a presença de `SKILL.md`, formato e propriedades permitidas do YAML, campos `name` e `description`, regras de nome/tamanho e certos marcadores TODO. Requer Python e o módulo `yaml`; confirmar disponibilidade ao executar, sem alegar que o comando foi rodado nesta revisão.

Na versão inspecionada, a conferência **não** verifica links, coerência das instruções, completude semântica, valor editorial nem correspondência do nome com a pasta. Alguns campos vazios também não são recusados. Portanto, T01-008 a T01-015 devem complementar o validador com leitura de nome/descrição não vazios, correspondência com a pasta, referências acessíveis e contratos completos. Resultado estrutural positivo não conclui T01-016.

### Referência complementar de avaliação

O outro [skill-creator disponível em `.agents`](</C:/Users/Rahman/.agents/skills/skill-creator/SKILL.md>) oferece ideias de pedidos realistas, comparação com uma versão de referência, avaliação qualitativa e iteração. Seu fluxo inclui ferramentas e execução voltadas a outro ambiente; usá-lo como fonte complementar, não como especificação obrigatória deste projeto.

Não adotar automaticamente suas rotinas de execução paralela, arquivos de benchmark, descrições expansivas ou campos adicionais de metadados. A compatibilidade segue o ambiente de destino e o escopo deste plano. Para escrita, a utilidade de comparação entre resultados e o retorno do autor importam mais que uma contagem de itens aprovados.

### Quatro evidências distintas

| Nível | Tarefa responsável | O que permite concluir |
| --- | --- | --- |
| Estrutura e contrato | T01-008 a T01-015. | Pacote legível, referências válidas e procedimento definido. |
| Decisões e passagem de contexto | T01-016. | Comportamentos observados nos exercícios e limites conhecidos. |
| Uso integrado na jornada | T01-018 e T01-019. | Aplicação real ao texto escolhido, com versões e pareceres. |
| Voz e experiência do autor | T01-020 e T01-021. | Apreciação humana registrada e ajustes decorrentes. |

## 9. Histórico de revisão das tasks

| Versão | Alteração | Resultado |
| --- | --- | --- |
| 0.1 | Decomposição em 21 tarefas com dependências e critérios. | Pronta para iniciar o guia. |
| 0.2 | Referências de autoria, limites reais do validador, registro reproduzível, cobertura de seleção e passagem de contexto. | Complementos nas tarefas existentes; nenhuma implementação ou avaliação executada. |
| 0.3 | Criação e conferência documental do guia v0.1. | T01-001 concluída; T01-002 e T01-005 com dependência atendida. |
| 0.4 | Criação e conferência documental do modelo de spec v0.1. | T01-002 concluída; T01-003 liberada na sequência principal. |
| 0.5 | Criação e conferência documental do modelo de plano v0.1. | T01-003 concluída; T01-004 liberada na sequência principal. |
| 0.6 | Criação e conferência documental do modelo de tasks v0.1. | T01-004 concluída; modelos de elaboração do método entregues; próxima T01-005. |
| 0.7 | Criação e conferência documental da ficha editorial v0.1, nas formas curta e completa. | T01-005 concluída; T01-006 liberada. |
| 0.8 | Criação e conferência documental do parecer editorial v0.1. | T01-006 concluída; próxima T01-007. |
| 0.9 | Criação e conferência documental do modelo de integração e avaliação v0.1. | T01-007 concluída; guia e seis modelos entregues; próxima T01-008. |
| 0.10 | Criação e validação estrutural/documental da skill de especificação v0.1. | T01-008 concluída no escopo de construção; próxima T01-009. |
| 0.11 | Criação e validação estrutural/documental da skill de planejamento v0.1. | T01-009 concluída no escopo de construção; próxima T01-010. |
| 0.12 | Registro da construção e validação estrutural/documental da skill de tarefas v0.1, concluído na retomada de 2026-10-14. | T01-010 concluída no escopo de construção; próxima T01-011. |
| 0.13 | Criação e validação estrutural/documental da skill de preparação editorial v0.1 em 2026-10-14. | T01-011 concluída no escopo de construção; próxima T01-012. |
| 0.14 | Criação e validação estrutural/documental da skill de redação v0.1 em 2026-10-14. | T01-012 concluída no escopo de construção; próxima T01-013. |
| 0.15 | Criação e validação estrutural/documental da skill de revisão e nove perfis v0.1 em 2026-10-14. | T01-013 concluída no escopo de construção; próxima T01-014. |
| 0.16 | Criação e validação estrutural/documental da skill de integração v0.1 em 2026-10-14. | T01-014 concluída; sete skills construídas; próxima T01-015. |
| 0.17 | Conferência integrada de 2026-10-14: links corrigidos, guia v0.2, passagens e cobertura documental examinadas. | T01-015 concluída; próxima T01-016. |
| 0.18 | Exercícios sintéticos E01–E07 em 2026-10-14, com entradas, saídas e limites preservados. | T01-016 concluída no recorte exercitado; próxima T01-017. |
| 0.19 | Reconciliação de 2026-10-14 com modelo e skill de tasks; situações atuais corrigidas e pendências do piloto explicitadas. | T01-017 concluída; próximo trabalho: definições da spec 02 para preparar T01-018. |
| 0.20 | Levantamento de PEN-01 e conferência localizada da spec 02 v0.2; propostas D02-01 a D02-07 e dependências registradas. | Aguardar escolhas autorais; T01-018 pendente, sem execução do piloto. |
| 0.21 | Separação expressamente solicitada pelo autor: método em 01, preparação/análise em 02, piloto em 03; conferência do fechamento e destinos. | 01 encerrada no novo escopo. T01-018 a T01-021 e PEN-01 a PEN-03 transferidas, sem conclusão fictícia. |
| 0.22 | Auditoria: corrigida falha em E03, reconciliados critérios antigos e arquivados os três documentos de 01. | T01-016/T01-017 reconferidas no aspecto afetado; iniciativa concluída nos limites registrados. |

## 10. Encerramento autorizado em 2026-10-14

**Base e versões:** spec 01 v0.6, plano 01 v0.4, tasks v0.21, spec 02 v0.3, spec 03 v0.1 e guia v0.3. A decisão do autor altera o escopo, preservando os vinte requisitos como contratos do método e critérios de aplicação futura.

**Evidência examinada:** registros T01-001 a T01-017, artefatos existentes, cobertura e saídas E01–E07. A conferência desta rodada tratou suficiência do fechamento, rastreabilidade das transferências e navegação; não repetiu os validadores estruturais ou os exercícios antigos. Não foi encontrado impeditivo de construção documental no recorte. As limitações observadas nas skills estão na análise da spec 02 e permanecem abertas para o uso pertinente.

**Preservação:** spec 01, plano, guia e AGENTS anteriores recuperáveis no commit `e931a1bbcd599c2337e576eb4bc6ad8a8f01c53d`. As alterações ainda não commitadas foram preservadas em `historico/2026-10-14-antes-da-separacao/01-tasks-v0.20.md` e `02-resumo-v0.2.md`, com hashes iguais aos arquivos de partida conferidos antes da edição. Essas cópias são históricas; links relativos internos conservam o contexto da localização original.

**Resultado:** ENT-01 a ENT-06 encerradas; ENT-07 e T01-018 a T01-021 recebidas na seção 2 da spec 03. PEN-01/PEN-02 recebidas em 02 e PEN-03 em 03. Nenhuma atividade transferida foi marcada como executada. Guia e AGENTS atualizados para retomar pela iniciativa pertinente; contratos das skills não alterados.

**Conferência final:** nove documentos vigentes alterados/criados examinados na navegação, com 115 referências locais e nenhum destino ausente; seis modelos e sete pacotes de skills encontrados. Tabela de acompanhamento mantém 21 IDs: 17 concluídos nos limites históricos e quatro transferidos sem execução. `git diff --check` sem erros. A referência antiga da base do livro foi corrigida para o arquivo existente em `capitulos estudos/`; nenhuma fonte ou texto da jornada foi reescrito. Guia v0.3 reconferido nas instruções de entrada, referência de base e encaminhamento do piloto; não houve mudança no contrato de redação/revisão.

**Limites:** revisão pela mesma IA com acesso ao histórico. Método construído e avaliado inicialmente não significa eficácia geral, voz reconhecida, aprendizagem ou prazer de leitura demonstrados. O piloto continua não iniciado.

**Próximo passo:** tratar os achados A02-01 a A02-07 da spec 02, começando pela história disponível e pelas referências de voz; depois fechar o contexto e os complementos de cobertura antes de planejar 03.

## 11. Auditoria e arquivamento — 2026-10-14

**Escopo e versões:** spec 01 0.6 → 0.7, plano 0.4 → 0.5, tasks 0.21 → 0.22; guia 0.4 com navegação atualizada. Conferidos requisitos, entregas, decisões antigas, checklist original, modelos, contratos das skills, nove perfis e entradas/saídas E01–E07. Os critérios e achados ARQ-01 a ARQ-05 estão na seção 20 da spec.

**Falha e reabertura localizada:** T01-016 foi reaberta para corrigir o estado de EX-T02 em E03; T01-017 foi reexaminada quanto à aceitação dessa evidência. A saída r1.1 agora usa pendente para a dependência futura, mantém produção distinta de conclusão e reabertura após mudança. Reconferência manual dirigida com os critérios já conhecidos; resultado atende após correção. As duas tarefas voltam a concluídas no recorte, sem apagar o julgamento inicial nem apresentar o exercício como independente. Nenhuma skill foi alterada.

**Demais correções:** checklist/decisões antigas com destino individual; tabela de histórico contínua; critério dos dois tipos de mudança explicitado na spec 03; links adequados ao arquivo. Nenhum dos itens do piloto foi concluído por essa revisão.

**Preservação:** versões imediatamente anteriores dos três documentos em `historico/2026-10-14-antes-do-arquivamento/`, relativas a `spec editorial/`; saída original E03 recuperável no commit `e931a1bbcd599c2337e576eb4bc6ad8a8f01c53d`. Cópias históricas mantêm seus caminhos relativos de origem e não são documentos ativos.

**Conferência estrutural atual:** sete chamadas de `validate_skill` do `quick_validate.py` local retornaram `True, Skill is valid!`, usando a dependência YAML isolada já disponível em `%TEMP%/sdd-editorial-validator-deps`. Sem instalação nova. Isso verifica estrutura, não qualidade editorial nem todos os modos de comportamento.

**Arquivamento:** somente spec, plano e tasks movidos para `spec editorial/concluida/01-sdd-editorial/`. Guia, modelos, skills e avaliações permanecem disponíveis nos caminhos de uso; fontes e textos da jornada preservados. IDs e evidências históricas mantidos.

**Conferência após a mudança:** 25 documentos ativos do conjunto examinados; 146 referências locais com destinos existentes e âncoras resolvidas. Vinte REQ na spec e no mapeamento do plano, sem requisito ausente; 21 IDs únicos no acompanhamento, sendo quatro transferidos e 17 concluídos. Seis modelos, sete skills e nove perfis presentes. `git diff --check` sem erros nos arquivos rastreados; os três arquivos movidos foram também conferidos em relação às cópias anteriores. Cópias em `historico/` foram preservadas e excluídas da conferência de navegação ativa, pois guardam o contexto de origem.

**Resultado:** concluída e arquivada após correções, sem impeditivo remanescente identificado no escopo documental e sintético conferido. Revisão pela mesma IA, com acesso ao histórico. Próximo trabalho em 02; piloto e apreciação autoral em 03.
