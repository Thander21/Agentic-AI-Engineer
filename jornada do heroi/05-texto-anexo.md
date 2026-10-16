# 05. Texto anexo — Mestres, fontes e boas perguntas

[Etapa da jornada](05-mestres-fontes-e-boas-perguntas.md) · [Índice](README.md) · [Mapa de origem](MAPA_ORIGEM.md)

Este anexo reúne 9 trechos: 6 principais e 3 cópias relacionadas. A organização abaixo identifica o que a conversa já oferece e o que ainda precisa ser aprofundado.

As sínteses são uma leitura editorial do material. Os blocos identificados como fonte preservam literalmente perguntas, respostas, exemplos e versões anteriores; sugestões da outra IA não passam a ser decisões aprovadas ou resultados comprovados por estarem neste anexo.

## Mapa de aprofundamento

| Assunto | O que já temos | O que aprofundar |
| --- | --- | --- |
| [Busca de formação estruturada e alegações sobre cursos](#assunto-01) | A conversa procura uma alternativa sequencial de estudo e recebe comparações amplas com universidades e bootcamps. | Verificar as comparações antes de usá-las como argumento editorial e selecionar fontes pelo conhecimento que ajudam a adquirir. |
| [Bibliografia e documentação já mencionadas](#assunto-02) | Foram citados livros de domínio, arquitetura, testes, dados e resiliência, além de documentação de padrões e observabilidade. | Conferir edições e capítulos e relacionar cada leitura ao problema estudado. O inventário não constitui uma recomendação atualizada por pesquisa externa. |
| [Ampliação para fundamentos formais](#assunto-03) | A última revisão menciona SWEBOK, requisitos, modularidade, métricas e autores de Engenharia de Software. | Localizar as fontes primárias e justificar a profundidade de cada tema em função das decisões pretendidas. |
| [Afirmações que precisam de verificação](#assunto-04) | Há limites numéricos e promessas de resultados formulados de maneira categórica pela IA. | Registrar alegação, fonte, contexto e evidência necessária antes de incorporá-los à metodologia ou ao livro. |

## Texto de referência por assunto

<a id="assunto-01"></a>

### 1. Busca de formação estruturada e alegações sobre cursos

**O que já temos:** A conversa procura uma alternativa sequencial de estudo e recebe comparações amplas com universidades e bootcamps.

**Para aprofundar:** Verificar as comparações antes de usá-las como argumento editorial e selecionar fontes pelo conhecimento que ajudam a adquirir.

<a id="fonte-f005"></a>

#### F005 — Busca de formação estruturada e comparação com cursos

Origem histórica: conversa original, linhas 137–147. Trecho principal desta etapa.

<!-- FONTE: F005 INICIO -->
> Sim
> Gostei se fosse fazer um engenheiro de software atual aprenderia esses pontos? Se não onde aprender de forma estruturada e sequêncial?
> 
> Uma graduação tradicional em Engenharia de Software ou Ciência da Computação não ensina a maioria desses pontos no nível exigido pelo mercado atual.
> 
> A academia é focada em fundamentos atemporais: algoritmos, estruturas de dados, cálculo, teoria dos compiladores, redes e álgebra relacional. O que acontece em produção — como modelagem de domínio rica, reconciliação de dados offline-first, resiliência distribuída e observabilidade — quase nunca entra na ementa universitária.
> 
> Já os cursos rápidos (bootcamps) vão para o extremo oposto: ensinam sintaxe de frameworks modernos e CRUDs rápidos, ignorando completamente arquitetura, concorrência e rigor de testes.
> 
> O conhecimento de um engenheiro sênior/arquiteto compõe o chamado currículo oculto da indústria. Para absorvê-lo de forma metódica, sem se perder em tutoriais fragmentados, siga uma trilha sequencial dividida em quatro fases estruturadas.
> 

<!-- FONTE: F005 FIM -->

<a id="fonte-f025"></a>

#### F025 — Afirmações sobre formação tradicional a examinar

Origem histórica: conversa original, linhas 439–453. Trecho principal desta etapa.

<!-- FONTE: F025 INICIO -->
> A grade tradicional de Engenharia de Software foi desenhada para uma era em que 80% do tempo de um profissional era gasto digitando sintaxe, depurando ponteiros e implementando manualmente algoritmos já resolvidos pela ciência da computação.
> 
> Na era da inteligência artificial, a sintaxe virou commodity. O gargalo da engenharia migrou para a formulação de problemas, definição de fronteiras arquiteturais, garantia de invariantes de negócio e validação determinística de soluções geradas por agentes.
> 
> Abaixo está o diagnóstico do que precisa ser descartado do modelo universitário convencional e a estrutura da Grade Prática do Engenheiro Orquestrador e Decisor.
> 
> Diagnóstico: O que é eliminado da grade tradicional
> Eliminado: Programação Básica e Avançada (Linguagem A, B ou C): Ensinar loops, sintaxe de ponteiros, alocação manual e estruturas de repetição isoladas é obsoleto como disciplina autônoma; o agente gera a implementação correta em segundos se a restrição for clara.
> 
> Eliminado: Implementação Manual de Algoritmos Clássicos: Escrever árvores binárias balanceadas, QuickSort ou listas encadeadas do zero. O engenheiro precisa saber a complexidade de tempo/espaço para tomar decisões de escala, não reescrever bibliotecas padrão.
> 
> Eliminado: Cálculo Puro e Física Teórica: Três semestres de integrais duplas e equações diferenciais sem ligação com software funcionam apenas como filtro de retenção acadêmico.
> 
> Eliminado: Engenharia de Requisitos Burocrática (UML Tradicional / RUP): Diagramas extensos de caso de uso e documentação estática em Word que nascem desatualizados.
> 

<!-- FONTE: F025 FIM -->

<a id="assunto-02"></a>

### 2. Bibliografia e documentação já mencionadas

**O que já temos:** Foram citados livros de domínio, arquitetura, testes, dados e resiliência, além de documentação de padrões e observabilidade.

**Para aprofundar:** Conferir edições e capítulos e relacionar cada leitura ao problema estudado. O inventário não constitui uma recomendação atualizada por pesquisa externa.

<a id="fonte-f007"></a>

#### F007 — Fontes de domínio e arquitetura

Origem histórica: conversa original, linhas 159–166. Trecho principal desta etapa.

<!-- FONTE: F007 INICIO -->
> Fontes estruturadas de estudo:
> 
> Livro: Domain-Driven Design Distilled — Vaughn Vernon. (Leitura curta, muito mais direta e prática do que o livro clássico original de Eric Evans).
> 
> Livro: Clean Architecture — Robert C. Martin. (Foque nos princípios de desacoplamento e inversão de dependência).
> 
> Referência online: O portal e os artigos de Martin Fowler (martinfowler.com), em especial os guias sobre Anemic Domain Model e Bounded Context.
> 

<!-- FONTE: F007 FIM -->

<a id="fonte-f009"></a>

#### F009 — Fontes de testes

Origem histórica: conversa original, linhas 178–183. Trecho principal desta etapa.

<!-- FONTE: F009 INICIO -->
> Fontes estruturadas de estudo:
> 
> Livro: Unit Testing Principles, Practices, and Patterns — Vladimir Khorikov. (A melhor referência moderna sobre o tema; ensina a diferença entre testar estado vs. comportamento e como evitar testes frágeis).
> 
> Livro: Growing Object-Oriented Software, Guided by Tests (GOOS) — Steve Freeman e Nat Pryce. (O clássico que ensina a projetar arquitetura guiada por testes de ponta a ponta).
> 

<!-- FONTE: F009 FIM -->

<a id="fonte-f011"></a>

#### F011 — Fontes de dados e local-first

Origem histórica: conversa original, linhas 195–200. Trecho principal desta etapa.

<!-- FONTE: F011 INICIO -->
> Fontes estruturadas de estudo:
> 
> Livro: Designing Data-Intensive Applications (DDIA) — Martin Kleppmann. (Considerada a bíblia da engenharia de software moderna. Leia prioritariamente os capítulos sobre transações, concorrência, replicação e consistência).
> 
> Referência online: Comunidade e manifestos em localfirstweb.dev (para entender as técnicas contemporâneas de sincronização local com nuvem, CRDTs e resolução de conflitos).
> 

<!-- FONTE: F011 FIM -->

<a id="fonte-f013"></a>

#### F013 — Fontes de resiliência e observabilidade

Origem histórica: conversa original, linhas 212–219. Trecho principal desta etapa.

<!-- FONTE: F013 INICIO -->
> Fontes estruturadas de estudo:
> 
> Livro: Release It! Design and Deploy Production-Ready Software — Michael T. Nygard. (O guia definitivo sobre padrões de resiliência e como sistemas quebram em produção).
> 
> Documentação de Padrões: Azure Architecture Center: Cloud Design Patterns ou AWS Well-Architected Framework (ambos são gratuitos, agnósticos de provedor na maior parte dos conceitos e cobrem padrões clássicos de resiliência e escalabilidade).
> 
> Documentação oficial: opentelemetry.io/docs/concepts (para entender o padrão global da indústria sobre telemetria).
> 

<!-- FONTE: F013 FIM -->

<a id="assunto-03"></a>

### 3. Ampliação para fundamentos formais

**O que já temos:** A última revisão menciona SWEBOK, requisitos, modularidade, métricas e autores de Engenharia de Software.

**Para aprofundar:** Localizar as fontes primárias e justificar a profundidade de cada tema em função das decisões pretendidas.

<a id="fonte-f075"></a>

#### F075 — Pedido de mais Engenharia de Software e fundamentos formais

Origem histórica: conversa original, linhas 1219–1252. Cópia relacionada para este assunto. Destino principal: [anexo 07](07-texto-anexo.md#fonte-f075).

<!-- FONTE: F075 INICIO -->
> Sim
> Vamos, é, melhorar as sete fases elaboradas, ficaram muito boas, mas eu sinto que faltou material da própria engenharia de software. É o que que a gente precisa incluir, ou que pontos adicionais, ou fases adicionais, ou dentro de cada fase, é, explorar melhor os conceitos de engenharia de software e a matéria da engenharia de software.
> 
> A lacuna na proposta anterior está exatamente onde a disciplina de Engenharia de Software (SE) se diferencia da mera programação com arquitetura: faltaram os fundamentos formais de Engenharia de Requisitos, Teoria da Modularidade, Métricas de Qualidade, Gestão de Mudança e Evolução (Leis de Lehman) e Economia do Software.
> 
> Sem essa bagagem conceitual formal (consolidada em referências como o SWEBOK — Software Engineering Body of Knowledge e nas obras clássicas de David Parnas, Kent Beck e Martin Fowler), o engenheiro orquestrador corre o risco de tomar decisões baseadas apenas em "gosto" ou intuição prática, sem conseguir provar e medir a qualidade da solução.
> 
> Abaixo está o mapeamento dos conceitos formais da Engenharia de Software que devem ser incorporados e a reestruturação aprofundada da jornada.
> 
> Os 5 Pilares Formais de Engenharia de Software que Faltavam
> 1. Engenharia de Requisitos e Atributos de Qualidade (NFRs)
> Na academia e na indústria séria, software não é apenas "regra funcional". O que define a arquitetura são os Requisitos Não-Funcionais (NFRs) ou Atributos de Qualidade:
> 
> As "Ilities": Manutenibilidade, Testabilidade, Auditabilidade, Disponibilidade, Escalabilidade, Portabilidade e Tolerância a Falhas.
> 
> Cenários de Atributo de Qualidade: Em vez de dizer "o sistema deve ser rápido", a Engenharia de Software ensina a formular estímulos mensuráveis: "Sob carga de 50 requisições/segundo (estímulo), o motor fiscal deve calcular o lote em menos de 800ms (resposta mensurada)".
> 
> Matriz de Rastreabilidade: A capacidade formal de conectar a necessidade do cliente 
> →
> → especificação 
> →
> → contrato de interface 
> →
> → teste de aceitação automatizado.
> 
> 2. Teoria Formal de Modularidade e Design (Parnas & Stevens)
> Antes de Clean Architecture ou Microsserviços existirem, a Engenharia de Software já havia definido matematicamente o que faz um sistema durar:
> 
> O Princípio de David Parnas (1972) — Information Hiding: O critério correto para fatiar um módulo não é agrupar funções parecidas, mas esconder uma decisão de design propensa a mudanças (ex.: a tabela de alíquotas fiscais ou o driver de impressão).
> 
> Espectro de Coesão e Acoplamento: Entender os tipos formais de acoplamento (de Conteúdo, Comum, de Controle, de Dados) e de coesão (Coincidente, Temporal, Comunicacional, Funcional).
> 
> SOLID como Métricas de Estabilidade: Compreender os princípios de Robert Martin não como dogmas, mas como técnicas de controle de acoplamento e preservação de contratos (especialmente o Princípio de Substituição de Liskov — LSP — que garante que subtipos não quebrem o comportamento esperado).
> 

<!-- FONTE: F075 FIM -->

<a id="assunto-04"></a>

### 4. Afirmações que precisam de verificação

**O que já temos:** Há limites numéricos e promessas de resultados formulados de maneira categórica pela IA.

**Para aprofundar:** Registrar alegação, fonte, contexto e evidência necessária antes de incorporá-los à metodologia ou ao livro.

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

<a id="fonte-f073"></a>

#### F073 — Resultados prometidos para o ciclo: a verificar

Origem histórica: conversa original, linhas 1215–1216. Cópia relacionada para este assunto. Destino principal: [anexo 11](11-texto-anexo.md#fonte-f073).

<!-- FONTE: F073 INICIO -->
> Ao final desse ciclo em 7 fases, você terá modernizado completamente o seu produto, adquirido senioridade arquitetural comprovada e concluído o manuscrito de um livro 100% ancorado na realidade da engenharia moderna.
> 

<!-- FONTE: F073 FIM -->
