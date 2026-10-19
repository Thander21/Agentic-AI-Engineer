# Documento Base — CAP-07: Propriedades, mutação e eficácia dos testes

**ID:** CAP-07  
**Parte:** III — Auditoria, Contratos e Verificação  
**Estado:** Planejado — aguardando conclusão de CAP-06  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como medir matematicamente se a nossa suÃ­te de testes realmente detecta bugs sutis introduzidos por agentes, e como usar testes baseados em propriedades para descobrir falhas de borda que nenhum humano ou prompt imaginou?
* **Objetivo de estudo:** Dominar tÃ©cnicas avanÃ§adas de teste: Testes Baseados em Propriedades (*Property-Based Testing*), Testes de MutaÃ§Ã£o (*Mutation Testing* / escore de mutaÃ§Ã£o) e anÃ¡lise de eficÃ¡cia de verificaÃ§Ã£o alÃ©m da ingÃªnua porcentagem de cobertura de linhas.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Cobertura de cÃ³digo (Code Coverage) de 100% nÃ£o significa que o cÃ³digo estÃ¡ livre de bugs â€” apenas que todas as linhas foram executadas durante os testes. Agentes frequentemente atingem 100% de cobertura com asserÃ§Ãµes fracas. Testes de mutaÃ§Ã£o sabotam o cÃ³digo propositalmente para provar se a suÃ­te detecta a alteraÃ§Ã£o.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Formular invariantes matemÃ¡ticas para testes de propriedades (ex.: idempotÃªncia, reversibilidade, comutatividade).
  * Avaliar o escore de mutaÃ§Ã£o (*mutation score*) e rejeitar suÃ­tes de testes cujos mutantes sobrevivem.
  * Utilizar geradores automÃ¡ticos de dados de teste (fuzzing / property testing) para encontrar casos de borda extremos.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-10: VerificaÃ§Ã£o, validaÃ§Ã£o e aceitaÃ§Ã£o](../10-verificacao-validacao-e-aceitacao/documento-base.md).
* **TÃ³picos essenciais:**
  * Limites da cobertura de cÃ³digo tradicional (Line & Branch Coverage vs. Test Efficacy).
  * Testes Baseados em Propriedades (QuickCheck / hipÃ³teses invariantes): geraÃ§Ã£o estocÃ¡stica de entradas extremas (valores nulos, strings com emojis, inteiros mÃ¡ximos/mÃ­nimos, coleÃ§Ãµes vazias).
  * Testes de MutaÃ§Ã£o: introduÃ§Ã£o proposital de falhas (troca de `>` por `>=`, exclusÃ£o de chamadas) e verificaÃ§Ã£o de "mutantes mortos" vs. "mutantes sobreviventes".
  * EstratÃ©gias de teste para algoritmos determinÃ­sticos e funÃ§Ãµes de negÃ³cio puras.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** AplicaÃ§Ã£o de um framework de teste de mutaÃ§Ã£o em uma funÃ§Ã£o de cÃ¡lculo de juros/desconto entregue por IA com suposta "100% de cobertura", seguida pela criaÃ§Ã£o de um teste baseado em propriedades.
* **EvidÃªncia esperada:** Registro da taxa de sobrevivÃªncia dos mutantes antes e depois do aprimoramento das asserÃ§Ãµes, documentando pelo menos 1 caso de borda descoberto pelo teste de propriedades que a IA nÃ£o havia considerado.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtro em destaque:** *Filtro 4 (Auditoria do Teste)* e *Filtro 3 (Invariantes)*.
* **Pergunta de auditoria rÃ¡pida:** "Se um operador matemÃ¡tico ou condicional for invertido nesta funÃ§Ã£o, algum teste da suÃ­te falha imediatamente, ou o teste deixa o mutante sobreviver?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **QuickCheck: A Lightweight Tool for Random Testing of Haskell Programs** â€” Koen Claessen e John Hughes.
2. **Mutation Testing for the New Millennium** â€” Mark Harman et al.
3. **Property-Based Testing with PropEr, Erlang, and Elixir** â€” Fred Hebert (fundamentos de propriedades e invariantes universais).

