# Registro de conhecimento e fontes

[Acervo](README.md) · [Jornada](<Template jornada do heroi/README.md>) · [Estudos](<../capitulos estudos/README.md>) · [Governança AIOX](<../AGENTS.md>)

## Os Dois Fluxos de Registro no Ecossistema

O repositório separa estritamente a **construção de autoridade pessoal** (Jornada do Herói e Artigos) da **construção do conhecimento técnico** (Capítulos de Estudo do Livro):

### 1. Fluxo da Jornada do Herói (Registro de Autoridade)
- **Princípio:** A história está na mente do autor. Nenhuma IA tem autorização para inventar fatos, datas, dores ou desfechos.
- **Etapa 1 — Elicitação com o autor (`*interview` com `@curator`):** Perguntas investigativas de como, quando, onde e por quê sobre os marcos e tensões reais.
- **Etapa 2 — Enriquecimento do Template (`Template jornada do heroi/NN-texto-anexo.md`):** As respostas reais do autor são arquivadas no anexo daquela etapa, preenchendo as lacunas identificadas.
- **Etapa 3 — Montagem do Épico (`Template jornada do heroi/NN-*.md`):** O agente `editorial` estrutura a narrativa em prosa contínua em 1ª pessoa, usando a temática de Isekai/RPG como lente condutora da campanha.
- **Etapa 4 — Derivação das Publicações (`registro da autoridade/publicacoes/`):** Geração do artigo público oficial (`artigo.md`) e da chamada de rede (`chamada-linkedin.md`), acompanhados da `ficha.md`.
- **Etapa 5 — Quality Gate dos 4 Pilares:** Revisão de fatos, didática, voz e língua culta.

### 2. Fluxo dos Capítulos de Estudo (O Livro Técnico / Grimório)
- **Princípio:** O conhecimento técnico e científico deve ensinar de maneira autocontida, com autonomia didática, sem exigir que o leitor conheça a autobiografia do autor.
- **Etapa 1 — Pesquisa e Extração Primária (`@deep-research`):** Consulta a documentações fundamentais, RFCs, papers e arquitetura de sistemas agênticos.
- **Etapa 2 — Design Instrucional (`@education`):** Estruturação do currículo via *Understanding by Design* (Wiggins) e controle de carga cognitiva (Sweller).
- **Etapa 3 — Redação Técnica (`editorial`):** Redação do `documento-base.md` na pasta da unidade em `capitulos estudos/NN-.../`.
- **Etapa 4 — Registro de Autoestudo e Laboratório:** Seção dedicada onde o autor registra de forma empírica como estudou aquele assunto, como o colocou à prova na prática (ex: PDV D+, orquestração de harnesses) e quais limites foram encontrados.
- **Etapa 5 — Quality Gate Técnico e Pedagógico:** Verificação de código, diagramas e progressão conceitual.

---

## Onde registrar

| Conteúdo | Destino |
| --- | --- |
| Versões anteriores, diff e mudanças de arquivos | Histórico do Git; GitHub quando sincronizado pelo autor. |
| Intenção e decisões editoriais | Spec da iniciativa pertinente ou ficha técnica da peça. |
| Estratégia de execução e DAGs | Orquestração AIOX e histórias (`docs/stories/`). |
| Progresso, critério e evidência de conclusão | Acompanhamento da etapa e fichas de publicação. |
| Experiência pessoal e respostas da entrevista | `Template jornada do heroi/NN-texto-anexo.md` e página da etapa na jornada. |
| Conceito, fonte, exercício e resultado de estudo | `capitulos estudos/NN-.../documento-base.md`. |
| Relato de como estudou e aplicou no laboratório | Seção de autoestudo no capítulo técnico de estudos. |
| Artigo/post e suas decisões de revisão | Pasta da peça em `registro da autoridade/publicacoes/`. |
| Finalidade e limites de uma fonte de consulta | Seu mapa de entrada, como o mapa das ferramentas. |

Não criar sessões para narrar alterações de arquivos, cópias de segurança, snapshots, manifestos de hashes ou um segundo histórico do trabalho. Não recriar `sessoes/`, `episodios/` ou `etapas/` no acervo. Um pedido de continuar uma tarefa não pede um novo relatório de sessão.

## O que merece ficar no conteúdo

Registrar pergunta, fonte selecionada, explicação própria, observação ou relato confirmado, limite do que se pode concluir e dúvida seguinte quando isso acrescentar conhecimento. Escrever diretamente no estudo ou relato pertinente. Não repetir a lista de arquivos alterados, as mesmas decisões ou o mesmo resultado em vários documentos.

A história pessoal mantém primeira pessoa, humor e referências confirmadas. Não inventar cenas, emoções ou resultados. O estudo técnico deve permitir compreensão independente da autobiografia. Um artigo pode nascer diretamente das fontes suficientes, sem sessão ou episódio intermediário.

## Evidência proporcional

Distinguir relato do autor, interpretação, hipótese e resultado conferido. Vincular a afirmação à fonte; não copiar conversas inteiras nem dados privados. Retorno de leitor e reconhecimento da voz só são registrados quando recebidos. Mudança relevante de conclusão atualiza o documento responsável e, quando necessário, a tarefa afetada.

Sempre que precisar preservar texto de publicação, jornada ou capítulo de estudo antes de alterar, conferir se a versão está recuperável no Git. Se não estiver, solicitar o commit do autor e aguardar a alteração dependente, continuando partes independentes. Havendo dispensa explícita do autor para aquela versão em andamento, registrar o alcance e continuar sem commit, conforme a seção 5 de [AGENTS.md](<../AGENTS.md#5-limites-antes-de-agir>), sem presumir recuperação. A dispensa não se estende automaticamente a outras versões nem à exclusão de fontes. Não executar commit ou envio automaticamente nem fabricar preservação por cópia paralela. Etiqueta de revisão não garante recuperação do texto.
