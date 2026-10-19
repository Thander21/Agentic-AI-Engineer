# 11. Texto anexo — Autonomia conquistada

[Etapa da jornada](11-autonomia-conquistada.md) · [Índice](README.md) · [Mapa de origem](MAPA_ORIGEM.md)

Este anexo reúne 10 trechos: 2 principais e 8 cópias relacionadas. A organização abaixo identifica o que a conversa já oferece e o que ainda precisa ser aprofundado.

As sínteses são uma leitura editorial do material. Os blocos identificados como fonte preservam literalmente perguntas, respostas, exemplos e versões anteriores; sugestões da outra IA não passam a ser decisões aprovadas ou resultados comprovados por estarem neste anexo.

## Mapa de aprofundamento

| Assunto | O que já temos | O que aprofundar |
| --- | --- | --- |
| [Capacidades que se deseja adquirir](#assunto-01) | Você quer tomar decisões e seguir uma sequência que produza autonomia prática. | Definir competências observáveis e uma referência inicial para acompanhar o progresso. |
| [Evidências sobre o software](#assunto-02) | A conversa propõe testes, filtros e verificações de comportamento. | Distinguir um resultado correto do produto da capacidade pessoal de explicar, reproduzir e transferir o raciocínio. |
| [Promessas que não substituem avaliação](#assunto-03) | Há afirmações de senioridade ao concluir um exercício ou ciclo e critérios numéricos apresentados como absolutos. | Construir critérios proporcionais à evidência e delimitar aquilo que cada demonstração permite concluir. |
| [Aprendizagem do leitor como outra avaliação](#assunto-04) | O exemplo editorial define objetivos e exercícios para o leitor. | Separar avaliação do autor, qualidade do produto e aprendizado de quem lê o livro. |

## Texto de referência por assunto

<a id="assunto-01"></a>

### 1. Capacidades que se deseja adquirir

**O que já temos:** Você quer tomar decisões e seguir uma sequência que produza autonomia prática.

**Para aprofundar:** Definir competências observáveis e uma referência inicial para acompanhar o progresso.

<a id="fonte-f024"></a>

#### F024 — Pedido de uma grade para orquestrar e decidir

Origem histórica: conversa original, linhas 437–438. Cópia relacionada para este assunto. Destino principal: [anexo 03](03-texto-anexo.md#fonte-f024).

<!-- FONTE: F024 INICIO -->
> Com base no que discutimos e os para mtos levantados análise a grade curricular de um curso de engenharia de software e monte a nossa grade prática retira tópicos de programação já que nessa área o código é gerado pela ia o engeniro tem que entender como orquestrar, responder, direcionar e tomar todas as decisões
> 

<!-- FONTE: F024 FIM -->

<a id="fonte-f065"></a>

#### F065 — Definição pessoal da jornada de estudo e autoria

Origem histórica: conversa original, linhas 1092–1094. Cópia relacionada para este assunto. Destino principal: [anexo 01](01-texto-anexo.md#fonte-f065).

<!-- FONTE: F065 INICIO -->
> Sim
> Como o livro vai ser o meu próprio caso de estudo, onde eu vou evoluir e, em consequência, vou documentar e vou escrever e vou exemplificar tudo aquilo que eu estou aprendendo para poder fazer cada capítulo do livro, que é o que eu vou aprender. Eu precisava de uma sequência lógica, estruturada e ordenada, onde uma pessoa técnica, com uma bagagem grande de conhecimento na área de tecnologia, mas com pouca experiência em criação de código, pudesse, eh, seguir essa sequência de estudo e pudesse realmente se tornar, eh, um engenheiro, eh, orquestrador.
> 

<!-- FONTE: F065 FIM -->

<a id="assunto-02"></a>

### 2. Evidências sobre o software

**O que já temos:** A conversa propõe testes, filtros e verificações de comportamento.

**Para aprofundar:** Distinguir um resultado correto do produto da capacidade pessoal de explicar, reproduzir e transferir o raciocínio.

<a id="fonte-f029"></a>

#### F029 — Qualidade, testes e revisão de código gerado

Origem histórica: conversa original, linhas 500–510. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f029).

<!-- FONTE: F029 INICIO -->
> Módulo 4: Redes de Contenção, Invariantes e Quality Gates
> Objetivo: Criar barreiras matemáticas e lógicas automatizadas que barram o código gerado por IA antes de qualquer deploy.
> 
> Engenharia de Testes de Comportamento (BDD): Escrita de critérios de aceitação executáveis em Gherkin antes da solicitação de código ao agente.
> 
> Testes Baseados em Propriedades (Property-Based Testing): Definição de invariantes universais (ex.: "saldo final = entradas - saídas") e geração aleatória massiva de cenários extremos para quebrar implementações sugeridas pela IA.
> 
> Testes de Mutação: Validação da eficácia da suíte de testes (garantir que os testes realmente falham quando regras são violadas).
> 
> Revisão Semântica de Código: Análise de vulnerabilidades sutis em código de IA: vazamentos de escopo, dependências fantasmas (package hallucinations) e complexidade ciclomática oculta.
> 

<!-- FONTE: F029 FIM -->

<a id="fonte-f057"></a>

#### F057 — Cinco filtros consolidados no blueprint

Origem histórica: conversa original, linhas 939–975. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f057).

<!-- FONTE: F057 INICIO -->
> ## 2. O Método dos 5 Filtros de Auditoria Rápida
> 
> Quando a IA entrega uma funcionalidade acompanhada de código e testes, o orquestrador submete os artefatos a uma triagem de até 3 minutos:
> 
> [Artefato Gerado pela IA]
> │
> ├──► 1. Contrato (Assinaturas): O que entra e o que sai é suficiente?
> ├──► 2. Efeitos Colaterais (I/O): Onde toca em rede, disco ou banco? Há loops ou transações abertas?
> ├──► 3. Invariante (Ctrl+F): A regra matemática ou de negócio foi respeitada no condicional?
> ├──► 4. Auditoria do Teste: O teste falha se eu alterar a expectativa para um valor incorreto?
> └──► 5. Inspeção Viva (Telemetria): O log/debugger mostra latência anormal ou contenção?
> 
> 
> ### Detalhamento dos Filtros
> 
> 1. **Filtro de Contrato (Assinatura e Tipagem):**
>    * *Ação:* Inspecionar exclusivamente os parâmetros de entrada e o objeto de retorno.
>    * *Pergunta de controle:* O contrato expõe todos os dados necessários para o chamador sem forçar consultas redundantes posteriores?
> 
> 2. **Filtro de Efeitos Colaterais (I/O, Banco e Rede):**
>    * *Ação:* Rastrear termos como `await`, `SELECT`, `transacao`, `HTTP` e chamadas a serviços externos.
>    * *Pergunta de controle:* Existem chamadas lentas de rede dentro de transações ACID? Existem consultas ao banco de dados presas dentro de laços (`for`/`foreach`)?
> 
> 3. **Filtro de Invariantes por Hipótese:**
>    * *Ação:* Buscar diretamente no código os valores-chave da regra de negócio (ex.: `0.15` para 15% de desconto, limites de crédito, faixas de alíquota).
>    * *Pergunta de controle:* A condição lógica representa a regra real ou confunde grandezas (ex.: porcentagem tratada como valor absoluto)?
> 
> 4. **Filtro de Auditoria do Teste:**
>    * *Ação:* Ignorar a taxa percentual de cobertura e ler diretamente as asserções (`Assert`) dos testes gerados.
>    * *Pergunta de controle:* O teste valida cálculos reais ou apenas confere se a função retornou sem disparar erro? Se o valor esperado for sabotado manualmente, o teste quebra?
> 
> 5. **Filtro de Inspeção Viva (Telemetria e Logs):**
>    * *Ação:* Observar a saída do terminal de execução, logs estruturados ou rastreamento de chamadas.
>    * *Pergunta de controle:* Qual foi a latência real entre o início e o fim da operação? Houve excesso de comandos disparados contra o banco?
> 
> ---
> 

<!-- FONTE: F057 FIM -->

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

<a id="assunto-03"></a>

### 3. Promessas que não substituem avaliação

**O que já temos:** Há afirmações de senioridade ao concluir um exercício ou ciclo e critérios numéricos apresentados como absolutos.

**Para aprofundar:** Construir critérios proporcionais à evidência e delimitar aquilo que cada demonstração permite concluir.

<a id="fonte-f054"></a>

#### F054 — Conclusões e alcance atribuídos ao exercício

Origem histórica: conversa original, linhas 891–913. Trecho principal desta etapa.

<!-- FONTE: F054 INICIO -->
> O Que Esse Exercício Prova
> Você não precisou:
> 
> Lembrar de cabeça a sintaxe de async/await ou using var.
> 
> Saber como o Entity Framework mapeia tabelas internamente.
> 
> Digitar 80 linhas de classes e métodos.
> 
> Você precisou apenas de:
> 
> Saber o que procurar: Onde o código fala com o mundo externo (banco e HTTP).
> 
> Checar o contrato: Entrada e saída.
> 
> Validar a invariante com busca direta: A regra do negócio (0.15).
> 
> Desconfiar do teste superficial: O teste validou o comportamento ou apenas um Guid?
> 
> Esse é o modelo exato que capacita um profissional sem anos de digitação de código a liderar e orquestrar agentes com segurança de nível sênior.
> 
> Quer transformar esse método dos 5 Filtros em um capítulo estruturado com exercícios no sumário do livro?
> 

<!-- FONTE: F054 FIM -->

<a id="fonte-f073"></a>

#### F073 — Resultados prometidos para o ciclo: a verificar

Origem histórica: conversa original, linhas 1215–1216. Trecho principal desta etapa.

<!-- FONTE: F073 INICIO -->
> Ao final desse ciclo em 7 fases, você terá modernizado completamente o seu produto, adquirido senioridade arquitetural comprovada e concluído o manuscrito de um livro 100% ancorado na realidade da engenharia moderna.
> 

<!-- FONTE: F073 FIM -->

<a id="fonte-f076"></a>

#### F076 — Métricas estáticas e análise de mutação

Origem histórica: conversa original, linhas 1253–1268. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f076).

<!-- FONTE: F076 INICIO -->
> 3. Métricas de Código e Garantia de Qualidade de Software (SQA)
> Para quem não lê milhares de linhas geradas pela IA, a Engenharia de Software oferece métricas estáticas objetivas:
> 
> Complexidade Ciclomática (Thomas McCabe): Quantidade de caminhos de execução independentes no código. Se a IA entrega uma função com complexidade ciclomática 
> >
> 10
> >10, a função é matematicamente propensa a bugs e deve ser sumariamente rejeitada.
> 
> Instabilidade (
> I
> I) e Abstração (
> A
> A): As métricas de Robert Martin para pacotes: um módulo central deve ser altamente abstrato e estável; módulos de borda devem ser flexíveis.
> 
> Cobertura de Código Efetiva (Análise de Mutação): O conceito formal de Mutation Testing, onde ferramentas injetam falhas deliberadas no código para provar se a suíte de testes realmente detecta anomalias.
> 

<!-- FONTE: F076 FIM -->

<a id="assunto-04"></a>

### 4. Aprendizagem do leitor como outra avaliação

**O que já temos:** O exemplo editorial define objetivos e exercícios para o leitor.

**Para aprofundar:** Separar avaliação do autor, qualidade do produto e aprendizado de quem lê o livro.

<a id="fonte-f020"></a>

#### F020 — Exemplo de spec editorial: escopo e objetivos

Origem histórica: conversa original, linhas 339–373. Cópia relacionada para este assunto. Destino principal: [anexo 15](15-texto-anexo.md#fonte-f020).

<!-- FONTE: F020 INICIO -->
> Markdown
> # SPEC-CH-04: Modelagem de Regras de Negócio Sem Depender do Banco
> 
> ## 1. Metadados e Contrato de Escopo
> 
> * **Capítulo:** 04 (Parte II: O Núcleo do Domínio)
> * **Público-Alvo:** Desenvolvedor prático que constrói CRUDs diretamente acoplados ao banco de dados e quer aprender a isolar regras de negócio críticas.
> * **Tempo Estimado de Leitura:** 22 minutos
> * **Extensão Alvo:** 2.800 a 3.400 palavras
> 
> ### 1.1. Objetivo Central de Transformação
> O leitor deve ser capaz de identificar um modelo de domínio anêmico, refatorá-lo para uma entidade rica com invariantes protegidas e testar essa regra em memória em menos de 10 milissegundos, sem instanciar banco de dados, ORM ou framework web.
> 
> ### 1.2. Pré-requisitos Assumidos
> * Compreensão básica de classes, métodos e tipos primitivos.
> * Familiaridade com escrita de funções que recebem parâmetros e retornam valores.
> * Git básico (leitura do repositório de exemplos do livro).
> 
> ### 1.3. Fora de Escopo (Non-Goals Explícitos)
> * **Proibido neste capítulo:** Configurações de ORM (Entity Framework, Prisma, Dapper, etc.).
> * **Proibido neste capítulo:** Criação de tabelas, migrações SQL ou scripts DDL.
> * **Proibido neste capítulo:** Discussões sobre microsserviços, mensageria externa ou eventos distribuídos.
> * **Justificativa do corte:** O leitor iniciante tende a misturar o design do dado com o mecanismo de persistência. O foco aqui é 100% lógica pura em memória.
> 
> ### 1.4. Novo Vocabulário Introduzido
> * **Invariante:** Regra de negócio inegociável que o objeto não permite ser violada em momento algum.
> * **Objeto de Valor (Value Object):** Objeto definido por seus atributos, imutável e sem identidade própria.
> * **Modelo Anêmico:** Classes que funcionam apenas como sacos de propriedades abertas (getters/setters públicos) sem comportamento.
> 
> ---
> 
> ## 2. Critérios de Aceitação do Leitor (Testes BDD)
> 
> Para o capítulo ser considerado aprovado editorialmente, o leitor que concluir o texto e os exercícios deve passar nos seguintes cenários:
> 

<!-- FONTE: F020 FIM -->

<a id="fonte-f021"></a>

#### F021 — Exemplo de spec editorial: critérios Gherkin

Origem histórica: conversa original, linhas 374–391. Cópia relacionada para este assunto. Destino principal: [anexo 15](15-texto-anexo.md#fonte-f021).

<!-- FONTE: F021 INICIO -->
~~~~text
```gherkin
Cenário: Identificação de Modelo Anêmico
  Dado um trecho de código onde uma classe Pedido possui propriedades públicas mutáveis
  E a validação de limite de desconto está dispersa dentro de um Controller ou Service
  Quando o leitor inspecionar a implementação
  Então ele deve apontar a falha de encapsulamento e explicar o risco de corrupção de estado.

Cenário: Refatoração para Entidade Rica com Invariante
  Dado o requisito de que "um item fiscal nunca pode ter quantidade negativa ou alíquota superior a 100%"
  Quando o leitor implementar o objeto ItemVenda
  Então a instanciação ou modificação com valores inválidos deve lançar uma exceção de domínio no construtor
  E o objeto não deve expor nenhum método setter público para esses campos.

Cenário: Criação de Teste de Comportamento em Memória
  Dado a entidade ItemVenda refatorada
  Quando o leitor escrever um teste unitário para validar o cálculo do total tributado
  Então o teste deve rodar sem nenhuma dependência de infraestrutura externa
  E o tempo de execução deve ser inferior a 15ms.

~~~~
<!-- FONTE: F021 FIM -->
