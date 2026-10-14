# Orientações para IAs e IDEs

Este arquivo é o ponto de entrada para trabalhar neste repositório. Aplica-se à raiz e às subpastas. Se o ambiente não carregar `AGENTS.md` automaticamente, leia-o explicitamente antes de atuar. Não presuma instalação ou descoberta automática das skills locais.

## Natureza do projeto

O projeto documenta a formação por autoestudo de um profissional experiente em TI em engenharia com agentes, a jornada de aprendizado e a elaboração de um livro. O trabalho principal é editorial: estudo, registros, fontes, escrita criativa e revisão. Não introduza código, aplicação, infraestrutura ou baterias de testes de software para organizar a escrita.

Comunique-se em português. A narrativa usa referências de RPG medieval e isekai, com humor e tom profissional, conforme o contexto. Não imponha essa linguagem a documentos operacionais nem fabrique sofrimento, derrota ou superação para completar um arco narrativo.

## Como começar ou retomar uma sessão

1. Identifique o pedido atual e seu escopo. Um pedido de análise não autoriza executar todas as fases seguintes. Instruções explícitas do autor prevalecem sobre orientações locais, respeitadas as regras do ambiente.
2. Leia o [guia de operação](<spec editorial/GUIA_DE_OPERACAO.md>) e o estado atual nas [tasks da iniciativa 01](<spec editorial/01-tasks-sdd-editorial.md>), incluindo pendências e o último registro relevante. Um “continue” deve partir dessas evidências, não de suposições sobre sessões anteriores.
3. Consulte as seções pertinentes da [spec 01](<spec editorial/01-especificacao-sdd-editorial.md>) e do [plano 01](<spec editorial/01-plano-sdd-editorial.md>). Confirme versões, dependências e arquivos existentes antes de editar.
4. Leia o `SKILL.md` correspondente à fase na tabela abaixo. Consulte seus modelos e referências conforme a necessidade; não carregue todo o acervo indiscriminadamente.
5. Execute o trabalho autorizado que tenha contexto suficiente. Registre lacunas concretas e prossiga nas partes independentes. Não peça novamente decisões já fornecidas pelo autor.

As tasks são a fonte do progresso atual. Este arquivo não mantém uma segunda lista de tarefas concluídas. Registros antigos descrevem o estado na data em que foram escritos; não devem substituir o acompanhamento atual.

## Fontes de orientação e organização

| Documento ou pasta | Função |
| --- | --- |
| [Spec 01](<spec editorial/01-especificacao-sdd-editorial.md>) | Intenção, requisitos e regras do SDD editorial. |
| [Plano 01](<spec editorial/01-plano-sdd-editorial.md>) | Entregas, dependências, contratos das skills e critérios de avaliação. |
| [Tasks 01](<spec editorial/01-tasks-sdd-editorial.md>) | Execução, evidências, versões, pendências e reaberturas. |
| [Guia de operação](<spec editorial/GUIA_DE_OPERACAO.md>) | Aplicação do fluxo, papéis, percursos e encerramento. |
| [Spec 02 — onde, como e quando](<spec editorial/02-resumo-editorial-onde-como-quando.md>) | Definições editoriais de registros, formatos, público, voz, canais e rotina. É outra iniciativa; não é o plano da spec 01. |
| [Jornada do herói](<jornada do heroi/README.md>) | Quinze etapas da formação e da autoria, com fontes e anexos. |
| [Estrutura técnica e estudo](<capitulos estudos/README.md>) | Organização técnica do livro e dados de estudo. As etapas da jornada não equivalem automaticamente a capítulos. |
| [Registro da autoridade](<registro da autoridade/README.md>) | Documentação das experiências e seu aproveitamento editorial. |
| [Base do livro](BASE_DO_LIVRO.md) | Relação entre experiências, maturidade dos registros e capítulos. |

Se houver divergência entre documentos, identifique-a e confira as decisões mais recentes. Não transforme proposta histórica em escolha aceita, nem sobrescreva silenciosamente regras para resolver o conflito. Use os caminhos reais do workspace; não recrie pastas antigas a partir de referências desatualizadas.

## Fluxo SDD editorial

O fluxo usa três documentos de trabalho por iniciativa e os artefatos resultantes:

1. **Spec:** reúne análise inicial, especificação, decisões, lacunas e revisão de consistência no mesmo documento.
2. **Plano:** documento separado, elaborado com base na spec suficientemente definida; organiza entregas, dependências e critérios.
3. **Tasks:** documento separado, atualizado durante produção e conferência, com IDs estáveis e evidências.
4. **Artefatos:** textos ou documentos produzidos, revisados segundo sua finalidade e ligados às tarefas correspondentes.

Não crie um documento separado para cada análise ou revisão de spec. Reutilize os [modelos locais](<spec editorial/modelos>) de forma proporcional, sem reformatação gratuita de documentos existentes. Correções pequenas não exigem nova iniciativa ou toda a cadeia de revisão.

Mudança de intenção ou requisito retorna à spec; mudança de estratégia retorna ao plano; execução e evidências ficam nas tasks. Preserve IDs e histórico. Pareceres antigos não validam automaticamente versões novas.

## Skills por fase

Leia explicitamente a skill selecionada antes de usá-la. Os caminhos são relativos à raiz; as referências internas de cada skill são relativas à pasta dela.

| Trabalho solicitado | Skill local |
| --- | --- |
| Analisar, elaborar ou revisar a spec | [sdd-editorial-especificar](<spec editorial/skills/sdd-editorial-especificar/SKILL.md>) |
| Elaborar, ajustar ou conferir o plano | [sdd-editorial-planejar](<spec editorial/skills/sdd-editorial-planejar/SKILL.md>) |
| Decompor, acompanhar ou conferir tasks | [sdd-editorial-tarefas](<spec editorial/skills/sdd-editorial-tarefas/SKILL.md>) |
| Selecionar fontes e preparar ficha editorial | [editorial-preparar](<spec editorial/skills/editorial-preparar/SKILL.md>) |
| Elaborar esboço, rascunho ou reescrita delimitada | [editorial-redigir](<spec editorial/skills/editorial-redigir/SKILL.md>) |
| Emitir parecer especializado sobre versão identificada | [editorial-revisar](<spec editorial/skills/editorial-revisar/SKILL.md>) |
| Resolver pareceres, integrar e reconferir alterações | [editorial-integrar](<spec editorial/skills/editorial-integrar/SKILL.md>) |

Os [nove perfis de revisão](<spec editorial/skills/editorial-revisar/references/perfis.md>) cobrem estrutura, fatos/fontes, didática, continuidade, voz/tom, linha/fluidez, preparação linguística, leitura crítica e prova final. Selecione os pertinentes; não imponha nove pareceres a toda correção.

A cadeia pode ser executada sequencialmente pela mesma IA. Papéis distintos não comprovam independência nem autorizam delegação automática. Declare acesso ao histórico e a pareceres anteriores. Revisores emitem pareceres; o integrador aplica as decisões sobre o texto.

## Preservação, voz e evidência

- Preserve fontes, anexos de extração e versões necessárias à comparação. Antes de integrar alterações, confirme uma versão anterior recuperável. Não exclua fontes nem reorganize o acervo sem escopo autorizado.
- Transcrições e conversas de IA são registros históricos, não comprovação de fatos técnicos ou pessoais. Verifique fontes e sinalize o que não foi conferido.
- Não invente emoções, diálogos, acontecimentos, aprendizados ou resultados do autor. Diferencie relato confirmado, hipótese, metáfora e exemplo fictício.
- Use decisões editoriais e amostras reais para orientar a voz. Markdown selecionado do Obsidian é suficiente; não exige acesso ao cofre inteiro. Erros de notas rápidas não se tornam regras de estilo automaticamente.
- Preserve fatos, ressalvas e trechos que funcionam. Uma revisão pode concluir que não é necessário alterar o texto. Resolva conflitos por intenção, evidência e voz, não por maioria de pareceres.
- Diferencie conferência estrutural, exercício sintético, uso no piloto e apreciação humana. Não declare prazer de leitura, aprendizado ou reconhecimento da voz como comprovados pela IA.

## Conferência e entrega

Ao concluir uma tarefa, registre artefato e versão, critério examinado, evidência, resultado, limitações e pendências. Arquivo produzido sem conferência permanece produzido/aguardando conferência. Reabra o aspecto afetado quando uma mudança invalidar evidência anterior.

Verifique referências, coerência e alterações pertinentes à entrega. Não crie testes que apenas repitam o texto. Validação estrutural de uma skill não comprova comportamento editorial; consulte a cobertura registrada nas tasks e complemente os modos necessários antes de usá-los no piloto.

O piloto escolhido é [01 — Novo mundo, bagagem antiga](<jornada do heroi/01-novo-mundo-bagagem-antiga.md>). Antes de executá-lo, confira as dependências nas tasks e as definições necessárias da spec 02. Não transforme exemplos sintéticos de avaliação em vivências do autor nem antecipe o piloto durante a elaboração do método.

Retorno autoral ausente permanece pendente. Texto revisado não significa aprovado ou publicado. Publicação exige instrução explícita e registro da versão e do destino.

Ao encerrar a sessão, informe o que mudou, o que foi conferido, os limites e o próximo passo. Mantenha o acompanhamento suficiente para que outra IA retome sem depender da memória da conversa.
