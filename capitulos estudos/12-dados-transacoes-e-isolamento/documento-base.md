# Documento Base — CAP-12: Dados, transações e isolamento

**ID:** CAP-12  
**Parte:** VI — Dados, Concorrência e Distribuição  
**Estado:** Planejado — aguardando conclusão de CAP-02 e CAP-03  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** O que acontece quando dois usuários executam a mesma operação simultaneamente no banco de dados, e por que o código gerado pela IA é propenso a corromper saldos, criar deadlocks ou permitir leituras fantasmas?
* **Objetivo de estudo:** Compreender em profundidade as propriedades ACID, os níveis formais de isolamento de transações (Read Uncommitted, Read Committed, Repeatable Read, Serializable), anomalias de concorrência e estratégias de bloqueio (travamento pessimista vs. otimista).

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** IAs quase invariavelmente escrevem consultas sem pensar em concorrência (ex.: fazer um `SELECT saldo FROM conta`, calcular o novo saldo em memória na aplicação e depois rodar um `UPDATE conta SET saldo = novo_saldo`). Sob concorrência real, isso gera a clássica perda de atualização (*Lost Update*), causando prejuízos financeiros graves.
* **Decisões sob responsabilidade do engenheiro:**
  * Determinar o nível de isolamento adequado para cada transação e o escopo correto do `BEGIN ... COMMIT`.
  * Escolher entre controle de concorrência otimista (versão/timestamp) e pessimista (`SELECT FOR UPDATE`).
  * Auditar o tempo de retenção de conexões e travas para evitar contenção e deadlocks.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-02: Processos, threads e I/O](../02-processos-threads-e-io/documento-base.md) e [CAP-03: Contratos e leitura diagnóstica](../03-contratos-e-leitura-diagnostica/documento-base.md).
* **Tópicos essenciais:**
  * Propriedades ACID (Atomicidade, Consistência, Isolamento, Durabilidade).
  * Anomalias de isolamento (ANSI SQL e extensões de Berenson et al., 1995): Dirty Read, Non-Repeatable Read, Phantom Read, Lost Update e Write Skew.
  * Níveis de Isolamento: Read Committed vs. Snapshot Isolation vs. Serializable (2PL e SSI).
  * Concorrência Otimista (OCC) vs. Pessimista (PCC) e detecção de Deadlocks.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Simulação de duas transações concorrentes disputando um saldo ou estoque limitado em um banco relacional (ex.: PostgreSQL / SQLite concorrente).
* **Evidência esperada:** Demonstração da anomalia ocorrendo com a implementação ingênua gerada por IA (Lost Update) e a subsequente correção usando travamento pessimista ou versão otimista, com logs de contenção e integridade preservada.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 2 (Efeitos Colaterais / Banco)* e *Filtro 3 (Invariantes)*.
* **Pergunta de auditoria rápida:** "A leitura e a atualização deste registro estão protegidas dentro de uma transação com isolamento seguro, ou a IA leu o dado, calculou na aplicação e enviou um update desprotegido?"

---

## 6. Fontes Primárias de Referência

1. **Designing Data-Intensive Applications (DDIA)** — Martin Kleppmann (Capítulo 7: Transações e Isolamento).
2. **A Critique of ANSI SQL Isolation Levels** (SIGMOD, 1995) — Hal Berenson, Phil Bernstein, Jim Gray et al.
3. **Database Systems: The Complete Book** — Hector Garcia-Molina, Jeffrey D. Ullman, Jennifer Widom.

