# Última revisão da estrutura — transcrição literal

[Estrutura consolidada](ESTRUTURA_E_ESTUDO.md) · [Índice do livro](README.md)

Origem: `pensamentos.md`, linhas 1219–1371. O trecho contém o pedido final de aprofundamento em Engenharia de Software e a resposta com os cinco pilares adicionais e a sequência revisada de sete fases.

A transcrição preserva as palavras, exemplos e afirmações da conversa. Alegações técnicas ou promessas presentes nela continuam como material a avaliar; a organização para estudo está no documento de estrutura consolidada.

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
> Fase 1: Fundamentos de Computação e Runtime
> A base da ciência da computação conectada ao chão de fábrica.
> 
> Engenharia de Software: O papel do runtime, gerenciamento de memória (Stack vs. Heap, Garbage Collection e ciclos de coleta), latência de I/O em ordens de magnitude.
> 
> Sistemas Operacionais: Processos, Threads, Concorrência preemptiva, descritores de arquivo e portas TCP/UDP.
> 
> Aplicação com IA: Diagnosticar se o código gerado pelo agente respeita os limites físicos de memória e concorrência do ambiente de execução.
> 
> Fase 2: Garantia da Qualidade (SQA), Métricas Estáticas e Auditoria
> A ciência da medição de código sem necessidade de leitura linha por linha.
> 
> Engenharia de Software: Análise Estática de Código (SAST), Complexidade Ciclomática (McCabe), Métricas de Acoplamento Aferente e Eferente, e Leis de Halstead.
> 
> Os 5 Filtros Enriquecidos: Auditoria visual de assinaturas, rastreamento de efeitos colaterais de I/O, verificação de invariantes, asserções de teste e profiling.
> 
> Aplicação com IA: Configurar linters e analisadores estáticos que barram automaticamente qualquer entrega de IA com complexidade ciclomática ou acoplamento excessivo.
> 
> Fase 3: Engenharia de Requisitos, Atributos de Qualidade e SDD
> Como transformar problemas ambíguos de negócio em especificações determinísticas.
> 
> Engenharia de Software: Elicitação e especificação de requisitos, Requisitos Não-Funcionais (NFRs), Cenários de Atributos de Qualidade e Matrizes de Rastreabilidade.
> 
> Domain-Driven Design Estratégico: Linguagem Ubíqua, Bounded Contexts, Context Mapping e a erradicação de Modelos Anêmicos.
> 
> Aplicação com IA: Elaboração de Especificações Técnicas (SDD) com escopos negativos (Non-Goals) explícitos e contratos formais que impedem alucinações de escopo.
> 
> Fase 4: Teoria Formal da Modularidade e Arquitetura de Software
> A matemática do baixo acoplamento e da alta coesão.
> 
> Engenharia de Software: O princípio de Information Hiding de David Parnas; os 7 níveis de coesão e acoplamento; princípios SOLID fundamentados em álgebra de tipos e teoria de contratos; Lei de Conway.
> 
> Estilos Arquiteturais: Arquitetura em Camadas, Hexagonal (Ports & Adapters) e Clean Architecture; Monolito Modular vs. Serviços Distribuídos.
> 
> Aplicação com IA: Instruir a IA a estruturar o projeto de forma que os adaptadores externos (bancos, telas, APIs de terceiros) sejam plugáveis e substituíveis sem impactar o núcleo de regras.
> 
> Fase 5: Verificação, Validação (V&V) e Redes de Contenção
> A distinção clássica: "Estamos construindo o produto certo?" (Validação) vs. "Estamos construindo o produto do jeito certo?" (Verificação).
> 
> Engenharia de Software: Pirâmide e Troféu de Testes; BDD (Behavior-Driven Development) como especificação executável; Property-Based Testing e Invariantes Matemáticas; Testes de Mutação para auditoria da suíte de testes.
> 
> Engenharia de Contratos: Design by Contract (Pré-condições, Pós-condições, Invariantes).
> 
> Aplicação com IA: Gerar testes comportamentais antes da implementação do código e utilizar testes de mutação para expor testes tautológicos gerados pela IA.
> 
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
> O Que Essa Mudança Agrega ao seu Livro
> Com essa estrutura, a sua obra deixa de ser apenas "um guia prático de prompts e arquitetura" e se torna um Tratado de Engenharia de Software Moderna.
> 
> O livro responderá a uma das maiores perguntas da década: “Como os 50 anos de teoria da Engenharia de Software (Parnas, McCabe, Beck, Fowler, Lehman) se aplicam quando o código é gerado por inteligência artificial?”
> 
> Quer escolher uma dessas disciplinas formais (por exemplo, Métricas de McCabe ou Information Hiding de Parnas) para detalharmos como exemplo prático no seu projeto?