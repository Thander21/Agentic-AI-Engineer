# Documento Base — CAP-09: Escolhas arquiteturais

**ID:** CAP-09  
**Parte:** IV — Modularidade e Arquitetura de Software  
**Estado:** Planejado — aguardando conclusão de CAP-05 e CAP-08  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Quando devemos optar por um monolito modular, uma arquitetura hexagonal (portas e adaptadores) ou microsserviços distribuídos, e como a Lei de Conway e os custos de infraestrutura condicionam essa decisão no desenvolvimento com agentes?
* **Objetivo de estudo:** Comparar formalmente os estilos arquiteturais mais influentes (em camadas, Hexagonal/Ports & Adapters, Clean Architecture, Monolito Modular e Microsserviços), avaliando seus trade-offs, limites de complexidade operacional e o impacto da Lei de Conway na organização de projetos e times.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes tendem a recomendar padrões populares ou excessivamente fragmentados (como dezenas de microsserviços para um problema trivial) sem avaliar os custos de latência de rede, consistência eventual, custos de nuvem ou complexidade de manutenção.
* **Decisões sob responsabilidade do engenheiro:**
  * Escolher o estilo arquitetural adequado à escala real e à taxa de mudanças do sistema.
  * Preservar a integridade das camadas (ex.: impedir que regras de negócio dependam diretamente de frameworks web ou bibliotecas de persistência).
  * Justificar as decisões arquiteturais com base em trade-offs econômicos e operacionais (ADRs — *Architecture Decision Records*).

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-05: Problema, requisitos e atributos de qualidade](../05-problema-requisitos-e-atributos-de-qualidade/documento-base.md) e [CAP-08: Modularidade e dependências](../08-modularidade-e-dependencias/documento-base.md).
* **Tópicos essenciais:**
  * Arquitetura em Camadas clássica vs. Inversão de Dependências.
  * Arquitetura Hexagonal (*Ports & Adapters* - Alistair Cockburn) e *Clean Architecture* (Robert Martin): isolamento do núcleo de negócio contra detalhes de entrega e persistência.
  * Monolito Modular vs. Serviços Distribuídos (Microsserviços): custos de rede, governança e complexidade acidental.
  * Lei de Conway: como a estrutura de comunicação e as fronteiras organizacionais moldam as interfaces dos sistemas.
  * Registros de Decisão Arquitetural (ADRs).

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Elaboração de uma ADR e diagrama arquitetural formal para uma aplicação com requisitos de desacoplamento, comparando uma abordagem hexagonal com um modelo monolítico modular.
* **Evidência esperada:** Registro de Decisão Arquitetural documentado com contexto, alternativas consideradas, forças e restrições, decisão tomada e consequências para os prompts e regras de geração do agente.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 1 (Contratos)* e *Filtro 2 (Efeitos Colaterais)*.
* **Pergunta de auditoria rápida:** "A camada de domínio puro importa bibliotecas de terceiros, pacotes de banco de dados ou frameworks de tela? As portas de entrada e saída estão explicitamente separadas dos adaptadores de infraestrutura?"

---

## 6. Fontes Primárias de Referência

1. **Hexagonal Architecture (Ports and Adapters)** — Alistair Cockburn ([alistair.cockburn.us/hexagonal-architecture](https://alistair.cockburn.us/hexagonal-architecture/)).
2. **Clean Architecture: A Craftsman's Guide to Software Structure and Design** — Robert C. Martin.
3. **Monolith to Microservices** — Sam Newman (capítulos de trade-offs de distribuição).
4. **How Do Committees Invent? (Conway's Law, 1968)** — Melvin E. Conway.

