# Documento Base — CAP-09: Escolhas arquiteturais

**ID:** CAP-09  
**Parte:** IV — Modularidade e Arquitetura  
**Estado:** Planejado — aguardando conclusão de CAP-02 e CAP-08  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Quando devemos optar por um monolito modular, uma arquitetura hexagonal (portas e adaptadores) ou microsserviÃ§os distribuÃ­dos, e como a Lei de Conway e os custos de infraestrutura condicionam essa decisÃ£o no desenvolvimento com agentes?
* **Objetivo de estudo:** Comparar formalmente os estilos arquiteturais mais influentes (em camadas, Hexagonal/Ports & Adapters, Clean Architecture, Monolito Modular e MicrosserviÃ§os), avaliando seus trade-offs, limites de complexidade operacional e o impacto da Lei de Conway na organizaÃ§Ã£o de projetos e times.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes tendem a recomendar padrÃµes populares ou excessivamente fragmentados (como dezenas de microsserviÃ§os para um problema trivial) sem avaliar os custos de latÃªncia de rede, consistÃªncia eventual, custos de nuvem ou complexidade de manutenÃ§Ã£o.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Escolher o estilo arquitetural adequado Ã  escala real e Ã  taxa de mudanÃ§as do sistema.
  * Preservar a integridade das camadas (ex.: impedir que regras de negÃ³cio dependam diretamente de frameworks web ou bibliotecas de persistÃªncia).
  * Justificar as decisÃµes arquiteturais com base em trade-offs econÃ´micos e operacionais (ADRs â€” *Architecture Decision Records*).

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-05: Problema, requisitos e atributos de qualidade](../05-problema-requisitos-e-atributos-de-qualidade/documento-base.md) e [CAP-08: Modularidade e dependÃªncias](../08-modularidade-e-dependencias/documento-base.md).
* **TÃ³picos essenciais:**
  * Arquitetura em Camadas clÃ¡ssica vs. InversÃ£o de DependÃªncias.
  * Arquitetura Hexagonal (*Ports & Adapters* - Alistair Cockburn) e *Clean Architecture* (Robert Martin): isolamento do nÃºcleo de negÃ³cio contra detalhes de entrega e persistÃªncia.
  * Monolito Modular vs. ServiÃ§os DistribuÃ­dos (MicrosserviÃ§os): custos de rede, governanÃ§a e complexidade acidental.
  * Lei de Conway: como a estrutura de comunicaÃ§Ã£o e as fronteiras organizacionais moldam as interfaces dos sistemas.
  * Registros de DecisÃ£o Arquitetural (ADRs).

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** ElaboraÃ§Ã£o de uma ADR e diagrama arquitetural formal para uma aplicaÃ§Ã£o com requisitos de desacoplamento, comparando uma abordagem hexagonal com um modelo monolÃ­tico modular.
* **EvidÃªncia esperada:** Registro de DecisÃ£o Arquitetural documentado com contexto, alternativas consideradas, forÃ§as e restriÃ§Ãµes, decisÃ£o tomada e consequÃªncias para os prompts e regras de geraÃ§Ã£o do agente.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 1 (Contratos)* e *Filtro 2 (Efeitos Colaterais)*.
* **Pergunta de auditoria rÃ¡pida:** "A camada de domÃ­nio puro importa bibliotecas de terceiros, pacotes de banco de dados ou frameworks de tela? As portas de entrada e saÃ­da estÃ£o explicitamente separadas dos adaptadores de infraestrutura?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Hexagonal Architecture (Ports and Adapters)** â€” Alistair Cockburn ([alistair.cockburn.us/hexagonal-architecture](https://alistair.cockburn.us/hexagonal-architecture/)).
2. **Clean Architecture: A Craftsman's Guide to Software Structure and Design** â€” Robert C. Martin.
3. **Monolith to Microservices** â€” Sam Newman (capÃ­tulos de trade-offs de distribuiÃ§Ã£o).
4. **How Do Committees Invent? (Conway's Law, 1968)** â€” Melvin E. Conway.

