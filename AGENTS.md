# Orientações para agentes

Aplica-se à raiz e às subpastas deste repositório. Leia este arquivo antes de atuar; não presuma carregamento automático das instruções ou das skills locais.

## 1. Escopo e autoridade

- Trabalhe em português. O ecossistema é orquestrado pelo **AIOX**, gerenciando tanto engenharia quanto a produção editorial de estudos, livros, capítulos e publicações de autoridade.
- A produção e revisão de conteúdo editorial é executada pelo agente **`editorial` (Scribe)** do AIOX, garantindo profundidade técnica, voz autoral e zero alucinações factuais sem a sobrecarga de burocracias ou pipelines fragmentados.
- O pedido do autor delimita a ação. Analisar não autoriza editar ou produzir as fases seguintes. “Continue” retoma a entrega autorizada até sua conclusão ou dependência real, sem pedir confirmação a cada parágrafo.
- Use o pedido explícito e as histórias (stories) gerenciadas pelo AIOX. Não crie especificações ou burocracias paralelas de controle.

## 2. Entrada e seleção de leitura

1. Identifique a entrega, a ação permitida e os arquivos afetados no acervo (`capitulos estudos/`, `registro da autoridade/` ou `docs/stories/`).
2. Se a tarefa for editorial, ative o agente `editorial` e utilize seus comandos nativos (`*brief`, `*write`, `*review`, `*refine`, `*proof`).
3. Consulte somente a peça/capítulo e as fontes selecionadas; não carregue pastas inteiras ou anexos desnecessários.
4. Antes de redigir ou alterar, garanta ter: objetivo, leitor-alvo, fontes de referência e decisões aplicáveis. Não preencha lacunas essenciais por suposição.

## 3. Onde ler e quando

Os READMEs das áreas explicam seus documentos de apoio. Use-os para escolher a fonte quando ela ainda não estiver identificada; não carregue pastas inteiras.

<a id="consulta-do-registro-da-autoridade"></a>
<a id="consulta-da-jornada-do-herói"></a>
<a id="consulta-dos-capítulos-e-estudos"></a>
<a id="consulta-das-ferramentas-de-estudo"></a>

| Necessidade | Entrada e aprofundamento |
| --- | --- |
| Entender a proposta geral do projeto | [README principal](README.md). Dispensável para uma tarefa delimitada cujo contexto já esteja disponível. |
| Orquestração e fluxo de trabalho | AIOX via `aiox-master`, `po` (histórias e critérios de aceite) e `editorial` (execução do texto). |
| Preparar, redigir ou revisar post/artigo | [Índice de publicações](<registro da autoridade/PUBLICACOES.md>) para localizar a peça; depois acione o agente `editorial`. Para outros documentos do acervo, [mapa de uso](<registro da autoridade/README.md#mapa-de-uso-dos-documentos>). |
| Registrar uma experiência ou conhecimento | [Método de registro](<registro da autoridade/METODO_DE_REGISTRO.md>); selecione o destino. Relato na jornada, conhecimento no estudo, post/artigo no acervo. |
| Trabalhar voz ou história pessoal | [Universo narrativo](<registro da autoridade/Template jornada do heroi/UNIVERSO_NARRATIVO.md>), [Amostras de voz](<registro da autoridade/Template jornada do heroi/AMOSTRAS_DE_VOZ.md>) e relatos pertinentes. |
| Rastrear uma afirmação ou referência histórica | [Mapa de origem](<registro da autoridade/Template jornada do heroi/MAPA_ORIGEM.md>) para localizar o trecho dos anexos; [referências](<registro da autoridade/Template jornada do heroi/REFERENCIAS.md>) para menções. |
| Localizar ou acompanhar estudo/capítulo | [README de estudos](<capitulos estudos/README.md>) para visão geral das 7 partes; [Mapa de estudos](<capitulos estudos/MAPA_DE_ESTUDOS.md>) para sequência; pasta da unidade (`capitulos estudos/NN-.../`) para `documento-base.md`. |
| Consultar ferramentas como fontes | [Mapa das ferramentas](<ferramentas de estudo/README.md>); apenas como fonte técnica. A leitura não autoriza desenvolvimento ou candidaturas sem pedido expresso. |

## 4. Agente Editorial e Coordenação AIOX

A produção textual é centralizada no agente **`editorial`** (`.aiox-core/development/agents/editorial.md` / `.agents/skills/editorial/SKILL.md`):

| Comando Editorial | Função |
| --- | --- |
| `*brief` | Define enquadramento: leitor, questão central, fontes e delimitação de lacunas. |
| `*write` | Redige o esboço estruturado ou versão completa, com tom autêntico e didática progressiva. |
| `*review` | Executa o Quality Gate dos 4 Pilares: 1) Fatos e Fontes, 2) Estrutura e Didática, 3) Voz e Fluidez, 4) Norma e Prova Final. |
| `*refine` | Aplica correções e integra melhorias preservando o que funciona. |
| `*proof` | Prova final técnica (gramática, links, markdown, resíduos). |

- **Orquestração AIOX:** O PO (`po`) especifica a Story com Critérios de Aceite (ACs); o agente `editorial` redige e revisa; a aprovação de voz e publicação pertence soberanamente ao autor humano.
- Não crie pareceres burocráticos ou comitês artificiais de IAs. Use o ciclo direto de valor: briefing → redação → revisão dos 4 pilares → refinamento → leitura autoral.

## 5. Limites antes de agir

- **Preservação:** antes de alterar texto de publicação, jornada ou capítulo que precise ser preservado, confira se a versão está recuperável no Git. Se faltar, solicite commit do autor e aguarde a edição dependente, continuando partes independentes. Se o autor dispensar explicitamente a preservação daquela versão em andamento, registre o alcance e prossiga conforme o guia, sem presumir recuperação. Não faça commit/push automático, backups, snapshots ou pastas de histórico para simular versionamento. Não exclua fontes nem reorganize o acervo sem escopo autorizado.
- **Fatos e voz:** não invente vivências, emoções, falas, aprendizados ou resultados. Diferencie relato, hipótese, metáfora e exemplo fictício. Use decisões e amostras reais; erros de notas rápidas não definem estilo. Preserve fatos, ressalvas e trechos que funcionam; revisão pode recomendar manter o texto. Capítulos devem ensinar independentemente da história pessoal.
- **Fontes:** transcrição e conversa de IA são registros históricos, não comprovação. Registre fonte publicável, data/versão e limite no acompanhamento pertinente; sinalize o que não foi conferido. Documentação de ferramenta não comprova implementação ou resultado, nem importa suas regras para este editorial.
- **Privacidade:** `ferramentas de estudo/VagasAutomatizado/` admite consulta local dirigida, inclusive de arquivos ignorados. Não copie conteúdo, dados pessoais, currículos, contatos, candidaturas, anexos, capturas ou resumos privados para arquivos versionáveis. Recorte público exige autorização específica e conferência. Mantenha exclusão pelo `.gitignore` e versionamento privado separado; não force adição, crie submódulo ou copie a pasta para contornar a separação. Confira arquivos rastreados antes de afirmar proteção; não presuma existência ou visibilidade de remoto.
- **Localização:** mantenha uma única versão de trabalho por peça. Posts/artigos em `registro da autoridade/publicacoes/`; relatos na jornada; capítulos de estudos em `capitulos estudos/` (em pastas dedicadas por unidade `NN-.../` com seu `documento-base.md`). Preserve IDs e atualize vínculos em movimentações autorizadas. Não recrie camadas paralelas de episódios, fichas de etapas ou sessões administrativas; histórico de arquivos pertence ao Git.
- **Aprovação e envio:** retorno autoral ausente permanece pendente. Texto revisado não significa aprovado ou publicado. Publicação exige instrução explícita e identificação da versão e destino.

## 6. Conferência e entrega

Confira conteúdo, referências e coerência pertinentes à mudança. Antes do uso de um modo de skill no piloto, consulte sua cobertura no acompanhamento e complemente o necessário. Validação estrutural, exercício sintético, uso real e apreciação humana são evidências distintas; não declare voz reconhecida, prazer de leitura ou aprendizado comprovados pela IA.

Registre uma vez no acompanhamento pertinente: artefato/versão, critério, evidência, resultado, limites e pendência/próxima ação. Sem tasks e em trabalho pequeno, use registro proporcional na peça/ficha quando necessário, sem criar relatório ou diário de sessão. Documento produzido sem conferência não está concluído; alteração que invalide evidência reabre o aspecto afetado.

Ao entregar, informe o que mudou, o que foi conferido, os limites e o próximo passo. Deixe o acompanhamento suficiente para retomada sem depender da memória da conversa. Não mantenha listas de progresso neste arquivo ou nos READMEs.
