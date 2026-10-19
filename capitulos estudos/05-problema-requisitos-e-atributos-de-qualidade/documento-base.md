# Documento Base — CAP-05: Problema, requisitos e atributos de qualidade

**ID:** CAP-05  
**Parte:** III — Requisitos, Atributos de Qualidade e SDD  
**Estado:** Planejado — aguardando conclusão de CAP-03  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como transformar uma necessidade de negócio em uma especificação técnica inequívoca, com critérios de aceitação e atributos de qualidade mensuráveis, para que os agentes de IA implementem exatamente o que o problema exige?
* **Objetivo de estudo:** Dominar as técnicas fundamentais de Engenharia de Requisitos, diferenciando requisitos funcionais de requisitos não-funcionais (Atributos de Qualidade ou "Ilities"), formulando Cenários de Atributos de Qualidade rigorosos com estímulo e resposta mensuráveis.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes não sabem o que o cliente realmente precisa; eles respondem a comandos literais. Quando a especificação diz apenas "o sistema deve ser rápido e seguro", o agente inventa comportamentos ou assume premissas arbitrárias. Requisitos ambíguos geram código desnecessário ou perigoso.
* **Decisões sob responsabilidade do engenheiro:**
  * Delimitar o escopo inegociável (o que está dentro e o que está expressamente fora do problema).
  * Formular restrições arquiteturais e métricas claras (ex.: latência máxima, throughput, auditabilidade).
  * Traduzir regras de negócio em critérios de aceitação binários (passa / não passa).

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-03: Contratos e leitura diagnóstica](../03-contratos-e-leitura-diagnostica/documento-base.md).
* **Tópicos essenciais:**
  * Elicitação e especificação de requisitos de software (IEEE 830 / ISO/IEC/IEEE 29148).
  * Requisitos Não-Funcionais (NFRs) e Atributos de Qualidade: Manutenibilidade, Disponibilidade, Escalabilidade, Testabilidade, Auditabilidade e Segurança.
  * Cenários de Atributos de Qualidade (SEI/Bass-Clements-Kazman): Fonte do estímulo, Estímulo, Artefato afetado, Ambiente, Resposta e Medida da resposta.
  * Critérios de aceitação e definição de pronto (*Definition of Done*).

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Elaboração de uma especificação formal de requisitos para um módulo de cálculo de faturas ou motor de regras com restrição de desempenho sob carga.
* **Evidência esperada:** Uma especificação enxuta contendo casos de uso delimitados e pelo menos 2 cenários completos de atributos de qualidade mensuráveis com critérios de verificação automatizáveis.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtro em destaque:** *Filtro 1 (Contrato e Assinatura)* e *Filtro 3 (Invariantes por Hipótese)*.
* **Pergunta de auditoria rápida:** "O código e a arquitetura entregues pelo agente respeitam os limiares de resposta mensurados estipulados no cenário de qualidade?"

---

## 6. Fontes Primárias de Referência

1. **Software Architecture in Practice** — Len Bass, Paul Clements e Rick Kazman (capítulos sobre Quality Attributes e Quality Attribute Scenarios).
2. **SWEBOK v3/v4** — IEEE Computer Society (capítulo sobre Software Requirements).
3. **Writing Effective Use Cases** — Alistair Cockburn (estruturação de metas e pré/pós-condições).

