# Documento Base — CAP-08: Modularidade e dependências

**ID:** CAP-08  
**Parte:** IV — Modularidade e Arquitetura de Software  
**Estado:** Planejado — aguardando conclusão de CAP-03 e CAP-06  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Qual é o critério matemático e formal correto para fatiar um sistema em módulos para que uma mudança solicitada pela IA não quebre o restante da aplicação?
* **Objetivo de estudo:** Compreender a Teoria Formal da Modularidade (David Parnas, W. P. Stevens), diferenciando tipos de acoplamento e coesão, aplicando os princípios SOLID sob a ótica de controle de dependências e estabilidade arquitetural.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes têm a tendência natural de agrupar código por similaridade superficial (ex.: juntar tudo que lida com texto no mesmo arquivo) ou de injetar dependências cruzadas e cíclicas entre classes para resolver rapidamente um erro de compilação imediato.
* **Decisões sob responsabilidade do engenheiro:**
  * Aplicar *Information Hiding*: ocultar atrás de uma interface exatamente as decisões de design voláteis (ex.: a tabela de alíquotas fiscais, o driver de banco de dados ou a API de pagamento).
  * Impor direção estrita nas dependências (módulos estáveis não devem depender de módulos voláteis).
  * Validar a aplicação do Princípio da Substituição de Liskov (LSP) para garantir que subtipos gerados por IA preservem o contrato esperado pelos chamadores.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-03: Contratos e leitura diagnóstica](../03-contratos-e-leitura-diagnostica/documento-base.md) e [CAP-06: Linguagem e fronteiras de domínio](../06-linguagem-e-fronteiras-de-dominio/documento-base.md).
* **Tópicos essenciais:**
  * O Princípio de David Parnas (1972) — *On the Criteria To Be Used in Decomposing Systems into Modules* (*Information Hiding*).
  * O espectro de Acoplamento (Conteúdo, Comum, Controle, Dados) e Coesão (Coincidente, Temporal, Comunicacional, Funcional) de Stevens, Myers e Constantine.
  * SOLID como métricas de engenharia e controle de dependências (SRP, OCP, LSP, ISP, DIP).
  * Inversão de Controle (IoC) e Injeção de Dependências aplicadas a fronteiras desacopladas.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Análise de um módulo com alto acoplamento e refatoração dirigida por agente isolando uma decisão propensa a mudanças atrás de uma abstração de contrato estável.
* **Evidência esperada:** Demonstração comparativa antes/depois documentando a eliminação de dependências cruzadas e a proteção dos clientes contra alterações internas no módulo.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 1 (Contratos e Assinaturas)* e *Filtro 2 (Efeitos Colaterais)*.
* **Pergunta de auditoria rápida:** "Este módulo expõe sua estrutura interna ou esconde a implementação volátil atrás de um contrato? Se eu trocar a tecnologia de persistência ou o serviço externo, quantos arquivos gerados precisarão ser alterados?"

---

## 6. Fontes Primárias de Referência

1. **On the Criteria To Be Used in Decomposing Systems into Modules** (Communications of the ACM, 1972) — David L. Parnas.
2. **Structured Design** (IBM Systems Journal, 1974) — W. P. Stevens, G. J. Myers, L. L. Constantine.
3. **Agile Software Development: Principles, Patterns, and Practices** — Robert C. Martin (seções sobre os princípios SOLID e Princípios de Pacotes).

