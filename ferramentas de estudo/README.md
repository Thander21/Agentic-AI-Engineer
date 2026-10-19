# Ferramentas de estudo — projetos e fontes de contexto

**Base histórica:** relato autoral de 16/10/2026. O antigo registro SS-2026-10-16-001 é recuperável no Git, sem manter um diário de alterações paralelo.

Esta pasta reúne três projetos com funções distintas na formação e na história do autor. Seus documentos podem ajudar a preparar estudos, posts, artigos ou histórias, conforme o assunto. A leitura começa pelo projeto pertinente e pelos trechos necessários; a existência de documentação não comprova implementação, aprendizagem ou resultado.

<a id="decisoes-de-consulta"></a>

## Os três escopos

| Projeto | Contexto de origem — relato de 16/10/2026 | Como contribui para o conhecimento e a escrita |
| --- | --- | --- |
| [FlutterGuard-AI](FlutterGuard-AI/README.md) | Somente uma ideia a desenvolver para estudo. | Contexto da intenção, perguntas a investigar e propostas de arquitetura. Funcionalidades descritas são pretendidas; não apresentar como ferramenta pronta ou caso validado. |
| [SDD-TDDkit](https://github.com/Thander21/SDD-TDDkit) e sua base [SpecSimpleKit](https://github.com/Thander21/SpecSimpleKit) | Em desenvolvimento e uso, evoluindo com a experimentação e personalização em cada projeto. | Contexto de decisões sobre especificação, trabalho com agentes e adaptação de métodos. Conferir separadamente o que está na base, o que foi ajustado no projeto e o que voltou ao kit. |
| VagasAutomatizado — chamado de VagasAutomatizada no pedido | Projeto em uso na busca de vagas e fonte privada com mais informações pessoais/profissionais do autor. | Consulta local dirigida para compreender o contexto do autor. Aqui se documentam apenas existência, finalidade e limites; conteúdo e dados permanecem no ambiente privado. |

O contexto acima preserva o relato autoral datado, sem acompanhar o progresso dos projetos. Ao preparar um texto, consultar a fonte pertinente e conferir as evidências. Não usar descrições promocionais ou instruções de execução como prova de algo realizado.

## FlutterGuard-AI: ler como proposta

Começar pelo [README](FlutterGuard-AI/README.md) e selecionar apenas os documentos relacionados à pergunta de estudo. O README usa o presente ao descrever funcionalidades; nesta base editorial, o relato autoral de 16/10/2026 a caracteriza como: **ideia a desenvolver**. A formulação original foi preservada como proposta, sem convertê-la em entrega executada.

Um post pode apresentar a intenção de estudar ou desenvolver a ideia. Uma história pode usar os motivos e acontecimentos efetivamente relatados. Resultados, testes e aprendizados exigem registros posteriores que os sustentem.

## SDD-TDDkit e SpecSimpleKit: base, prática e evolução

O autor relata que começa cada projeto com o SpecSimpleKit para experimentar a base. Durante o uso, faz as modificações necessárias ao contexto e, a partir dessas experiências, evolui o SDD-TDDkit. Neste projeto editorial, a base também foi personalizada para apoiar o trabalho de escrita.

Essa relação é um relato de uso e adaptação; não comprova instalação de um motor de software neste repositório nem que toda mudança local já foi incorporada ao kit. O projeto possui repositório próprio ([Thander21/SDD-TDDkit](https://github.com/Thander21/SDD-TDDkit)) e fica excluído do controle de versão principal pelo [`.gitignore`](../.gitignore), servindo para consulta de contexto local e remota.

| Consulta | Ponto de entrada | Limite |
| --- | --- | --- |
| Compreender a oficina de desenvolvimento | Repositório [SDD-TDDkit no GitHub](https://github.com/Thander21/SDD-TDDkit) (local: [README](SDD-TDDkit/README.md) e [instruções locais](SDD-TDDkit/AGENTS.md)). | As regras de desenvolvimento pertencem ao kit; não substituem as regras editoriais da raiz. |
| Compreender a base inicial usada nos projetos | Repositório [SpecSimpleKit no GitHub](https://github.com/Thander21/SpecSimpleKit) (local: [README](SDD-TDDkit/SpecSimpleKit/README.md)). | Capacidades descritas e versão declarada precisam de conferência antes de afirmar funcionamento. |
| Examinar o modelo editorial agêntico | Governança em [AGENTS.md](../AGENTS.md) e agente [editorial](../.aiox-core/development/agents/editorial.md). | As decisões e evidências locais não demonstram, por si, adoção em outros projetos. |

Para contar uma mudança concreta, identificar a base usada, a necessidade do projeto, a adaptação feita e a evidência disponível. Não inventar uma cronologia de versões, atribuir ganhos sem comparação ou declarar retorno ao kit sem conferir o registro correspondente.

## VagasAutomatizado: fonte privada de consulta

O caminho local é `ferramentas de estudo/VagasAutomatizado/`. A grafia real foi mantida; não foi criada outra pasta com a variante VagasAutomatizada. A pasta fica excluída do Git principal pelo [`.gitignore`](../.gitignore), inclusive seu conteúdo e eventual repositório interno.

A consulta local está autorizada pelo autor quando o assunto exigir contexto pessoal/profissional ou da busca de vagas. Começar pelas instruções locais e selecionar a documentação necessária, sem executar automações ou enviar candidaturas por consequência da leitura. Não copiar arquivos, currículos, contatos, candidaturas, dados, capturas ou resumos privados para este acervo, seus históricos ou fichas. Um uso público exige seleção e autorização específica do recorte pelo autor; a versão resultante deverá ser conferida antes da publicação.

O versionamento deve permanecer separado e privado. A existência e a visibilidade de um repositório remoto exigem verificação própria; a consulta local não autoriza criar, alterar ou sincronizar repositórios.

## Passagem para estudos, posts e histórias

1. Definir a finalidade do texto e consultar somente o escopo pertinente, além dos relatos e notas já selecionados.
2. Distinguir relato autoral, proposta, observação e resultado conferido. Para fontes publicáveis, registrar caminho, data/versão, afirmação sustentada e limites. Detalhes de fontes privadas continuam no ambiente privado.
3. Aplicar o agente [editorial](../.aiox-core/development/agents/editorial.md) com seu comando `*brief`, preservando lacunas reais.
4. Guardar posts e artigos no [acervo de publicações](<../registro da autoridade/PUBLICACOES.md>), com origem `jornada`, `estudo` ou `ambas`. Capítulos e evidências de estudo ficam em [capítulos e estudos](<../capitulos estudos/README.md>); a [jornada](<../registro da autoridade/Template jornada do heroi/README.md>) fornece contexto narrativo.

Os três projetos são fontes possíveis, não uma nova ordem de estudo nem uma fila automática de publicações. A seleção de uma fonte não inicia desenvolvimento, estudo técnico ou piloto.

## Obsidian e continuidade

Notas Markdown selecionadas no Obsidian podem complementar as consultas. Os links deste mapa oferecem a navegação inicial entre as áreas públicas; o caminho privado foi registrado como texto e sua ausência em uma cópia pública é esperada.

Os vínculos entre projetos, dados e notas no Obsidian dependem da seleção autoral do material, preservando a separação entre consulta local e conteúdo publicável. As configurações de `.obsidian/` servem à navegação e apresentação, sem importar dados privados.
