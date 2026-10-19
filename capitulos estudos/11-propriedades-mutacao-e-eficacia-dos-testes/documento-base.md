# Documento Base — CAP-11: Propriedades, mutação e eficácia dos testes

**ID:** CAP-11  
**Parte:** V — Verificação, Validação e Testes  
**Estado:** Planejado — aguardando conclusão de CAP-10  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como medir matematicamente se a nossa suíte de testes realmente detecta bugs sutis introduzidos por agentes, e como usar testes baseados em propriedades para descobrir falhas de borda que nenhum humano ou prompt imaginou?
* **Objetivo de estudo:** Dominar técnicas avançadas de teste: Testes Baseados em Propriedades (*Property-Based Testing*), Testes de Mutação (*Mutation Testing* / escore de mutação) e análise de eficácia de verificação além da ingênua porcentagem de cobertura de linhas.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Cobertura de código (Code Coverage) de 100% não significa que o código está livre de bugs — apenas que todas as linhas foram executadas durante os testes. Agentes frequentemente atingem 100% de cobertura com asserções fracas. Testes de mutação sabotam o código propositalmente para provar se a suíte detecta a alteração.
* **Decisões sob responsabilidade do engenheiro:**
  * Formular invariantes matemáticas para testes de propriedades (ex.: idempotência, reversibilidade, comutatividade).
  * Avaliar o escore de mutação (*mutation score*) e rejeitar suítes de testes cujos mutantes sobrevivem.
  * Utilizar geradores automáticos de dados de teste (fuzzing / property testing) para encontrar casos de borda extremos.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-10: Verificação, validação e aceitação](../10-verificacao-validacao-e-aceitacao/documento-base.md).
* **Tópicos essenciais:**
  * Limites da cobertura de código tradicional (Line & Branch Coverage vs. Test Efficacy).
  * Testes Baseados em Propriedades (QuickCheck / hipóteses invariantes): geração estocástica de entradas extremas (valores nulos, strings com emojis, inteiros máximos/mínimos, coleções vazias).
  * Testes de Mutação: introdução proposital de falhas (troca de `>` por `>=`, exclusão de chamadas) e verificação de "mutantes mortos" vs. "mutantes sobreviventes".
  * Estratégias de teste para algoritmos determinísticos e funções de negócio puras.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Aplicação de um framework de teste de mutação em uma função de cálculo de juros/desconto entregue por IA com suposta "100% de cobertura", seguida pela criação de um teste baseado em propriedades.
* **Evidência esperada:** Registro da taxa de sobrevivência dos mutantes antes e depois do aprimoramento das asserções, documentando pelo menos 1 caso de borda descoberto pelo teste de propriedades que a IA não havia considerado.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtro em destaque:** *Filtro 4 (Auditoria do Teste)* e *Filtro 3 (Invariantes)*.
* **Pergunta de auditoria rápida:** "Se um operador matemático ou condicional for invertido nesta função, algum teste da suíte falha imediatamente, ou o teste deixa o mutante sobreviver?"

---

## 6. Fontes Primárias de Referência

1. **QuickCheck: A Lightweight Tool for Random Testing of Haskell Programs** — Koen Claessen e John Hughes.
2. **Mutation Testing for the New Millennium** — Mark Harman et al.
3. **Property-Based Testing with PropEr, Erlang, and Elixir** — Fred Hebert (fundamentos de propriedades e invariantes universais).

