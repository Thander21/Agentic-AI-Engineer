# Documento Base — CAP-06: Verificação, validação e aceitação

**ID:** CAP-06  
**Parte:** III — Auditoria, Contratos e Verificação  
**Estado:** Planejado — aguardando conclusão de CAP-02 e CAP-05  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como ter certeza de que o software gerado pela IA faz a coisa certa (validaÃ§Ã£o) e funciona da maneira correta (verificaÃ§Ã£o), sem cair na ilusÃ£o de testes tautolÃ³gicos verdes que nÃ£o testam nada?
* **Objetivo de estudo:** Distinguir formalmente VerificaÃ§Ã£o de ValidaÃ§Ã£o (V&V), compreender a PirÃ¢mide e o TrofÃ©u de Testes, dominar o Desenvolvimento Guiado por Comportamento (BDD) e aprender a auditar asserÃ§Ãµes de testes criadas por agentes de IA.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** IAs sÃ£o especialistas em gerar "testes de farsa": mocks que respondem exatamente o que o teste espera, asserÃ§Ãµes vazias ou testes que apenas executam o mÃ©todo sem validar o estado resultante. O desenvolvedor despreparado vÃª a barra verde e acredita falsamente que a funcionalidade estÃ¡ garantida.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Auditar o cÃ³digo do teste antes de aprovar o cÃ³digo de produÃ§Ã£o gerado.
  * Escolher o nÃ­vel adequado de teste (unitÃ¡rio, integraÃ§Ã£o ou ponta a ponta) para cada componente sem inflar a suÃ­te com testes lentos e frÃ¡geis.
  * Formular cenÃ¡rios BDD claros (Dado / Quando / EntÃ£o) que sirvam de gabarito inequÃ­voco para a IA implementar e verificar.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-03: Contratos e leitura diagnÃ³stica](../03-contratos-e-leitura-diagnostica/documento-base.md) e [CAP-05: Problema, requisitos e atributos de qualidade](../05-problema-requisitos-e-atributos-de-qualidade/documento-base.md).
* **TÃ³picos essenciais:**
  * VerificaÃ§Ã£o ("ConstruÃ­mos o produto corretamente?") vs. ValidaÃ§Ã£o ("ConstruÃ­mos o produto certo?").
  * PirÃ¢mide de Testes (Mike Cohn) vs. TrofÃ©u de Testes (Kent C. Dodds): custos, velocidade e isolamento.
  * BDD (*Behavior-Driven Development*) com especificaÃ§Ã£o executÃ¡vel (Gherkin: Given / When / Then).
  * Anatomia de um teste real: Arrange, Act, Assert (AAA).
  * A farsa dos testes tautolÃ³gicos e o perigo de mocks excessivos.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** Uma suÃ­te de testes gerada por um agente para uma regra de faturamento contendo um teste tautolÃ³gico camuflado e um teste com mock circular.
* **EvidÃªncia esperada:** Auditoria demonstrando por que o teste falso passa mesmo com o cÃ³digo quebrado, reescrita do teste com asserÃ§Ãµes reais baseadas em BDD e verificaÃ§Ã£o de sua quebra legÃ­tima quando a regra Ã© violada.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtro em destaque:** *Filtro 4 (Auditoria do Teste e AsserÃ§Ãµes)*.
* **Pergunta de auditoria rÃ¡pida:** "Se eu alterar a resposta esperada no `Assert` para um valor intencionalmente errado, o teste quebra de verdade? O teste valida o comportamento ou apenas mockou o prÃ³prio retorno que finge verificar?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Unit Testing Principles, Practices, and Patterns** â€” Vladimir Khorikov (capÃ­tulos sobre o que torna um teste bom e perigos de mocks).
2. **Growing Object-Oriented Software, Guided by Tests** â€” Steve Freeman e Nat Pryce.
3. **Specification by Example** â€” Gojko Adzic (como criar especificaÃ§Ãµes executÃ¡veis e BDD).

