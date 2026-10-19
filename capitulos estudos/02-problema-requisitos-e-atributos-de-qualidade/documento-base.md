# Documento Base — CAP-02: Problema, requisitos e atributos de qualidade

**ID:** CAP-02  
**Parte:** II — Especificação e Domínio  
**Estado:** Planejado — aguardando conclusão de CAP-01  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como transformar uma necessidade de negÃ³cio em uma especificaÃ§Ã£o tÃ©cnica inequÃ­voca, com critÃ©rios de aceitaÃ§Ã£o e atributos de qualidade mensurÃ¡veis, para que os agentes de IA implementem exatamente o que o problema exige?
* **Objetivo de estudo:** Dominar as tÃ©cnicas fundamentais de Engenharia de Requisitos, diferenciando requisitos funcionais de requisitos nÃ£o-funcionais (Atributos de Qualidade ou "Ilities"), formulando CenÃ¡rios de Atributos de Qualidade rigorosos com estÃ­mulo e resposta mensurÃ¡veis.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes nÃ£o sabem o que o cliente realmente precisa; eles respondem a comandos literais. Quando a especificaÃ§Ã£o diz apenas "o sistema deve ser rÃ¡pido e seguro", o agente inventa comportamentos ou assume premissas arbitrÃ¡rias. Requisitos ambÃ­guos geram cÃ³digo desnecessÃ¡rio ou perigoso.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Delimitar o escopo inegociÃ¡vel (o que estÃ¡ dentro e o que estÃ¡ expressamente fora do problema).
  * Formular restriÃ§Ãµes arquiteturais e mÃ©tricas claras (ex.: latÃªncia mÃ¡xima, throughput, auditabilidade).
  * Traduzir regras de negÃ³cio em critÃ©rios de aceitaÃ§Ã£o binÃ¡rios (passa / nÃ£o passa).

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-03: Contratos e leitura diagnÃ³stica](../03-contratos-e-leitura-diagnostica/documento-base.md).
* **TÃ³picos essenciais:**
  * ElicitaÃ§Ã£o e especificaÃ§Ã£o de requisitos de software (IEEE 830 / ISO/IEC/IEEE 29148).
  * Requisitos NÃ£o-Funcionais (NFRs) e Atributos de Qualidade: Manutenibilidade, Disponibilidade, Escalabilidade, Testabilidade, Auditabilidade e SeguranÃ§a.
  * CenÃ¡rios de Atributos de Qualidade (SEI/Bass-Clements-Kazman): Fonte do estÃ­mulo, EstÃ­mulo, Artefato afetado, Ambiente, Resposta e Medida da resposta.
  * CritÃ©rios de aceitaÃ§Ã£o e definiÃ§Ã£o de pronto (*Definition of Done*).

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** ElaboraÃ§Ã£o de uma especificaÃ§Ã£o formal de requisitos para um mÃ³dulo de cÃ¡lculo de faturas ou motor de regras com restriÃ§Ã£o de desempenho sob carga.
* **EvidÃªncia esperada:** Uma especificaÃ§Ã£o enxuta contendo casos de uso delimitados e pelo menos 2 cenÃ¡rios completos de atributos de qualidade mensurÃ¡veis com critÃ©rios de verificaÃ§Ã£o automatizÃ¡veis.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtro em destaque:** *Filtro 1 (Contrato e Assinatura)* e *Filtro 3 (Invariantes por HipÃ³tese)*.
* **Pergunta de auditoria rÃ¡pida:** "O cÃ³digo e a arquitetura entregues pelo agente respeitam os limiares de resposta mensurados estipulados no cenÃ¡rio de qualidade?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Software Architecture in Practice** â€” Len Bass, Paul Clements e Rick Kazman (capÃ­tulos sobre Quality Attributes e Quality Attribute Scenarios).
2. **SWEBOK v3/v4** â€” IEEE Computer Society (capÃ­tulo sobre Software Requirements).
3. **Writing Effective Use Cases** â€” Alistair Cockburn (estruturaÃ§Ã£o de metas e prÃ©/pÃ³s-condiÃ§Ãµes).

