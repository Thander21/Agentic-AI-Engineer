# Documento Base — CAP-13: Dados, transações e isolamento

**ID:** CAP-13  
**Parte:** VI — Dados, Concorrência e Distribuição  
**Estado:** Planejado — aguardando conclusão de CAP-05 e CAP-11  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** O que acontece quando dois usuÃ¡rios executam a mesma operaÃ§Ã£o simultaneamente no banco de dados, e por que o cÃ³digo gerado pela IA Ã© propenso a corromper saldos, criar deadlocks ou permitir leituras fantasmas?
* **Objetivo de estudo:** Compreender em profundidade as propriedades ACID, os nÃ­veis formais de isolamento de transaÃ§Ãµes (Read Uncommitted, Read Committed, Repeatable Read, Serializable), anomalias de concorrÃªncia e estratÃ©gias de bloqueio (travamento pessimista vs. otimista).

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** IAs quase invariavelmente escrevem consultas sem pensar em concorrÃªncia (ex.: fazer um `SELECT saldo FROM conta`, calcular o novo saldo em memÃ³ria na aplicaÃ§Ã£o e depois rodar um `UPDATE conta SET saldo = novo_saldo`). Sob concorrÃªncia real, isso gera a clÃ¡ssica perda de atualizaÃ§Ã£o (*Lost Update*), causando prejuÃ­zos financeiros graves.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Determinar o nÃ­vel de isolamento adequado para cada transaÃ§Ã£o e o escopo correto do `BEGIN ... COMMIT`.
  * Escolher entre controle de concorrÃªncia otimista (versÃ£o/timestamp) e pessimista (`SELECT FOR UPDATE`).
  * Auditar o tempo de retenÃ§Ã£o de conexÃµes e travas para evitar contenÃ§Ã£o e deadlocks.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-02: Processos, threads e I/O](../02-processos-threads-e-io/documento-base.md) e [CAP-03: Contratos e leitura diagnÃ³stica](../03-contratos-e-leitura-diagnostica/documento-base.md).
* **TÃ³picos essenciais:**
  * Propriedades ACID (Atomicidade, ConsistÃªncia, Isolamento, Durabilidade).
  * Anomalias de isolamento (ANSI SQL e extensÃµes de Berenson et al., 1995): Dirty Read, Non-Repeatable Read, Phantom Read, Lost Update e Write Skew.
  * NÃ­veis de Isolamento: Read Committed vs. Snapshot Isolation vs. Serializable (2PL e SSI).
  * ConcorrÃªncia Otimista (OCC) vs. Pessimista (PCC) e detecÃ§Ã£o de Deadlocks.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** SimulaÃ§Ã£o de duas transaÃ§Ãµes concorrentes disputando um saldo ou estoque limitado em um banco relacional (ex.: PostgreSQL / SQLite concorrente).
* **EvidÃªncia esperada:** DemonstraÃ§Ã£o da anomalia ocorrendo com a implementaÃ§Ã£o ingÃªnua gerada por IA (Lost Update) e a subsequente correÃ§Ã£o usando travamento pessimista ou versÃ£o otimista, com logs de contenÃ§Ã£o e integridade preservada.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 2 (Efeitos Colaterais / Banco)* e *Filtro 3 (Invariantes)*.
* **Pergunta de auditoria rÃ¡pida:** "A leitura e a atualizaÃ§Ã£o deste registro estÃ£o protegidas dentro de uma transaÃ§Ã£o com isolamento seguro, ou a IA leu o dado, calculou na aplicaÃ§Ã£o e enviou um update desprotegido?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Designing Data-Intensive Applications (DDIA)** â€” Martin Kleppmann (CapÃ­tulo 7: TransaÃ§Ãµes e Isolamento).
2. **A Critique of ANSI SQL Isolation Levels** (SIGMOD, 1995) â€” Hal Berenson, Phil Bernstein, Jim Gray et al.
3. **Database Systems: The Complete Book** â€” Hector Garcia-Molina, Jeffrey D. Ullman, Jennifer Widom.

