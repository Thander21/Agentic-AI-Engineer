# 09. Texto anexo — Agentes sob comando

[Etapa da jornada](09-agentes-sob-comando.md) · [Índice](README.md) · [Mapa de origem](MAPA_ORIGEM.md)

Este anexo reúne 10 trechos: 4 principais e 6 cópias relacionadas. A organização abaixo identifica o que a conversa já oferece e o que ainda precisa ser aprofundado.

As sínteses são uma leitura editorial do material. Os blocos identificados como fonte preservam literalmente perguntas, respostas, exemplos e versões anteriores; sugestões da outra IA não passam a ser decisões aprovadas ou resultados comprovados por estarem neste anexo.

## Mapa de aprofundamento

| Assunto | O que já temos | O que aprofundar |
| --- | --- | --- |
| [Responsabilidade de quem conduz](#assunto-01) | O pedido original coloca o profissional como responsável por orientar, responder, direcionar e decidir. | Definir responsabilidades humanas e critérios para delegar tarefas aos agentes. |
| [Especificação, requisitos e domínio](#assunto-02) | Os módulos propõem contratos, limites de escopo, invariantes e requisitos de qualidade; o exemplo de fatura fornece uma primeira spec. | Criar um processo de especificação que explicite intenção, restrições, alternativas e critérios de aceitação. |
| [Contexto, avaliações e governança](#assunto-03) | O material menciona contexto de projeto, avaliações de agentes e rastreabilidade. | Detalhar o ciclo real de instrução, execução, supervisão e correção, ainda pouco desenvolvido na conversa. |
| [Aceitação de entregas e evolução](#assunto-04) | Há propostas de quality gates, filtros de auditoria, integração contínua e compatibilidade. | Ligar especificação, implementação, verificação e manutenção; estabelecer quando revisar ou rejeitar uma entrega. |

## Texto de referência por assunto

<a id="assunto-01"></a>

### 1. Responsabilidade de quem conduz

**O que já temos:** O pedido original coloca o profissional como responsável por orientar, responder, direcionar e decidir.

**Para aprofundar:** Definir responsabilidades humanas e critérios para delegar tarefas aos agentes.

<a id="fonte-f024"></a>

#### F024 — Pedido de uma grade para orquestrar e decidir

Origem histórica: `pensamentos.md`, linhas 437–438. Cópia relacionada para este assunto. Destino principal: [anexo 03](03-texto-anexo.md#fonte-f024).

<!-- FONTE: F024 INICIO -->
> Com base no que discutimos e os para mtos levantados análise a grade curricular de um curso de engenharia de software e monte a nossa grade prática retira tópicos de programação já que nessa área o código é gerado pela ia o engeniro tem que entender como orquestrar, responder, direcionar e tomar todas as decisões
> 

<!-- FONTE: F024 FIM -->

<a id="fonte-f032"></a>

#### F032 — Comparação de papéis e competências pretendidas

Origem histórica: `pensamentos.md`, linhas 540–549. Cópia relacionada para este assunto. Destino principal: [anexo 03](03-texto-anexo.md#fonte-f032).

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

### 2. Especificação, requisitos e domínio

**O que já temos:** Os módulos propõem contratos, limites de escopo, invariantes e requisitos de qualidade; o exemplo de fatura fornece uma primeira spec.

**Para aprofundar:** Criar um processo de especificação que explicite intenção, restrições, alternativas e critérios de aceitação.

<a id="fonte-f027"></a>

#### F027 — Especificação e modelagem no trabalho com agentes

Origem histórica: `pensamentos.md`, linhas 467–477. Trecho principal desta etapa.

<!-- FONTE: F027 INICIO -->
> Módulo 1: Engenharia de Especificação e Modelagem de Domínio (SDD)
> Objetivo: Tornar a intenção do negócio semanticamente inequívoca para que modelos de IA executem sem alucinações de regra.
> 
> Spec-Driven Development (SDD): Redação de especificações técnicas formais com restrições explícitas, pré-condições, pós-condições e declaração de escopos excluídos (non-goals).
> 
> Domain-Driven Design Estratégico: Delimitação de Bounded Contexts, mapas de contexto (Context Mapping) e linguagem ubíqua.
> 
> Design por Contrato e Invariantes: Definição de regras imutáveis que o sistema não pode violar em nenhum cenário, impedindo geração de estados inválidos.
> 
> Modelagem Semântica de Tipos: Tipagem forte como ferramenta de design de restrição (uso de Value Objects para impedir primitivos soltos).
> 

<!-- FONTE: F027 FIM -->

<a id="fonte-f069"></a>

#### F069 — Primeira sequência: especificação e domínio

Origem histórica: `pensamentos.md`, linhas 1129–1143. Trecho principal desta etapa.

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

<a id="fonte-f081"></a>

#### F081 — Sequência revisada: requisitos e SDD

Origem histórica: `pensamentos.md`, linhas 1321–1329. Trecho principal desta etapa.

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

<a id="fonte-f045"></a>

#### F045 — Exemplo didático: especificação e cenário de fatura

Origem histórica: `pensamentos.md`, linhas 748–760. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f045).

<!-- FONTE: F045 INICIO -->
> Sim
> Sim
> 
> Vamos ver isso na prática com um cenário realista de negócio: emissão de fatura com cálculo tributário e desconto.
> 
> Imagine que você especificou para a IA (via SDD):
> 
> "Criar o serviço de emissão de fatura. Regras: (1) Desconto acima de 15% exige aprovação de gerente; (2) Calcular o imposto de cada item; (3) Gravar a fatura no banco de dados; (4) Notificar o serviço fiscal governamental por API externa."
> 
> A IA gerou o código abaixo, avisou que "o código foi implementado com sucesso e 100% dos testes passaram".
> 
> O Código Gerado pela IA (Parece perfeito à primeira vista)
> C#

<!-- FONTE: F045 FIM -->

<a id="assunto-03"></a>

### 3. Contexto, avaliações e governança

**O que já temos:** O material menciona contexto de projeto, avaliações de agentes e rastreabilidade.

**Para aprofundar:** Detalhar o ciclo real de instrução, execução, supervisão e correção, ainda pouco desenvolvido na conversa.

<a id="fonte-f031"></a>

#### F031 — Orquestração e governança de agentes

Origem histórica: `pensamentos.md`, linhas 531–539. Trecho principal desta etapa.

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

<a id="assunto-04"></a>

### 4. Aceitação de entregas e evolução

**O que já temos:** Há propostas de quality gates, filtros de auditoria, integração contínua e compatibilidade.

**Para aprofundar:** Ligar especificação, implementação, verificação e manutenção; estabelecer quando revisar ou rejeitar uma entrega.

<a id="fonte-f029"></a>

#### F029 — Qualidade, testes e revisão de código gerado

Origem histórica: `pensamentos.md`, linhas 500–510. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f029).

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

Origem histórica: `pensamentos.md`, linhas 939–975. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f057).

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

<a id="fonte-f077"></a>

#### F077 — Evolução, dívida técnica, configuração e XP

Origem histórica: `pensamentos.md`, linhas 1269–1286. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f077).

<!-- FONTE: F077 INICIO -->
> 4. Manutenção, Evolução de Software e Dívida Técnica
> O desenvolvimento não termina no deploy; 70% a 80% do custo total de propriedade (TCO) de um software ocorre na sua manutenção.
> 
> Leis da Evolução de Software de Lehman: Leis empíricas clássicas, como a Mudança Contínua (um sistema que é usado precisa se adaptar ou se torna inútil) e a Complexidade Crescente (à medida que evolui, a complexidade aumenta a menos que haja trabalho explícito para reduzi-la).
> 
> Taxonomia da Dívida Técnica (Ward Cunningham / Martin Fowler): Diferenciar dívida prudente vs. imprudente, deliberada vs. inadvertida, e estabelecer planos de quitação contínua.
> 
> Padrões de Refatoração Contínua e Estrangulamento (Strangler Fig Pattern): A engenharia por trás de migrar sistemas legados sem paralisação do negócio.
> 
> 5. Gestão de Configuração e Práticas de Extreme Programming (XP)
> A disciplina que garante que equipes (humanas ou agentes de IA) trabalhem sem colisão:
> 
> Versionamento Semântico Formal (SemVer 2.0): Impacto de quebras de contrato (Major), adições retrocompatíveis (Minor) e patches.
> 
> Padrão Expand and Contract (Parallel Run): Como alterar esquemas de banco de dados e contratos de API em produção com zero downtime.
> 
> Práticas Centrais de XP na Era da IA: Integração Contínua (CI), Releases Pequenos e Frequentes, Design Simples (as 4 regras de Kent Beck) e Pareamento (agora Engenheiro-IA).
> 

<!-- FONTE: F077 FIM -->

