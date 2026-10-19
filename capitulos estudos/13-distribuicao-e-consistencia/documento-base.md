# Documento Base — CAP-13: Distribuição e consistência

**ID:** CAP-13  
**Parte:** VI — Dados, Concorrência e Distribuição  
**Estado:** Planejado — aguardando conclusão de CAP-09 e CAP-12  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Quando dividimos um sistema em múltiplos nós ou serviços, o que acontece durante falhas parciais de rede, e por que não é possível ter consistência imediata e disponibilidade total simultaneamente?
* **Objetivo de estudo:** Analisar formalmente os teoremas fundamentais de sistemas distribuídos (Teorema CAP e modelo PACELC), modelos de consistência (Linearizabilidade vs. Consistência Eventual) e coordenação distribuída (Two-Phase Commit - 2PC vs. Padrão Saga).

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes pressupõem que a rede é rápida, confiável e infinita (as clássicas Falácias da Computação Distribuída). Ao projetar operações entre múltiplos serviços, a IA frequentemente cria transações distribuídas ingênuas que deixam o sistema travado caso um serviço terceiro fique lento ou indisponível.
* **Decisões sob responsabilidade do engenheiro:**
  * Escolher o trade-off entre consistência forte e alta disponibilidade sob partição de rede (CAP/PACELC).
  * Projetar fluxos de compensação no padrão Saga (orquestrado vs. coreografado) em vez de acoplar serviços com 2PC síncrono.
  * Delimitar as janelas de inconsistência toleráveis pelo negócio.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-09: Escolhas arquiteturais](../09-escolhas-arquiteturais/documento-base.md) e [CAP-12: Dados, transações e isolamento](../12-dados-transacoes-e-isolamento/documento-base.md).
* **Tópicos essenciais:**
  * As 8 Falácias da Computação Distribuída (Peter Deutsch).
  * Teorema CAP de Eric Brewer (Consistência, Disponibilidade, Tolerância a Partições) e extensão PACELC (Daniel Abadi).
  * Consistência Forte (Linearizabilidade) vs. Consistência Causal vs. Consistência Eventual.
  * Two-Phase Commit (2PC): o risco do bloqueio em caso de falha do coordenador.
  * Padrão Saga: transações locais, eventos e ações compensatórias.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Projeto de um fluxo de reserva/pagamento distribuído entre dois serviços independentes sob simulação de queda de rede no meio da operação.
* **Evidência esperada:** Comparação formal entre uma tentativa de commit de duas fases (2PC) e um fluxo Saga com transações compensatórias, demonstrando a recuperação do estado consistente após a falha.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 2 (Efeitos Colaterais / Rede)* e *Filtro 3 (Invariantes)*.
* **Pergunta de auditoria rápida:** "O que acontece se a chamada HTTP externa nesta etapa falhar com timeout? Existe uma ação de compensação ou o sistema deixa dados órfãos e inconsistentes no banco?"

---

## 6. Fontes Primárias de Referência

1. **Designing Data-Intensive Applications (DDIA)** — Martin Kleppmann (Capítulos 8 e 9: Problemas com Sistemas Distribuídos e Consistência/Consenso).
2. **Consistency Tradeoffs in Modern Distributed Database System Design (PACELC)** — Daniel J. Abadi.
3. **Sagas** (ACM SIGMOD, 1987) — Hector Garcia-Molina e Kenneth Salem.

