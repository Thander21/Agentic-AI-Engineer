# 03. Texto anexo — A classe: engenheiro agêntico

[Etapa da jornada](03-a-classe-engenheiro-agentico.md) · [Índice](README.md) · [Mapa de origem](MAPA_ORIGEM.md)

Este anexo reúne 6 trechos: 2 principais e 4 cópias relacionadas. A organização abaixo identifica o que a conversa já oferece e o que ainda precisa ser aprofundado.

As sínteses são uma leitura editorial do material. Os blocos identificados como fonte preservam literalmente perguntas, respostas, exemplos e versões anteriores; sugestões da outra IA não passam a ser decisões aprovadas ou resultados comprovados por estarem neste anexo.

## Mapa de aprofundamento

| Assunto | O que já temos | O que aprofundar |
| --- | --- | --- |
| [Orquestrar, direcionar e tomar decisões](#assunto-01) | Você pede uma formação orientada à decisão e à condução dos agentes. A IA propõe um comparativo de competências. | Converter a descrição do papel em atividades observáveis, sem assumir como correto todo o contraste com a formação tradicional. |
| [Contexto, avaliações e governança de agentes](#assunto-02) | Há um módulo explícito de engenharia de contexto, avaliações de agentes e rastreabilidade das alterações. | Delimitar se a formação abrangerá apenas desenvolvimento com agentes ou também a construção de sistemas agênticos. |
| [Pré-requisitos para assumir esse papel](#assunto-03) | A revisão da grade aponta leitura, runtime, modelo físico e assincronismo como lacunas relevantes. | Relacionar cada responsabilidade pretendida ao conhecimento e à prática necessários para exercê-la. |

## Texto de referência por assunto

<a id="assunto-01"></a>

### 1. Orquestrar, direcionar e tomar decisões

**O que já temos:** Você pede uma formação orientada à decisão e à condução dos agentes. A IA propõe um comparativo de competências.

**Para aprofundar:** Converter a descrição do papel em atividades observáveis, sem assumir como correto todo o contraste com a formação tradicional.

<a id="fonte-f024"></a>

#### F024 — Pedido de uma grade para orquestrar e decidir

Origem histórica: conversa original, linhas 437–438. Trecho principal desta etapa.

<!-- FONTE: F024 INICIO -->
> Com base no que discutimos e os para mtos levantados análise a grade curricular de um curso de engenharia de software e monte a nossa grade prática retira tópicos de programação já que nessa área o código é gerado pela ia o engeniro tem que entender como orquestrar, responder, direcionar e tomar todas as decisões
> 

<!-- FONTE: F024 FIM -->

<a id="fonte-f032"></a>

#### F032 — Comparação de papéis e competências pretendidas

Origem histórica: conversa original, linhas 540–549. Trecho principal desta etapa.

<!-- FONTE: F032 INICIO -->
> Comparativo: Grade Tradicional vs. Grade Prática do Orquestrador
> Dimensão	Engenharia Tradicional (Foco na Digitação)	Engenharia Moderna (Foco na Decisão)
> Atividade Principal	Escrever código, loops, classes e funções	Especificar requisitos em contratos e avaliar saídas
> Design de Software	Foco em padrões estruturais (ex.: Singleton, Visitor)	Foco em fronteiras de domínio, contratos e resiliência
> Garantia de Qualidade	Testes manuais ou testes unitários triviais de sintaxe	BDD, testes de propriedade e quality gates automatizados
> Dados e Persistência	Normalização até a 3ª forma normal e queries CRUD	Níveis de isolamento, concorrência, idempotência e sincronização
> Papel da IA	Ferramenta de autocompletar na IDE	Agente orquestrado sob restrições estritas de engenharia
> Habilidade Decisiva	Velocidade de digitação e memorização de APIs	Clareza analítica para julgar trade-offs de arquitetura
> Quer que eu monte o plano detalhado do Módulo 1 (Engenharia de Especificação) com exercícios práticos de orquestração de IA?
> 

<!-- FONTE: F032 FIM -->

<a id="assunto-02"></a>

### 2. Contexto, avaliações e governança de agentes

**O que já temos:** Há um módulo explícito de engenharia de contexto, avaliações de agentes e rastreabilidade das alterações.

**Para aprofundar:** Delimitar se a formação abrangerá apenas desenvolvimento com agentes ou também a construção de sistemas agênticos.

<a id="fonte-f031"></a>

#### F031 — Orquestração e governança de agentes

Origem histórica: conversa original, linhas 531–539. Cópia relacionada para este assunto. Destino principal: [anexo 09](09-texto-anexo.md#fonte-f031).

<!-- FONTE: F031 INICIO -->
> Módulo 7: Orquestração de Agentes e Governança de IA
> Objetivo: Dominar o fluxo de comando, supervisão e avaliação contínua de inteligências artificiais trabalhando no ecossistema de engenharia.
> 
> Engenharia de Contexto e Harness de Agentes: Arquitetura de arquivos de contexto, regras de escopo (.cursorrules, instruções de projeto) e limites de atenção de LLMs.
> 
> Pipelines de Avaliação Automatizada (Evals): Criação de testes de regressão que avaliam não apenas o software, mas a própria assertividade dos prompts e especificações dos agentes.
> 
> Governança Técnica e Auditoria: Rastreabilidade de alterações geradas por agentes, verificação de conformidade de licenças de código aberto e auditoria de segurança de artefatos gerados.
> 

<!-- FONTE: F031 FIM -->

<a id="assunto-03"></a>

### 3. Pré-requisitos para assumir esse papel

**O que já temos:** A revisão da grade aponta leitura, runtime, modelo físico e assincronismo como lacunas relevantes.

**Para aprofundar:** Relacionar cada responsabilidade pretendida ao conhecimento e à prática necessários para exercê-la.

<a id="fonte-f034"></a>

#### F034 — Lacuna de leitura e auditoria

Origem histórica: conversa original, linhas 562–579. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f034).

<!-- FONTE: F034 INICIO -->
> 1. Literacia de Leitura (Saber Ler Código 
> ≠
> 
> = Saber Digitar Código)
> O Gap: Eliminar a digitação manual de sintaxe não significa eliminar a necessidade de ler e rastrear código fluentemente.
> 
> O Risco na Tomada de Decisão: A IA vai gerar código com bugs sutis de lógica, loops com complexidade assintótica oculta (
> O
> (
> N
> 2
> )
> O(N 
> 2
>  )) ou vazamento de conexões. Se o engenheiro orquestrador não consegue bater o olho em um trecho de código gerado e apontar: "aqui você está abrindo uma transação no banco antes de fazer uma chamada HTTP externa", a spec falha na implementação.
> 
> O que falta: Treinamento deliberado em Auditoria e Leitura Crítica de Código, focado em fluxo de controle, variáveis de escopo e chamadas assíncronas.
> 

<!-- FONTE: F034 FIM -->

<a id="fonte-f035"></a>

#### F035 — Lacunas de máquina, runtime e assincronismo

Origem histórica: conversa original, linhas 580–600. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f035).

<!-- FONTE: F035 INICIO -->
> 2. O Modelo Físico da Máquina (Onde a Computação Acontece)
> O Gap: A grade vai direto para conceitos avançados como Circuit Breakers e Concorrência, mas uma pessoa sem base técnica não sabe o que é um processo do sistema operacional.
> 
> O Risco na Tomada de Decisão: Como especificar níveis de isolamento de banco de dados se a pessoa não entende a diferença entre ler um dado na memória RAM (nanossegundos) e buscar um dado no disco ou pela rede (milissegundos)? Decisões de arquitetura são puramente gestão de latência e consumo de recursos.
> 
> O que falta: Computação Pragmática: CPU (ciclos de processamento), Memória (Stack vs. Heap, ponteiros e referências), Disco (escrita sequencial vs. aleatória) e Rede (sockets, latência, perda de pacotes).
> 
> 3. Ambiente de Execução e "Chão de Fábrica" (CLI, Redes e Contêineres)
> O Gap: A grade salta do documento de requisitos para padrões arquiteturais abstratos, ignorando o ecossistema onde o código de fato roda.
> 
> O Risco na Tomada de Decisão: O código gerado pela IA precisará ser executado, testado e empacotado. Se a pessoa não domina terminal (CLI), variáveis de ambiente, portas de rede (TCP/UDP), permissões e contêineres (Docker), ela fica travada no primeiro erro de runtime (Connection Refused, Port 8080 already in use, CORS error).
> 
> O que falta: Engenharia de Runtime: Uso de linha de comando, isolamento com contêineres, inspeção de portas e configuração de ambientes de execução.
> 
> 4. Assincronismo e Gerenciamento de Estado
> O Gap: A maioria das falhas graves de sistemas modernos não decorre de regras de negócio erradas, mas de problemas temporais.
> 
> O Risco na Tomada de Decisão: A IA frequentemente gera códigos que causam deadlocks em bancos de dados ou criam condições de corrida (race conditions) em memória. Uma pessoa sem bagagem técnica tende a achar que o computador executa tudo de forma síncrona e linear, linha após linha.
> 
> O que falta: Entendimento visual e prático de Threads, Event Loops, promessas/tarefas assíncronas e concorrência na vida real.
> 

<!-- FONTE: F035 FIM -->

<a id="fonte-f065"></a>

#### F065 — Definição pessoal da jornada de estudo e autoria

Origem histórica: conversa original, linhas 1092–1094. Cópia relacionada para este assunto. Destino principal: [anexo 01](01-texto-anexo.md#fonte-f065).

<!-- FONTE: F065 INICIO -->
> Sim
> Como o livro vai ser o meu próprio caso de estudo, onde eu vou evoluir e, em consequência, vou documentar e vou escrever e vou exemplificar tudo aquilo que eu estou aprendendo para poder fazer cada capítulo do livro, que é o que eu vou aprender. Eu precisava de uma sequência lógica, estruturada e ordenada, onde uma pessoa técnica, com uma bagagem grande de conhecimento na área de tecnologia, mas com pouca experiência em criação de código, pudesse, eh, seguir essa sequência de estudo e pudesse realmente se tornar, eh, um engenheiro, eh, orquestrador.
> 

<!-- FONTE: F065 FIM -->
