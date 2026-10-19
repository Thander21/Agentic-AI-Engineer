# Documento Base — CAP-10: Verificação, validação e aceitação

**ID:** CAP-10  
**Parte:** V — Verificação, Validação e Testes  
**Estado:** Planejado — aguardando conclusão de CAP-03 e CAP-05  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como ter certeza de que o software gerado pela IA faz a coisa certa (validação) e funciona da maneira correta (verificação), sem cair na ilusão de testes tautológicos verdes que não testam nada?
* **Objetivo de estudo:** Distinguir formalmente Verificação de Validação (V&V), compreender a Pirâmide e o Troféu de Testes, dominar o Desenvolvimento Guiado por Comportamento (BDD) e aprender a auditar asserções de testes criadas por agentes de IA.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** IAs são especialistas em gerar "testes de farsa": mocks que respondem exatamente o que o teste espera, asserções vazias ou testes que apenas executam o método sem validar o estado resultante. O desenvolvedor despreparado vê a barra verde e acredita falsamente que a funcionalidade está garantida.
* **Decisões sob responsabilidade do engenheiro:**
  * Auditar o código do teste antes de aprovar o código de produção gerado.
  * Escolher o nível adequado de teste (unitário, integração ou ponta a ponta) para cada componente sem inflar a suíte com testes lentos e frágeis.
  * Formular cenários BDD claros (Dado / Quando / Então) que sirvam de gabarito inequívoco para a IA implementar e verificar.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-03: Contratos e leitura diagnóstica](../03-contratos-e-leitura-diagnostica/documento-base.md) e [CAP-05: Problema, requisitos e atributos de qualidade](../05-problema-requisitos-e-atributos-de-qualidade/documento-base.md).
* **Tópicos essenciais:**
  * Verificação ("Construímos o produto corretamente?") vs. Validação ("Construímos o produto certo?").
  * Pirâmide de Testes (Mike Cohn) vs. Troféu de Testes (Kent C. Dodds): custos, velocidade e isolamento.
  * BDD (*Behavior-Driven Development*) com especificação executável (Gherkin: Given / When / Then).
  * Anatomia de um teste real: Arrange, Act, Assert (AAA).
  * A farsa dos testes tautológicos e o perigo de mocks excessivos.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Uma suíte de testes gerada por um agente para uma regra de faturamento contendo um teste tautológico camuflado e um teste com mock circular.
* **Evidência esperada:** Auditoria demonstrando por que o teste falso passa mesmo com o código quebrado, reescrita do teste com asserções reais baseadas em BDD e verificação de sua quebra legítima quando a regra é violada.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtro em destaque:** *Filtro 4 (Auditoria do Teste e Asserções)*.
* **Pergunta de auditoria rápida:** "Se eu alterar a resposta esperada no `Assert` para um valor intencionalmente errado, o teste quebra de verdade? O teste valida o comportamento ou apenas mockou o próprio retorno que finge verificar?"

---

## 6. Fontes Primárias de Referência

1. **Unit Testing Principles, Practices, and Patterns** — Vladimir Khorikov (capítulos sobre o que torna um teste bom e perigos de mocks).
2. **Growing Object-Oriented Software, Guided by Tests** — Steve Freeman e Nat Pryce.
3. **Specification by Example** — Gojko Adzic (como criar especificações executáveis e BDD).

