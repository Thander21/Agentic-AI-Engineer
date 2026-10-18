# Mapa de estudos e capítulos

**Versão:** 0.3 — 18/10/2026. **Natureza:** mapa documental iniciado na iniciativa 04; preparação de CAP-01 aberta por pedido do autor.

[Índice de estudos](README.md) · [Base histórica das sete partes](ESTRUTURA_E_ESTUDO.md) · [Acervo de publicações](<../registro da autoridade/PUBLICACOES.md>) · [Método editorial](<../spec editorial/GUIA_DE_OPERACAO.md>)

## Como usar

Este é o local de referência para a ordem de estudo e a decomposição em capítulos. Os IDs CAP-01 a CAP-18 identificam unidades de trabalho, não capítulos já escritos. A sequência e as dependências abaixo são propostas operacionais derivadas dos assuntos do acervo, sujeitas a ajuste após diagnóstico; não foram confirmadas como currículo definitivo pelo autor nem validadas tecnicamente nesta entrega. As sete partes da fonte não equivalem a sete capítulos, e as quinze etapas narrativas não determinam o sumário.

Percorrer a ordem numérica como ponto de partida, conferindo os pré-requisitos indicados antes de cada unidade. Dependência significa compreensão necessária para a atividade proposta, não obrigação de concluir todo um livro. O primeiro passo é delimitar o caso e selecionar a fonte de CAP-01; estudos anteriores só contam como atendidos quando houver evidência identificada. Registrar antecipações ou retornos com motivo e manter IDs estáveis. Não há prazo semanal, calendário ou domínio técnico presumido.

A ordem final de ensino no livro permanece a definir a partir do público, dos casos e dos pré-requisitos demonstrados. Uma nota de estudo pode anteceder o capítulo; uma publicação derivada pode surgir antes de seu acabamento editorial.

## Fontes de origem e limites

As referências abaixo comprovam a origem documental dos assuntos, não sua validade técnica. Antes de estudar cada unidade, selecionar obra/documentação, edição ou versão e trechos específicos; conferir adequação e atualidade. Obras mencionadas na conversa continuam candidatas, sem nova recomendação bibliográfica nesta organização.

| Código | Origem local | Conteúdo a organizar |
| --- | --- | --- |
| S01 | [Parte I e F079](ESTRUTURA_E_ESTUDO.md), [F079 original](<../jornada do heroi/06-texto-anexo.md#fonte-f079>) | Runtime, stack/heap, memória/GC, processos/threads, I/O, descritores e portas. |
| S02 | [Parte II e F080](ESTRUTURA_E_ESTUDO.md), [F080 original](<../jornada do heroi/06-texto-anexo.md#fonte-f080>) | SQA, análise estática/SAST, métricas, contratos, efeitos colaterais, invariantes, asserções e profiling. |
| S03 | [Parte III e F081](ESTRUTURA_E_ESTUDO.md), [F081 original](<../jornada do heroi/06-texto-anexo.md#fonte-f081>) | Requisitos, atributos de qualidade, rastreabilidade, linguagem ubíqua, contextos e SDD de software. |
| S04 | [Parte IV e F082](ESTRUTURA_E_ESTUDO.md), [F082 original](<../jornada do heroi/06-texto-anexo.md#fonte-f082>) | Information hiding, coesão/acoplamento, SOLID, contratos, Conway e alternativas arquiteturais. |
| S05 | [Parte V e F083](ESTRUTURA_E_ESTUDO.md), [F083 original](<../jornada do heroi/06-texto-anexo.md#fonte-f083>) | Verificação/validação, pirâmide/troféu, BDD, propriedades, mutação e design por contrato. |
| S06 | [Parte VI e F084](ESTRUTURA_E_ESTUDO.md), [F084 original](<../jornada do heroi/06-texto-anexo.md#fonte-f084>) | Relacional, ACID, isolamento, travas, CAP/PACELC, Saga/2PC, idempotência, mensageria, APIs e offline-first. |
| S07 | [Parte VII e F084](ESTRUTURA_E_ESTUDO.md), [F077](<../jornada do heroi/07-texto-anexo.md#fonte-f077>) | Evolução, dívida, SemVer, migração, resiliência, observabilidade e criptografia aplicada. |
| S08 | [Temas transversais](ESTRUTURA_E_ESTUDO.md), [F031](<../jornada do heroi/09-texto-anexo.md#fonte-f031>), [F072](<../jornada do heroi/06-texto-anexo.md#fonte-f072>) | Contexto, orquestração, avaliações, governança, custos e ciclo estudo/aplicação/registro. |

## Sequência inicial

Em todas as linhas, o estado **Pendente** significa que esta iniciativa não executou nem avaliou a aprendizagem. Os resultados são critérios propostos para orientar o estudo; não são evidências já produzidas.

| Ordem / ID | Parte e capítulo de estudo | Objetivo | Pré-requisitos propostos | Fonte | Resultado esperado | Estado |
| --- | --- | --- | --- | --- | --- | --- |
| 01 / CAP-01 | I — Execução, runtime e memória | Explicar stack, heap e gerenciamento de memória no ambiente escolhido. | Delimitar ambiente e conhecimento de partida; nenhum CAP exigido. | S01 | Fluxo comentado de uma execução e limites da observação. | Preparação conferida — estudo ainda não iniciado |
| 02 / CAP-02 | I — Processos, threads e I/O | Relacionar execução, concorrência e recursos físicos. | CAP-01. | S01 | Caso de uso de recursos com latência, descritores ou comunicação observados. | Pendente |
| 03 / CAP-03 | II — Contratos e leitura diagnóstica | Localizar invariantes, efeitos colaterais e asserções. | CAP-01. | S02 | Leitura de uma entrega com afirmações ligadas a trechos e limites. | Pendente |
| 04 / CAP-04 | II — Qualidade, métricas e profiling | Interpretar sinais de SQA, análise estática/SAST, complexidade, acoplamento e Halstead sem confundi-los com prova geral. | CAP-02 e CAP-03. | S02 | Análise contextualizada de sinais estáticos e de execução. | Pendente |
| 05 / CAP-05 | III — Problema, requisitos e atributos de qualidade | Delimitar intenção, escopo e critérios de aceitação. | CAP-03; contexto do problema escolhido. | S03 | Especificação curta com cenários de qualidade e limites. | Pendente |
| 06 / CAP-06 | III — Linguagem e fronteiras de domínio | Relacionar linguagem ubíqua, bounded contexts e context mapping. | CAP-05. | S03 | Mapa de conceitos e fronteiras justificado pelo problema. | Pendente |
| 07 / CAP-07 | III — SDD e rastreabilidade no desenvolvimento | Ligar especificação, entrega e evidência sem prometer eliminar erros dos agentes. | CAP-05 e CAP-06. | S03/S08 | Uma cadeia de requisito até verificação, com lacunas identificadas. | Pendente |
| 08 / CAP-08 | IV — Modularidade e dependências | Examinar information hiding, coesão, acoplamento, SOLID e contratos. | CAP-03 e CAP-06. | S04 | Decisão de divisão com alternativas e consequências de mudança. | Pendente |
| 09 / CAP-09 | IV — Escolhas arquiteturais | Comparar camadas, hexagonal, Clean Architecture, monolito modular e serviços no contexto estudado, incluindo organização e Conway. | CAP-05 e CAP-08. | S04 | Diagrama e decisão arquitetural com restrições e custos. | Pendente |
| 10 / CAP-10 | V — Verificação, validação e aceitação | Relacionar intenção, BDD e estratégias de teste. | CAP-03 e CAP-05. | S05 | Cenários de aceitação com alcance e limites das verificações. | Pendente |
| 11 / CAP-11 | V — Propriedades, mutação e eficácia dos testes | Examinar se verificações detectam violações relevantes. | CAP-10. | S05 | Caso de falha detectada ou não detectada e explicação do limite. | Pendente |
| 12 / CAP-12 | VI — Dados, transações e isolamento | Relacionar modelo relacional, ACID, isolamento e travas. | CAP-02 e CAP-03. | S06 | Caso concorrente com invariante e evidência observada. | Pendente |
| 13 / CAP-13 | VI — Distribuição e consistência | Examinar falhas de comunicação, CAP/PACELC, Saga e 2PC. | CAP-09 e CAP-12. | S06 | Comparação de alternativas sob uma falha delimitada. | Pendente |
| 14 / CAP-14 | VI — Mensageria, APIs e sincronização | Examinar idempotência e offline-first em operações distribuídas. | CAP-10 e CAP-13. | S06 | Fluxo de sincronização com repetição/falha e limites documentados. | Pendente |
| 15 / CAP-15 | VII — Evolução e compatibilidade | Relacionar manutenção, dívida, Lehman, Strangler Fig, SemVer e Expand and Contract. | CAP-09 e CAP-10. | S07 | Plano de mudança com compatibilidade, custos e verificação. | Pendente |
| 16 / CAP-16 | VII — Resiliência e observabilidade | Examinar circuit breaker, bulkhead, retry/backoff/jitter e OpenTelemetry conforme o caso. | CAP-04 e CAP-14. | S07 | Diagnóstico de uma falha com evidências e alternativas de recuperação. | Pendente |
| 17 / CAP-17 | VII — Segurança aplicada e julgamento econômico | Relacionar criptografia, riscos e custo de manutenção às decisões do caso. | CAP-09 e CAP-14; base específica de segurança a selecionar. | S07/S08 | Análise de riscos e trade-offs com limites da fonte e da conclusão. | Pendente |
| 18 / CAP-18 | Transversal — Orquestração, contexto e governança de agentes | Consolidar direção, avaliação e registro das entregas de agentes. | CAP-07 e CAP-11 para consolidar; observações podem começar em qualquer ciclo. | S08 | Caso rastreável de orientação, entrega, avaliação e ajuste. | Pendente |

## Práticas que acompanham os capítulos

Leitura de código e diagnóstico atravessam as partes, com aprofundamento em CAP-03/04. Economia e julgamento aparecem nas alternativas de cada caso, com síntese em CAP-15/17. Orquestração é observada desde o primeiro uso de agentes; CAP-18 consolida essas observações e não obriga esperar o fim do percurso para praticá-la. O ciclo de pergunta, fonte, aplicação, registro e revisão acompanha todas as unidades. Os exemplos históricos exigem conferência antes de uso didático.

## Acompanhamento e vínculos

Ao iniciar uma unidade, acrescentar abaixo uma linha real com CAP, versão da nota/capítulo, fonte selecionada e trecho, sessão/episódio quando existir, evidência examinada, limitação e próxima ação. Estados de estudo: pendente, em estudo, evidência produzida/aguardando conferência e objetivo conferido no recorte. A maturidade editorial do capítulo é registrada separadamente conforme [Base do livro](BASE_DO_LIVRO.md). Concluir estudo não equivale a capítulo revisado ou texto publicado.

| Capítulo | Nota/capítulo e revisão | Fonte selecionada | Registro/evidência | Resultado e limite | Post/artigo derivado | Próxima ação |
| --- | --- | --- | --- | --- | --- | --- |

| CAP-01 | [FIC-CAP-01 r02](01-execucao-runtime-e-memoria/ficha-editorial.md); capítulo ainda não produzido | TEC01-01/02/04/05 para introdução; TEC01-03 reservada a aprofundamento; trechos e consulta na ficha | Autor escolheu Dart desktop e declarou leitura de chamadas/ifs/funções/waits, sem explicação dos conceitos-alvo. Fontes de chamadas/quadros complementadas; adequação didática conferida | Preparação concluída para rascunho conceitual com pendências delimitadas; sem experiência ou aprendizagem demonstrada | Nenhum | Próxima passagem: esboço introdutório, quando autorizada a produção. Antes de prática/detalhes da VM, identificar SDK, sistema e modo de execução e fixar fonte de implementação. |

Ao produzir um artigo/post, criar sua entrada no [índice central](<../registro da autoridade/PUBLICACOES.md>) e vincular o mesmo ID aqui. Episódio pessoal é opcional; uma síntese de fontes pode originar publicação. Não copiar uma experiência como se fossem acontecimentos diferentes.

## Pendências concretas

- CAP-01: Dart desktop e ponto de partida recebidos em 18/10/2026; preparação conceitual conferida. Versão do SDK, sistema operacional, modo de execução e fonte imutável da implementação são necessários antes de observação prática ou detalhamento da VM, sem impedir a futura redação introdutória delimitada.
- Antes de cada unidade: selecionar e conferir bibliografia específica; a listagem S01–S08 rastreia a conversa, não substitui fontes técnicas primárias.
- Durante o percurso: ajustar dependências conforme as dificuldades reais, registrando motivo e versão; definir caso e evidência antes de declarar aprendizagem.
- Antes de organizar a obra final: definir ordem didática, extensão e eventual divisão/união de capítulos, preservando a correspondência dos IDs.

**Conferência documental v0.1:** cobertura das sete partes e temas transversais confrontada com a estrutura existente; sequência proposta sem dependências futuras ou ciclos entre CAPs. Não houve estudo técnico, pesquisa externa, redação dos capítulos nem apreciação autoral da sequência. A iniciativa 04 registra a conferência integrada.
