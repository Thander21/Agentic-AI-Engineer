# Documento Base — CAP-05: Contratos e leitura diagnóstica

**ID:** CAP-05  
**Parte:** III — Auditoria, Contratos e Verificação  
**Estado:** Planejado — aguardando conclusão de CAP-01 e CAP-04  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como auditar o cÃ³digo gerado por um agente em poucos minutos, identificando se ele viola contratos, ignora invariantes de negÃ³cio ou gera efeitos colaterais perigosos, sem precisar ler centenas de linhas de cÃ³digo utilitÃ¡rio?
* **Objetivo de estudo:** Desenvolver o mÃ©todo de leitura diagnÃ³stica de fronteiras, dominando o conceito formal de Design por Contrato (prÃ©-condiÃ§Ãµes, pÃ³s-condiÃ§Ãµes e invariantes), separando cÃ³digo puro em memÃ³ria de efeitos colaterais e treinando a auditoria visual rÃ¡pida.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes preenchem lacunas com cÃ³digo padrÃ£o genÃ©rico. Ao receber um prompt vago, a IA pode omitir validaÃ§Ãµes essenciais de domÃ­nio (ex.: aceitar valores negativos em uma transaÃ§Ã£o financeira) ou alterar o estado global do sistema silenciosamente.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Avaliar assinaturas e tipos de entrada/saÃ­da antes de inspecionar corpos de funÃ§Ãµes.
  * Localizar onde as regras inviolÃ¡veis de negÃ³cio (invariantes) estÃ£o sendo garantidas no cÃ³digo e onde estÃ£o desprotegidas.
  * Isolar efeitos colaterais e garantir que funÃ§Ãµes declaradas como "puras" ou de consulta nÃ£o realizem alteraÃ§Ãµes de estado ou I/O oculto.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-01: ExecuÃ§Ã£o, runtime e memÃ³ria](../01-execucao-runtime-e-memoria/documento-base.md).
* **TÃ³picos essenciais:**
  * Design por Contrato (Bertrand Meyer): prÃ©-condiÃ§Ãµes (o que o chamador garante), pÃ³s-condiÃ§Ãµes (o que a funÃ§Ã£o devolve) e invariantes de classe/mÃ³dulo (o que nunca pode ser falso).
  * Efeitos colaterais (*side effects*) vs. FunÃ§Ãµes puras (*referential transparency*).
  * O MÃ©todo dos 5 Filtros de Auditoria Visual:
    1. Assinatura e Contrato (entradas, saÃ­das e suficiÃªncia de tipos).
    2. Efeitos Colaterais (I/O, chamadas externas, mutaÃ§Ã£o de estado global).
    3. Invariantes por HipÃ³tese (busca direcionada por constantes e condicionais da regra).
    4. Auditoria de AsserÃ§Ãµes de Teste (verificaÃ§Ã£o de testes falsos/tautolÃ³gicos).
    5. InspeÃ§Ã£o Viva de ExecuÃ§Ã£o (telemetria, logs e debugger).

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** Uma regra de faturamento/cÃ¡lculo tributÃ¡rio ou desconto comercial entregue por um agente de IA, contendo um defeito sutil de contrato (ex.: falta de parÃ¢metro essencial de UF) e um efeito colateral oculto.
* **EvidÃªncia esperada:** Documento de auditoria diagnÃ³stica contendo a aplicaÃ§Ã£o explÃ­cita dos filtros, a demarcaÃ§Ã£o das linhas defeituosas e a formulaÃ§Ã£o de um contrato corrigido.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 1 (Contrato)* e *Filtro 3 (Invariantes por HipÃ³tese)*.
* **Pergunta de auditoria rÃ¡pida:** "A assinatura deste mÃ©todo expÃµe todos os dados que a regra exige? Onde estÃ¡ o `if` ou asserÃ§Ã£o que impede a quebra da regra de negÃ³cio caso um valor invÃ¡lido seja recebido?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Object-Oriented Software Construction** â€” Bertrand Meyer (capÃ­tulo sobre Design by Contract).
2. **Clean Code / Pragmatic Programmer** â€” Robert C. Martin / Andrew Hunt e David Thomas (leitura de cÃ³digo, pureza funcional e comandos vs. consultas â€” CQS).
3. **SWEBOK v3/v4** â€” IEEE Computer Society (capÃ­tulo sobre Software Quality e VerificaÃ§Ã£o).

