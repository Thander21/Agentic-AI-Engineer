# 06. Texto anexo — A rota de autoestudo

[Etapa da jornada](06-a-rota-de-autoestudo.md) · [Índice](README.md) · [Mapa de origem](MAPA_ORIGEM.md)

Este anexo reúne 23 trechos: 8 principais e 15 cópias relacionadas. A organização abaixo identifica o que a conversa já oferece e o que ainda precisa ser aprofundado.

As sínteses são uma leitura editorial do material. Os blocos identificados como fonte preservam literalmente perguntas, respostas, exemplos e versões anteriores; sugestões da outra IA não passam a ser decisões aprovadas ou resultados comprovados por estarem neste anexo.

## Mapa de aprofundamento

| Assunto | O que já temos | O que aprofundar |
| --- | --- | --- |
| [O ciclo de autoestudo aplicado](#assunto-01) | A conversa propõe estudar a partir de uma dor do projeto, aplicar o conceito e escrever o aprendizado, inclusive com uma sugestão inicial de duração por atividade. | Definir disponibilidade real, tamanho do ciclo, revisão e critérios de avanço; os prazos sugeridos não foram demonstrados. |
| [Primeira grade: quatro fases](#assunto-02) | A primeira sequência reúne domínio e arquitetura, testes, dados e resiliência. | Identificar o que essa proposta pressupõe e quais assuntos continuam necessários na rota atual. |
| [Sete módulos e preparação para começar](#assunto-03) | A grade do orquestrador introduz sete módulos; a revisão acrescenta fundamentos de execução e leitura. | Relacionar módulos, pré-requisitos e atividades práticas antes de fechar uma ordem de estudo. |
| [Primeira sequência de sete fases ligada ao livro](#assunto-04) | Cada fase recebe um objetivo, assuntos de estudo e um capítulo sugerido, do modelo físico à operação. | Separar sequência de aprendizagem da sequência editorial e avaliar as dependências entre as fases. |
| [Sequência revisada com Engenharia de Software](#assunto-05) | A versão final reforça qualidade, requisitos, modularidade, verificação, dados e evolução. | Comparar as versões e recuperar explicitamente a orquestração de agentes, sem somar todas as grades como obrigações independentes. |

## Texto de referência por assunto

<a id="assunto-01"></a>

### 1. O ciclo de autoestudo aplicado

**O que já temos:** A conversa propõe estudar a partir de uma dor do projeto, aplicar o conceito e escrever o aprendizado, inclusive com uma sugestão inicial de duração por atividade.

**Para aprofundar:** Definir disponibilidade real, tamanho do ciclo, revisão e critérios de avanço; os prazos sugeridos não foram demonstrados.

<a id="fonte-f004"></a>

#### F004 — Estudo aplicado ao próprio produto

Origem histórica: conversa original, linhas 124–136. Trecho principal desta etapa.

<!-- FONTE: F004 INICIO -->
> O Caminho Rápido para Fechar a Lacuna
> Não tente ler manuais de 1.000 páginas do início ao fim sem contexto. Use o método de reengenharia reversa do seu próprio produto:
> 
> Pegue um módulo crítico que você já codificou (ex.: emissão de documento, cálculo de alíquotas ou sincronização com a nuvem).
> 
> Estude o livro de referência sobre o tema (veja referências como Domain-Driven Design de Eric Evans, Designing Data-Intensive Applications de Martin Kleppmann, ou Clean Architecture de Robert Martin).
> 
> Mapeie o que você fez versus o padrão formal: documente as diferenças, os atalhos tomados e como aquele módulo seria desenhado sob os padrões da indústria.
> 
> Esse exercício fornece tanto o vocabulário sênior quanto conteúdo de alto nível para artigos e discussões técnicas no LinkedIn.
> 
> Quer que eu monte um plano de estudos estruturado para os próximos 3 meses com os livros e referências essenciais?
> 

<!-- FONTE: F004 FIM -->

<a id="fonte-f014"></a>

#### F014 — Como estudar enquanto mantém as entregas

Origem histórica: conversa original, linhas 220–229. Trecho principal desta etapa.

<!-- FONTE: F014 INICIO -->
> Como Estudar sem Parar as Entregas Práticas
> Para quem já tem anos de prática e projetos rodando, o método mais eficiente é o estudo aplicado por refatoração:
> 
> Escolha um livro por vez: Comece por Unit Testing (Khorikov) ou Domain-Driven Design Distilled (Vernon).
> 
> Identifique um trecho do seu sistema: Pegue uma regra que hoje está densa, difícil de testar ou que depende diretamente de uma tabela do banco de dados.
> 
> Aplique o padrão estudado no código real: Reescreva a camada isolando o domínio e escreva os testes cobrindo as invariantes.
> 
> Esse ciclo fecha a lacuna teórica imediatamente e gera material concreto para documentações técnicas e artigos de autoridade.

<!-- FONTE: F014 FIM -->

<a id="fonte-f072"></a>

#### F072 — Ciclo proposto de estudo, aplicação e escrita

Origem histórica: conversa original, linhas 1204–1214. Trecho principal desta etapa.

<!-- FONTE: F072 INICIO -->
> A Dinâmica do Estudo Aplicado
> Para manter a consistência e não transformar o processo em uma sobrecarga teórica, cada fase deve seguir o mesmo ciclo de execução:
> 
> A Dor Real (1 semana): Identifique no seu sistema atual onde essa fase dói (ex.: na Fase 6, uma venda que trava o banco ou uma sincronização offline com conflito).
> 
> O Estudo Focado (1 semana): Leia os capítulos correspondentes dos livros clássicos (Kleppmann para dados, Khorikov para testes, Vernon para domínio) anotando apenas o que resolve aquela dor específica.
> 
> A Refatoração via IA (1 semana): Escreva a Spec técnica (SDD), submeta à IA, aplique os filtros de auditoria e implemente a correção no seu software.
> 
> O Registro do Capítulo (1 semana): Escreva o capítulo do livro detalhando: qual era o erro original, qual foi o raciocínio arquitetural aplicado, como a IA foi direcionada e qual foi o código resultante.
> 

<!-- FONTE: F072 FIM -->

<a id="fonte-f074"></a>

#### F074 — Possibilidade de detalhamento do cronograma

Origem histórica: conversa original, linhas 1217–1218. Trecho principal desta etapa.

<!-- FONTE: F074 INICIO -->
> Quer desenhar o cronograma prático para executar a Fase 1 (Modelo Físico e Recursos) no seu projeto nas próximas duas semanas?
> 

<!-- FONTE: F074 FIM -->

<a id="assunto-02"></a>

### 2. Primeira grade: quatro fases

**O que já temos:** A primeira sequência reúne domínio e arquitetura, testes, dados e resiliência.

**Para aprofundar:** Identificar o que essa proposta pressupõe e quais assuntos continuam necessários na rota atual.

<a id="fonte-f006"></a>

#### F006 — Grade inicial: modelagem e arquitetura

Origem histórica: conversa original, linhas 148–158. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f006).

<!-- FONTE: F006 INICIO -->
> Fase 1: Modelagem e Arquitetura de Software (O Núcleo da Aplicação)
> O objetivo desta fase é aprender a estruturar regras de negócio complexas sem deixá-las acopladas a bancos de dados, telas ou bibliotecas externas.
> 
> O que dominar:
> 
> Separação de camadas (Ports & Adapters / Arquitetura Hexagonal / Clean Architecture).
> 
> Domain-Driven Design (DDD): entidades, objetos de valor (Value Objects), agregados e fronteiras de contexto (Bounded Contexts).
> 
> Padrões de projeto com foco em redução de acoplamento (Injeção de Dependência, Strategy, Factory, Repository).
> 

<!-- FONTE: F006 FIM -->

<a id="fonte-f008"></a>

#### F008 — Grade inicial: testes e confiabilidade

Origem histórica: conversa original, linhas 167–177. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f008).

<!-- FONTE: F008 INICIO -->
> Fase 2: Rigor de Testes e Engenharia Confiável (A Rede de Proteção)
> Uma boa arquitetura é o que permite testar o software sem atrito. Nesta fase, o foco é transformar testes em ferramentas de design de código e validação de requisitos.
> 
> O que dominar:
> 
> Testes de unidade focados em comportamento e regras de negócio, não em detalhes de implementação.
> 
> Estratégias de isolamento de infraestrutura (uso de Testcontainers para bancos de dados reais vs. simuladores/mocks).
> 
> Especificação executável com BDD (Behavior-Driven Development) e testes orientados a propriedades (Property-Based Testing) para regras financeiras e cálculos matemáticos.
> 

<!-- FONTE: F008 FIM -->

<a id="fonte-f010"></a>

#### F010 — Grade inicial: dados, concorrência e sincronização

Origem histórica: conversa original, linhas 184–194. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f010).

<!-- FONTE: F010 INICIO -->
> Fase 3: Dados, Concorrência e Sincronização (O Mundo Real)
> Aqui você entra na camada de sistemas que precisam lidar com falhas de rede, operações concorrentes e integridade estrita de dados.
> 
> O que dominar:
> 
> Transacionalidade em bancos relacionais: níveis de isolamento (Dirty Read, Non-repeatable Read, Phantom Read, Serializable) e bloqueios (Locking otimista vs. pessimista).
> 
> Idempotência em APIs e mensageria (chaves de idempotência, tratamento de requisições duplicadas).
> 
> Arquiteturas Offline-First, filas locais de persistência, resolução de conflitos e reconciliação com a nuvem.
> 

<!-- FONTE: F010 FIM -->

<a id="fonte-f012"></a>

#### F012 — Grade inicial: resiliência, segurança e operação

Origem histórica: conversa original, linhas 201–211. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f012).

<!-- FONTE: F012 INICIO -->
> Fase 4: Resiliência, Segurança Aplicada e Operação em Produção
> A fase final consolida o papel do arquiteto: garantir que o sistema não apenas funcione no "caminho feliz", mas suporte falhas de serviços de terceiros e seja diagnosticável sem intervenção manual destrutiva.
> 
> O que dominar:
> 
> Padrões de estabilidade: Circuit Breaker, Retry com Exponential Backoff e Jitter, Bulkhead e Dead Letter Queues.
> 
> Criptografia aplicada a negócios: funcionamento de certificados digitais (PKI, X.509), cadeias de assinatura, hashing e armazenamento seguro de segredos.
> 
> Observabilidade moderna com OpenTelemetry: instrumentação de logs estruturados correlacionados (Trace ID), métricas de saúde e rastreamento distribuído.
> 

<!-- FONTE: F012 FIM -->

<a id="assunto-03"></a>

### 3. Sete módulos e preparação para começar

**O que já temos:** A grade do orquestrador introduz sete módulos; a revisão acrescenta fundamentos de execução e leitura.

**Para aprofundar:** Relacionar módulos, pré-requisitos e atividades práticas antes de fechar uma ordem de estudo.

<a id="fonte-f026"></a>

#### F026 — Visão geral da grade de sete módulos

Origem histórica: conversa original, linhas 454–466. Trecho principal desta etapa.

<!-- FONTE: F026 INICIO -->
> A Nova Grade Prática: O Engenheiro Orquestrador e Decisor
> Esta grade substitui a digitação de código pelo domínio de especificação, governança, topologia de sistemas e controle de qualidade automatizado.
> 
> [Nível 1: Especificação & Modelagem] ──> [Nível 2: Topologia & Arquitetura]
>                  │                                        │
>                  ▼                                        ▼
> [Nível 3: Consistência & Dados]      ──> [Nível 4: Redes de Contenção & Testes]
>                  │                                        │
>                  ▼                                        ▼
> [Nível 5: Resiliência & Segurança]   ──> [Nível 6: Observabilidade & Produção]
>                                      │
>                                      ▼
>                    [Nível 7: Orquestração de Agentes]

<!-- FONTE: F026 FIM -->

<a id="fonte-f037"></a>

#### F037 — Reorganização com módulos preparatórios

Origem histórica: conversa original, linhas 608–618. Trecho principal desta etapa.

<!-- FONTE: F037 INICIO -->
> A Correção da Grade: O "Módulo Zero" e a Mudança de Dinâmica
> Para que uma pessoa leiga se torne de fato uma orquestradora capaz de especificar e direcionar implementações com autonomia, a grade precisa de uma reorganização estrutural:
> 
> Módulo Adicional / Ajustado	O Que Ensina	O Que Habilita na Decisão da Spec
> Módulo 0: Fundamentos Físicos de Execução	Como memória, disco, CPU e rede operam. O terminal Linux, contêineres (Docker) e o ciclo de vida de um processo.	Saber onde o software vai rodar, seus limites de hardware e como subir o ambiente de teste local.
> Módulo 0.5: Literacia e Auditoria de Código	Como ler árvores de código, rastrear chamadas assíncronas e inspecionar consumo de recursos via debuggers/profilers.	Capacidade de validar se o código gerado pelo agente reflete a intenção da spec e não possui armadilhas invisíveis.
> Ajuste Pedagógico: Laboratórios de Quebra (Chaos Labs)	Em vez de mandar a IA escrever código novo, o aluno recebe códigos quebrados e deve usar a IA para diagnosticar a causa-raiz.	Constrói a intuição de causa e efeito indispensável para prever cenários de erro durante a escrita da spec.
> Com essa base mecânica e a capacidade de auditar o que a IA entrega, a transição para Spec-Driven Development, Domain-Driven Design e governança de agentes torna-se sólida, evitando que o profissional seja apenas um operador passivo de ferramentas generativas.
> 
> Quer ver como ficaria a ementa prática desse 'Módulo 0' focada exclusivamente em leitura, runtime e modelo mental da máquina?
> 

<!-- FONTE: F037 FIM -->

<a id="assunto-04"></a>

### 4. Primeira sequência de sete fases ligada ao livro

**O que já temos:** Cada fase recebe um objetivo, assuntos de estudo e um capítulo sugerido, do modelo físico à operação.

**Para aprofundar:** Separar sequência de aprendizagem da sequência editorial e avaliar as dependências entre as fases.

<a id="fonte-f066"></a>

#### F066 — Introdução à primeira sequência de sete fases

Origem histórica: conversa original, linhas 1095–1098. Trecho principal desta etapa.

<!-- FONTE: F066 INICIO -->
> Para estruturar a sua própria jornada e transformá-la no índice sequencial do livro, a trilha precisa seguir uma ordem estrita de causa e efeito: você só pode orquestrar o que sabe auditar, só pode auditar o que sabe testar, e só pode testar o que sabe especificar.
> 
> A sequência lógica abaixo divide esse aprendizado em 7 fases progressivas. Cada fase representa um ciclo completo de estudo pessoal, aplicação no seu projeto real e redação do respectivo capítulo do livro.
> 

<!-- FONTE: F066 FIM -->

<a id="fonte-f067"></a>

#### F067 — Primeira sequência: modelo físico e execução

Origem histórica: conversa original, linhas 1099–1113. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f067).

<!-- FONTE: F067 INICIO -->
> Fase 1: Conectar a Infraestrutura ao Código (O Modelo Físico de Execução)
> Objetivo: Usar sua experiência prévia em servidores, banco e sistemas operacionais como alavanca para entender o comportamento do software em memória.
> 
> O que estudar e praticar:
> 
> O caminho da execução: como o código sai do disco, vira binário/bytecode e consome recursos da CPU e memória (Stack vs. Heap, alocação e liberação de recursos).
> 
> O custo real da latência: a diferença de tempo de resposta entre ler a memória RAM, acessar disco SSD e fazer uma requisição via rede.
> 
> O ciclo de vida de um processo do sistema operacional: portas, sockets, variáveis de ambiente e contenção de threads.
> 
> A virada de chave: Parar de enxergar o código como "texto mágico" e passar a vê-lo como um consumidor de recursos físicos de uma máquina.
> 
> Capítulo gerado: A Máquina Invisível: Como o Código Realmente Consome a Infraestrutura.
> 

<!-- FONTE: F067 FIM -->

<a id="fonte-f068"></a>

#### F068 — Primeira sequência: leitura e filtros de auditoria

Origem histórica: conversa original, linhas 1114–1128. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f068).

<!-- FONTE: F068 INICIO -->
> Fase 2: Literacia Diagnóstica e os 5 Filtros de Auditoria
> Objetivo: Adquirir a capacidade de inspecionar, criticar e rejeitar código gerado por IA em minutos sem precisar aprender a digitar sintaxe do zero.
> 
> O que estudar e praticar:
> 
> Leitura por amostragem: identificação rápida de contratos de entrada/saída, assinaturas de métodos e fluxo de dependências.
> 
> O método dos 5 Filtros na prática: Contrato, Efeitos Colaterais (I/O), Invariantes por Busca Rápida (Ctrl+F), Asserção de Teste e Inspeção de Logs.
> 
> Reconhecimento de armadilhas clássicas da IA: chamadas assíncronas bloqueantes, loops aninhados com chamadas externas (N+1) e dependências alucinadas.
> 
> A virada de chave: Compreender que auditar código é uma habilidade de reconhecimento de padrões, e não de digitação criativa.
> 
> Capítulo gerado: Auditoria Cirúrgica: Como Ler e Conter Código Sem Passar Anos Programando.
> 

<!-- FONTE: F068 FIM -->

<a id="fonte-f069"></a>

#### F069 — Primeira sequência: especificação e domínio

Origem histórica: conversa original, linhas 1129–1143. Cópia relacionada para este assunto. Destino principal: [anexo 09](09-texto-anexo.md#fonte-f069).

<!-- FONTE: F069 INICIO -->
> Fase 3: Engenharia de Especificação (SDD) e Modelagem de Domínio
> Objetivo: Aprender a formular o problema de negócio de forma tão precisa que a IA não tenha margem para inventar regras ou desviar do escopo.
> 
> O que estudar e praticar:
> 
> Spec-Driven Development (SDD): redação de especificações com escopos fechados, pré-condições, pós-condições e limites explícitos (Non-Goals).
> 
> Domain-Driven Design (DDD) Estratégico: criação de linguagem ubíqua e isolamento de modelos ricos contra modelos anêmicos.
> 
> Objetos de Valor (Value Objects) e Invariantes: impedir que estados inválidos (ex.: dinheiro negativo, alíquota de imposto incoerente) existam na aplicação.
> 
> A virada de chave: Substituir descrições vagas de requisitos por contratos matemáticos e semânticos inegociáveis.
> 
> Capítulo gerado: A Arte da Especificação: Modelando Domínios Blindados Antes da Primeira Linha de Código.
> 

<!-- FONTE: F069 FIM -->

<a id="fonte-f070"></a>

#### F070 — Primeira sequência: testes e validação

Origem histórica: conversa original, linhas 1144–1158. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f070).

<!-- FONTE: F070 INICIO -->
> Fase 4: A Rede de Contenção (BDD, Testes de Propriedade e Anti-Tautologia)
> Objetivo: Dominar as técnicas que provam matematicamente se a implementação da IA funciona, eliminando falsos positivos.
> 
> O que estudar e praticar:
> 
> BDD com Gherkin: escrita de cenários executáveis baseados em comportamento de negócio antes de acionar a IA para codificar.
> 
> Desmascarando testes tautológicos: como verificar se um teste falha de verdade quando a regra é violada (testes de mutação conceituais).
> 
> Testes baseados em propriedades (Property-Based Testing): definição de invariantes globais e geração de centenas de entradas extremas para tentar quebrar a lógica gerada.
> 
> A virada de chave: Entender que a suíte de testes não serve para "agradar o pipeline", mas para ser a cerca elétrica que impede a IA de alucinar.
> 
> Capítulo gerado: Testes Reais vs. Testes Placebo: Construindo a Rede de Proteção Contra a IA.
> 

<!-- FONTE: F070 FIM -->

<a id="fonte-f071"></a>

#### F071 — Primeira sequência: arquitetura, dados e operação

Origem histórica: conversa original, linhas 1159–1203. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f071).

<!-- FONTE: F071 INICIO -->
> Fase 5: Fronteiras Arquiteturais e Desacoplamento (Clean & Hexagonal)
> Objetivo: Estruturar o sistema para que bancos de dados, telas e bibliotecas externas sejam apenas detalhes substituíveis ao redor da regra de negócio.
> 
> O que estudar e praticar:
> 
> Ports & Adapters (Arquitetura Hexagonal): definição de interfaces para tudo o que entra (APIs, UI) e tudo o que sai (Bancos, Serviços Fiscais, Filas).
> 
> Inversão de Dependência na prática: fazer o mecanismo de banco de dados depender do modelo de negócio, nunca o inverso.
> 
> Estruturação de diretórios e módulos para isolamento de contexto.
> 
> A virada de chave: Perceber que uma boa arquitetura permite trocar o banco de dados ou reescrever uma tela inteira via IA sem alterar uma única linha da regra de negócio central.
> 
> Capítulo gerado: Fronteiras e Portas: Desacoplando o Negócio dos Detalhes Tecnológicos.
> 
> Fase 6: Dados, Concorrência e Conflitos do Mundo Real
> Objetivo: Resolver os gargalos onde a teoria falha: múltiplos usuários acessando os mesmos dados, quedas de conexão e concorrência.
> 
> O que estudar e praticar:
> 
> Níveis de isolamento em bancos relacionais e impactos em cenários concorrentes (Deadlocks, Phantom Reads).
> 
> Travamento otimista vs. pessimista para integridade de estoque e faturamento.
> 
> Arquiteturas Offline-First: persistência local resiliente, filas de sincronização, reconciliação e chaves de idempotência em transações financeiras.
> 
> A virada de chave: Parar de planejar sistemas apenas para o "caminho feliz" e projetar o software assumindo que a rede sempre falhará e que o hardware local oscilará.
> 
> Capítulo gerado: O Caos da Concorrência: Transações, Idempotência e Sistemas Offline-First.
> 
> Fase 7: Resiliência, Criptografia e Observabilidade em Produção
> Objetivo: Tornar o sistema autônomo, seguro contra fraudes fiscais/regulatórias e diagnosticável sem acesso manual invasivo.
> 
> O que estudar e praticar:
> 
> Padrões de estabilidade: Circuit Breakers, Retries com Backoff Exponencial e Bulkheads para chamadas de APIs externas (como servidores tributários e gateways de pagamento).
> 
> Criptografia aplicada a processos: certificados digitais (X.509/PKI), hashes imutáveis e cadeias de integridade de dados.
> 
> Telemetria moderna: instrumentação com OpenTelemetry, rastreamento distribuído (Traces) e logs estruturados correlacionados com ID de transação.
> 
> A virada de chave: Passar a diagnosticar a causa-raiz de qualquer pane em produção em poucos minutos através de gráficos de telemetria e traces, sem adivinhação.
> 
> Capítulo gerado: Operação de Missão Crítica: Resiliência, Criptografia e Telemetria em Produção.
> 

<!-- FONTE: F071 FIM -->

<a id="assunto-05"></a>

### 5. Sequência revisada com Engenharia de Software

**O que já temos:** A versão final reforça qualidade, requisitos, modularidade, verificação, dados e evolução.

**Para aprofundar:** Comparar as versões e recuperar explicitamente a orquestração de agentes, sem somar todas as grades como obrigações independentes.

<a id="fonte-f078"></a>

#### F078 — Visão geral da sequência revisada de sete fases

Origem histórica: conversa original, linhas 1287–1302. Trecho principal desta etapa.

<!-- FONTE: F078 INICIO -->
> A Nova Estrutura Enriquecida das 7 Fases
> Com a infusão da matéria formal de Engenharia de Software, as sete fases tornam-se profundamente técnicas, equilibrando a fundamentação científica e a orquestração pragmática de IA.
> 
> Fase 1: O Modelo Físico & Runtime (Infraestrutura de Computação)
>    │
> Fase 2: Métricas de Qualidade & Auditoria Estática (SQA & McCabe)
>    │
> Fase 3: Engenharia de Requisitos & SDD (Rastreabilidade & NFRs)
>    │
> Fase 4: Teoria de Modularidade & Design (Parnas, Coesão & SOLID)
>    │
> Fase 5: Verificação, Validação & Redes de Contenção (V&V, BDD & Mutação)
>    │
> Fase 6: Concorrência, Transações & Consistência de Dados (ACID & CAP)
>    │
> Fase 7: Evolução, Manutenção & Resiliência de Sistemas (Lehman & SRE)

<!-- FONTE: F078 FIM -->

<a id="fonte-f079"></a>

#### F079 — Sequência revisada: computação e runtime

Origem histórica: conversa original, linhas 1303–1311. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f079).

<!-- FONTE: F079 INICIO -->
> Fase 1: Fundamentos de Computação e Runtime
> A base da ciência da computação conectada ao chão de fábrica.
> 
> Engenharia de Software: O papel do runtime, gerenciamento de memória (Stack vs. Heap, Garbage Collection e ciclos de coleta), latência de I/O em ordens de magnitude.
> 
> Sistemas Operacionais: Processos, Threads, Concorrência preemptiva, descritores de arquivo e portas TCP/UDP.
> 
> Aplicação com IA: Diagnosticar se o código gerado pelo agente respeita os limites físicos de memória e concorrência do ambiente de execução.
> 

<!-- FONTE: F079 FIM -->

<a id="fonte-f080"></a>

#### F080 — Sequência revisada: qualidade e auditoria

Origem histórica: conversa original, linhas 1312–1320. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f080).

<!-- FONTE: F080 INICIO -->
> Fase 2: Garantia da Qualidade (SQA), Métricas Estáticas e Auditoria
> A ciência da medição de código sem necessidade de leitura linha por linha.
> 
> Engenharia de Software: Análise Estática de Código (SAST), Complexidade Ciclomática (McCabe), Métricas de Acoplamento Aferente e Eferente, e Leis de Halstead.
> 
> Os 5 Filtros Enriquecidos: Auditoria visual de assinaturas, rastreamento de efeitos colaterais de I/O, verificação de invariantes, asserções de teste e profiling.
> 
> Aplicação com IA: Configurar linters e analisadores estáticos que barram automaticamente qualquer entrega de IA com complexidade ciclomática ou acoplamento excessivo.
> 

<!-- FONTE: F080 FIM -->

<a id="fonte-f081"></a>

#### F081 — Sequência revisada: requisitos e SDD

Origem histórica: conversa original, linhas 1321–1329. Cópia relacionada para este assunto. Destino principal: [anexo 09](09-texto-anexo.md#fonte-f081).

<!-- FONTE: F081 INICIO -->
> Fase 3: Engenharia de Requisitos, Atributos de Qualidade e SDD
> Como transformar problemas ambíguos de negócio em especificações determinísticas.
> 
> Engenharia de Software: Elicitação e especificação de requisitos, Requisitos Não-Funcionais (NFRs), Cenários de Atributos de Qualidade e Matrizes de Rastreabilidade.
> 
> Domain-Driven Design Estratégico: Linguagem Ubíqua, Bounded Contexts, Context Mapping e a erradicação de Modelos Anêmicos.
> 
> Aplicação com IA: Elaboração de Especificações Técnicas (SDD) com escopos negativos (Non-Goals) explícitos e contratos formais que impedem alucinações de escopo.
> 

<!-- FONTE: F081 FIM -->

<a id="fonte-f082"></a>

#### F082 — Sequência revisada: modularidade e arquitetura

Origem histórica: conversa original, linhas 1330–1338. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f082).

<!-- FONTE: F082 INICIO -->
> Fase 4: Teoria Formal da Modularidade e Arquitetura de Software
> A matemática do baixo acoplamento e da alta coesão.
> 
> Engenharia de Software: O princípio de Information Hiding de David Parnas; os 7 níveis de coesão e acoplamento; princípios SOLID fundamentados em álgebra de tipos e teoria de contratos; Lei de Conway.
> 
> Estilos Arquiteturais: Arquitetura em Camadas, Hexagonal (Ports & Adapters) e Clean Architecture; Monolito Modular vs. Serviços Distribuídos.
> 
> Aplicação com IA: Instruir a IA a estruturar o projeto de forma que os adaptadores externos (bancos, telas, APIs de terceiros) sejam plugáveis e substituíveis sem impactar o núcleo de regras.
> 

<!-- FONTE: F082 FIM -->

<a id="fonte-f083"></a>

#### F083 — Sequência revisada: verificação e validação

Origem histórica: conversa original, linhas 1339–1347. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f083).

<!-- FONTE: F083 INICIO -->
> Fase 5: Verificação, Validação (V&V) e Redes de Contenção
> A distinção clássica: "Estamos construindo o produto certo?" (Validação) vs. "Estamos construindo o produto do jeito certo?" (Verificação).
> 
> Engenharia de Software: Pirâmide e Troféu de Testes; BDD (Behavior-Driven Development) como especificação executável; Property-Based Testing e Invariantes Matemáticas; Testes de Mutação para auditoria da suíte de testes.
> 
> Engenharia de Contratos: Design by Contract (Pré-condições, Pós-condições, Invariantes).
> 
> Aplicação com IA: Gerar testes comportamentais antes da implementação do código e utilizar testes de mutação para expor testes tautológicos gerados pela IA.
> 

<!-- FONTE: F083 FIM -->

<a id="fonte-f084"></a>

#### F084 — Sequência revisada: dados, evolução e resiliência

Origem histórica: conversa original, linhas 1348–1365. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f084).

<!-- FONTE: F084 INICIO -->
> Fase 6: Engenharia de Dados, Concorrência e Teoria de Distribuição
> Onde a física impõe restrições à lógica.
> 
> Engenharia de Software: Teoria de Bancos Relacionais, transacionalidade ACID, anomalias de concorrência (Dirty Read, Non-Repeatable Read, Phantom Read) e estratégias de lock (otimista vs. pessimista).
> 
> Teorema CAP e PACELC: Consistência forte vs. eventual; Padrão Saga vs. transações distribuídas (2PC); idempotência em mensageria e APIs.
> 
> Aplicação com IA: Desenhar sistemas Offline-First com sincronização resiliente, evitando race conditions e deadlocks em códigos concorrentes gerados por IA.
> 
> Fase 7: Evolução, Manutenção de Software e Resiliência em Produção
> Garantindo que o sistema sobreviva ao tempo e às mudanças de mercado.
> 
> Engenharia de Software: Leis de Lehman de Evolução de Software; gestão do ciclo de vida e pagamento de Dívida Técnica; Padrão Strangler Fig para modernização de legados; padrões de versionamento e compatibilidade (SemVer, Expand and Contract).
> 
> Resiliência e Observabilidade: Padrões de estabilidade (Circuit Breaker, Bulkhead, Retry com Exponential Backoff e Jitter); telemetria (OpenTelemetry: logs estruturados, métricas e traces); Criptografia aplicada (PKI, X.509, hashing e integridade de registros).
> 
> Aplicação com IA: Implementar observabilidade contínua para auditar sistemas em produção e orquestrar refatorações seguras de módulos legados.
> 

<!-- FONTE: F084 FIM -->
