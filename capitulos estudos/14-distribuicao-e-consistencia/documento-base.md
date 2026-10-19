# Documento Base — CAP-14: Distribuição e consistência

**ID:** CAP-14  
**Parte:** VI — Dados, Concorrência e Distribuição  
**Estado:** Planejado — aguardando conclusão de CAP-09 e CAP-13  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Quando dividimos um sistema em mÃºltiplos nÃ³s ou serviÃ§os, o que acontece durante falhas parciais de rede, e por que nÃ£o Ã© possÃ­vel ter consistÃªncia imediata e disponibilidade total simultaneamente?
* **Objetivo de estudo:** Analisar formalmente os teoremas fundamentais de sistemas distribuÃ­dos (Teorema CAP e modelo PACELC), modelos de consistÃªncia (Linearizabilidade vs. ConsistÃªncia Eventual) e coordenaÃ§Ã£o distribuÃ­da (Two-Phase Commit - 2PC vs. PadrÃ£o Saga).

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes pressupÃµem que a rede Ã© rÃ¡pida, confiÃ¡vel e infinita (as clÃ¡ssicas FalÃ¡cias da ComputaÃ§Ã£o DistribuÃ­da). Ao projetar operaÃ§Ãµes entre mÃºltiplos serviÃ§os, a IA frequentemente cria transaÃ§Ãµes distribuÃ­das ingÃªnuas que deixam o sistema travado caso um serviÃ§o terceiro fique lento ou indisponÃ­vel.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Escolher o trade-off entre consistÃªncia forte e alta disponibilidade sob partiÃ§Ã£o de rede (CAP/PACELC).
  * Projetar fluxos de compensaÃ§Ã£o no padrÃ£o Saga (orquestrado vs. coreografado) em vez de acoplar serviÃ§os com 2PC sÃ­ncrono.
  * Delimitar as janelas de inconsistÃªncia tolerÃ¡veis pelo negÃ³cio.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-09: Escolhas arquiteturais](../09-escolhas-arquiteturais/documento-base.md) e [CAP-12: Dados, transaÃ§Ãµes e isolamento](../12-dados-transacoes-e-isolamento/documento-base.md).
* **TÃ³picos essenciais:**
  * As 8 FalÃ¡cias da ComputaÃ§Ã£o DistribuÃ­da (Peter Deutsch).
  * Teorema CAP de Eric Brewer (ConsistÃªncia, Disponibilidade, TolerÃ¢ncia a PartiÃ§Ãµes) e extensÃ£o PACELC (Daniel Abadi).
  * ConsistÃªncia Forte (Linearizabilidade) vs. ConsistÃªncia Causal vs. ConsistÃªncia Eventual.
  * Two-Phase Commit (2PC): o risco do bloqueio em caso de falha do coordenador.
  * PadrÃ£o Saga: transaÃ§Ãµes locais, eventos e aÃ§Ãµes compensatÃ³rias.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** Projeto de um fluxo de reserva/pagamento distribuÃ­do entre dois serviÃ§os independentes sob simulaÃ§Ã£o de queda de rede no meio da operaÃ§Ã£o.
* **EvidÃªncia esperada:** ComparaÃ§Ã£o formal entre uma tentativa de commit de duas fases (2PC) e um fluxo Saga com transaÃ§Ãµes compensatÃ³rias, demonstrando a recuperaÃ§Ã£o do estado consistente apÃ³s a falha.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 2 (Efeitos Colaterais / Rede)* e *Filtro 3 (Invariantes)*.
* **Pergunta de auditoria rÃ¡pida:** "O que acontece se a chamada HTTP externa nesta etapa falhar com timeout? Existe uma aÃ§Ã£o de compensaÃ§Ã£o ou o sistema deixa dados Ã³rfÃ£os e inconsistentes no banco?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Designing Data-Intensive Applications (DDIA)** â€” Martin Kleppmann (CapÃ­tulos 8 e 9: Problemas com Sistemas DistribuÃ­dos e ConsistÃªncia/Consenso).
2. **Consistency Tradeoffs in Modern Distributed Database System Design (PACELC)** â€” Daniel J. Abadi.
3. **Sagas** (ACM SIGMOD, 1987) â€” Hector Garcia-Molina e Kenneth Salem.

