# Estrutura do livro e dados de estudo

[Índice do livro](README.md) · [Texto literal da última revisão](EXTRACAO_ULTIMA_REVISAO.md) · [Base editorial](BASE_DO_LIVRO.md)

**Uso atual:** esta consolidação preserva a origem das sete partes. A sequência e a decomposição inicial em capítulos estão no [mapa de estudos](MAPA_DE_ESTUDOS.md); as lacunas abaixo permanecem como pontos a conferir por unidade.

## Qual versão está sendo consolidada

A base é o último ajuste de conversa original: o pedido para enriquecer as sete fases com matéria de Engenharia de Software e a resposta que acrescenta requisitos, modularidade, qualidade, evolução e configuração. Sua visão geral está preservada em [F078](<../jornada do heroi/06-texto-anexo.md#fonte-f078>).

As sete fases são apresentadas aqui como **partes técnicas provisórias do livro**. A ordem da última proposta foi preservada. O conteúdo e as referências foram reunidos a partir da conversa; os produtos de estudo e de escrita abaixo são sugestões de organização para o próximo detalhamento.

## Visão geral das sete partes

| Parte | Foco da última revisão | Base de estudo e produção |
| --- | --- | --- |
| I | Computação e runtime | Compreender execução, recursos e limites físicos. |
| II | Qualidade, métricas e auditoria | Examinar entregas e interpretar sinais de qualidade. |
| III | Requisitos, atributos de qualidade e SDD | Transformar necessidades em especificações e critérios verificáveis. |
| IV | Modularidade e arquitetura | Justificar fronteiras, dependências e escolhas de design. |
| V | Verificação, validação e testes | Avaliar comportamento, contratos e eficácia das verificações. |
| VI | Dados, concorrência e distribuição | Projetar operações consistentes sob concorrência e falhas. |
| VII | Evolução, manutenção e produção | Sustentar o sistema ao longo de mudanças e incidentes. |

## Parte I — Fundamentos de Computação e Runtime

**Objetivo de estudo:** relacionar a experiência em infraestrutura ao funcionamento do software e ao uso de recursos.

**Conteúdo da última revisão:** runtime, stack e heap, gerenciamento de memória, garbage collection, latência de I/O, processos, threads, concorrência preemptiva, descritores de arquivo e portas TCP/UDP.

**Aplicação com IA proposta na conversa:** examinar se a implementação respeita os limites de memória e concorrência do ambiente.

**Dados de estudo disponíveis:** o modelo físico e as lacunas de execução aparecem também em [F035](<../jornada do heroi/07-texto-anexo.md#fonte-f035>) e na primeira sequência em [F067](<../jornada do heroi/07-texto-anexo.md#fonte-f067>). A conversa não escolheu uma obra específica para toda esta parte; essa seleção permanece aberta.

**Material a produzir ao estudar:** um caso de execução com o fluxo observado, recursos utilizados, hipótese examinada e explicação do resultado. Esse caso poderá sustentar capítulos sobre modelo físico, runtime e diagnóstico.

**Fonte da última revisão:** [F079](<../jornada do heroi/06-texto-anexo.md#fonte-f079>).

## Parte II — Garantia da Qualidade, Métricas e Auditoria

**Objetivo de estudo:** desenvolver critérios para examinar código, testes e execução e compreender o alcance de cada sinal.

**Conteúdo da última revisão:** SQA, análise estática, SAST, complexidade ciclomática, acoplamento aferente e eferente, métricas de Halstead, contratos, efeitos colaterais, invariantes, asserções e profiling.

**Aplicação com IA proposta na conversa:** configurar verificações de qualidade para avaliar as entregas. Limites numéricos e critérios de rejeição ainda precisam de definição contextualizada.

**Dados de estudo disponíveis:** autores e conceitos de métricas estão em [F076](<../jornada do heroi/10-texto-anexo.md#fonte-f076>). A aplicação prática da leitura e dos cinco filtros está reunida no [anexo 10](<../jornada do heroi/10-texto-anexo.md>). O SWEBOK é citado como referência geral em [F075](<../jornada do heroi/07-texto-anexo.md#fonte-f075>); fontes primárias específicas das métricas ainda devem ser selecionadas.

**Material a produzir ao estudar:** uma análise de entrega com sinais encontrados, explicação do que significam, verificações realizadas e limites da conclusão. Poderá alimentar capítulos de leitura diagnóstica e auditoria.

**Fonte da última revisão:** [F080](<../jornada do heroi/06-texto-anexo.md#fonte-f080>).

## Parte III — Requisitos, Atributos de Qualidade e SDD

**Objetivo de estudo:** formular o problema, os limites e os comportamentos esperados com precisão suficiente para orientar e avaliar o desenvolvimento.

**Conteúdo da última revisão:** elicitação e especificação de requisitos, requisitos não funcionais, cenários de atributos de qualidade, matrizes de rastreabilidade, linguagem ubíqua, bounded contexts, context mapping e limites de escopo.

**Aplicação com IA proposta na conversa:** usar especificações com restrições e critérios explícitos para conduzir os agentes. A alegação de eliminar alucinações permanece como afirmação da fonte a avaliar.

**Dados de estudo disponíveis:** SWEBOK e rastreabilidade são citados em [F075](<../jornada do heroi/07-texto-anexo.md#fonte-f075>). *Domain-Driven Design Distilled*, de Vaughn Vernon, e artigos de Martin Fowler aparecem em [F007](<../jornada do heroi/05-texto-anexo.md#fonte-f007>). *Domain-Driven Design*, de Eric Evans, também foi mencionado em [F004](<../jornada do heroi/06-texto-anexo.md#fonte-f004>).

**Material a produzir ao estudar:** uma especificação ligada ao problema real, com atributos de qualidade, critérios de aceitação, decisões e evidências posteriores. Poderá gerar capítulos de requisitos, modelagem e engenharia de especificação.

**Fonte da última revisão:** [F081](<../jornada do heroi/06-texto-anexo.md#fonte-f081>).

## Parte IV — Modularidade e Arquitetura de Software

**Objetivo de estudo:** justificar como o sistema será dividido e quais dependências serão admitidas diante das mudanças esperadas.

**Conteúdo da última revisão:** information hiding, coesão, acoplamento, SOLID, contratos, Lei de Conway, arquitetura em camadas, hexagonal, Clean Architecture, monolito modular e serviços distribuídos.

**Aplicação com IA proposta na conversa:** conduzir a implementação de fronteiras e adaptadores que permitam modificar detalhes externos sem espalhar mudanças pelo domínio.

**Dados de estudo disponíveis:** *Clean Architecture*, de Robert C. Martin, e artigos de Fowler são citados em [F007](<../jornada do heroi/05-texto-anexo.md#fonte-f007>). Parnas, Stevens e os fundamentos de modularidade aparecem em [F075](<../jornada do heroi/07-texto-anexo.md#fonte-f075>). A conversa não identifica as obras primárias completas de todos esses autores.

**Material a produzir ao estudar:** uma decisão arquitetural com restrições, alternativas, escolha e consequências, acompanhada de um diagrama e de um caso de mudança. Poderá sustentar capítulos de modularidade, arquitetura e trade-offs.

**Fonte da última revisão:** [F082](<../jornada do heroi/06-texto-anexo.md#fonte-f082>).

## Parte V — Verificação, Validação e Testes

**Objetivo de estudo:** relacionar as verificações à intenção do negócio e compreender que evidência cada teste fornece.

**Conteúdo da última revisão:** distinção entre verificação e validação, pirâmide e troféu de testes, BDD, testes baseados em propriedades, invariantes, testes de mutação e design por contrato.

**Aplicação com IA proposta na conversa:** orientar testes comportamentais e examinar se a suíte detecta violações relevantes, inclusive nos testes gerados pelo agente.

**Dados de estudo disponíveis:** *Unit Testing Principles, Practices, and Patterns*, de Vladimir Khorikov, e *Growing Object-Oriented Software, Guided by Tests*, de Steve Freeman e Nat Pryce, foram indicados em [F009](<../jornada do heroi/05-texto-anexo.md#fonte-f009>). O exemplo de fatura e seus testes está preservado no [anexo 10](<../jornada do heroi/10-texto-anexo.md>), ainda como material didático a examinar.

**Material a produzir ao estudar:** cenários de aceitação, testes e uma demonstração do que detectam e deixam em aberto. Poderá alimentar capítulos sobre contratos, testes e avaliação das entregas.

**Fonte da última revisão:** [F083](<../jornada do heroi/06-texto-anexo.md#fonte-f083>).

## Parte VI — Dados, Concorrência e Distribuição

**Objetivo de estudo:** compreender conflitos, integridade e consistência em operações concorrentes e sistemas sujeitos a falhas de rede.

**Conteúdo da última revisão:** modelo relacional, ACID, anomalias de isolamento, travas otimistas e pessimistas, CAP, PACELC, Saga, 2PC, idempotência, mensageria, APIs e offline-first.

**Aplicação com IA proposta na conversa:** orientar sincronização e processamento concorrente e investigar race conditions e deadlocks.

**Dados de estudo disponíveis:** *Designing Data-Intensive Applications*, de Martin Kleppmann, e a referência localfirstweb.dev foram mencionados em [F011](<../jornada do heroi/05-texto-anexo.md#fonte-f011>). A primeira abordagem de dados está em [F010](<../jornada do heroi/07-texto-anexo.md#fonte-f010>).

**Material a produzir ao estudar:** um experimento com operações concorrentes ou falha de comunicação, invariantes esperadas e evidências da estratégia escolhida. Poderá sustentar capítulos de transações, sincronização e consistência.

**Fonte da última revisão:** primeira seção de [F084](<../jornada do heroi/06-texto-anexo.md#fonte-f084>).

## Parte VII — Evolução, Manutenção e Resiliência em Produção

**Objetivo de estudo:** planejar a continuidade do sistema diante de falhas, mudanças de requisitos e evolução das dependências.

**Conteúdo da última revisão:** leis de Lehman, dívida técnica, Strangler Fig, SemVer, Expand and Contract, circuit breaker, bulkhead, retry, backoff, jitter, observabilidade, OpenTelemetry e criptografia aplicada.

**Aplicação com IA proposta na conversa:** conduzir mudanças de módulos legados e usar evidências de produção para avaliar comportamento e corrigir falhas.

**Dados de estudo disponíveis:** *Release It!*, de Michael T. Nygard, Azure Architecture Center, AWS Well-Architected e conceitos do OpenTelemetry aparecem em [F013](<../jornada do heroi/05-texto-anexo.md#fonte-f013>). Lehman, Cunningham, Fowler e Beck são citados em [F077](<../jornada do heroi/07-texto-anexo.md#fonte-f077>); suas fontes específicas para cada seção ainda precisam de seleção.

**Material a produzir ao estudar:** um caso de manutenção ou falha com diagnóstico, escolha de evolução, critérios de compatibilidade e evidências. Poderá alimentar capítulos sobre operação, segurança, evolução e custo de manutenção.

**Fonte da última revisão:** segunda seção de [F084](<../jornada do heroi/06-texto-anexo.md#fonte-f084>).

## Temas que atravessam as sete partes

**Leitura e diagnóstico de código:** praticados em todas as partes, com especial atenção ao runtime e à avaliação das entregas.

**Orquestração de agentes:** a última lista mantém aplicações com IA em cada fase, mas reduz o destaque do módulo específico de contexto, avaliações e governança apresentado antes. Preservar esse material de [F031](<../jornada do heroi/09-texto-anexo.md#fonte-f031>); o mapa inicial prevê CAP-18 como consolidação e prática transversal desde os primeiros ciclos, sujeito a revisão.

**Economia e julgamento de engenharia:** a última revisão menciona economia do software, custos de manutenção, dívida técnica e escolhas sob restrições. Organizar essas relações nas decisões e nos casos; a bibliografia específica ainda não foi definida.

**Estudo, projeto e registro:** aproveitar o ciclo de problema, leitura, aplicação e documentação de [F072](<../jornada do heroi/06-texto-anexo.md#fonte-f072>). Os prazos de uma semana sugeridos na fonte ainda não representam um cronograma adotado.

## Ligação com a jornada e com os registros

| Frente do livro | Etapas da jornada que a alimentam |
| --- | --- |
| Perfil, tese e leitor | 01, 02, 03 e 04. |
| Fontes e sequência de estudo | 05 e 06. |
| Sete partes técnicas e aplicação | 07, 08, 09, 10 e 11. |
| Casos documentados | 12, com registro desde o começo. |
| Textos públicos e retorno dos leitores | 13. |
| Estrutura e elaboração do livro | 14 e 15. |

Consultar o [registro contínuo](<../registro da autoridade/README.md>) para sessões, episódios e fichas das etapas. Vincular cada capítulo aos registros que sustentam suas explicações, usando a [base editorial](BASE_DO_LIVRO.md).

## Dados ainda necessários para o próximo detalhamento

- Conferir os pré-requisitos propostos no mapa e delimitar profundidade por unidade.
- Obras, edições e trechos específicos para os assuntos ainda sem fonte selecionada.
- Um caso ou experimento delimitado por objetivo de aprendizagem.
- Critérios para demonstrar entendimento e autonomia, além do resultado do produto.
- Rever a decomposição inicial CAP-01 a CAP-18 e definir a ordem final de ensino; o mapa não fixa o sumário definitivo.

As referências acima foram recuperadas da conversa. Sua atualidade e adequação ainda precisarão de conferência ao selecionar as leituras; esta consolidação não acrescenta uma bibliografia externa nova.
