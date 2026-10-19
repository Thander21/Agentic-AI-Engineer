# Documento Base — CAP-03: Contratos e leitura diagnóstica

**ID:** CAP-03  
**Parte:** II — Garantia da Qualidade, Métricas e Auditoria  
**Estado:** Planejado — aguardando conclusão de CAP-01 e CAP-02  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como auditar o código gerado por um agente em poucos minutos, identificando se ele viola contratos, ignora invariantes de negócio ou gera efeitos colaterais perigosos, sem precisar ler centenas de linhas de código utilitário?
* **Objetivo de estudo:** Desenvolver o método de leitura diagnóstica de fronteiras, dominando o conceito formal de Design por Contrato (pré-condições, pós-condições e invariantes), separando código puro em memória de efeitos colaterais e treinando a auditoria visual rápida.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes preenchem lacunas com código padrão genérico. Ao receber um prompt vago, a IA pode omitir validações essenciais de domínio (ex.: aceitar valores negativos em uma transação financeira) ou alterar o estado global do sistema silenciosamente.
* **Decisões sob responsabilidade do engenheiro:**
  * Avaliar assinaturas e tipos de entrada/saída antes de inspecionar corpos de funções.
  * Localizar onde as regras invioláveis de negócio (invariantes) estão sendo garantidas no código e onde estão desprotegidas.
  * Isolar efeitos colaterais e garantir que funções declaradas como "puras" ou de consulta não realizem alterações de estado ou I/O oculto.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-01: Execução, runtime e memória](../01-execucao-runtime-e-memoria/documento-base.md).
* **Tópicos essenciais:**
  * Design por Contrato (Bertrand Meyer): pré-condições (o que o chamador garante), pós-condições (o que a função devolve) e invariantes de classe/módulo (o que nunca pode ser falso).
  * Efeitos colaterais (*side effects*) vs. Funções puras (*referential transparency*).
  * O Método dos 5 Filtros de Auditoria Visual:
    1. Assinatura e Contrato (entradas, saídas e suficiência de tipos).
    2. Efeitos Colaterais (I/O, chamadas externas, mutação de estado global).
    3. Invariantes por Hipótese (busca direcionada por constantes e condicionais da regra).
    4. Auditoria de Asserções de Teste (verificação de testes falsos/tautológicos).
    5. Inspeção Viva de Execução (telemetria, logs e debugger).

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Uma regra de faturamento/cálculo tributário ou desconto comercial entregue por um agente de IA, contendo um defeito sutil de contrato (ex.: falta de parâmetro essencial de UF) e um efeito colateral oculto.
* **Evidência esperada:** Documento de auditoria diagnóstica contendo a aplicação explícita dos filtros, a demarcação das linhas defeituosas e a formulação de um contrato corrigido.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 1 (Contrato)* e *Filtro 3 (Invariantes por Hipótese)*.
* **Pergunta de auditoria rápida:** "A assinatura deste método expõe todos os dados que a regra exige? Onde está o `if` ou asserção que impede a quebra da regra de negócio caso um valor inválido seja recebido?"

---

## 6. Fontes Primárias de Referência

1. **Object-Oriented Software Construction** — Bertrand Meyer (capítulo sobre Design by Contract).
2. **Clean Code / Pragmatic Programmer** — Robert C. Martin / Andrew Hunt e David Thomas (leitura de código, pureza funcional e comandos vs. consultas — CQS).
3. **SWEBOK v3/v4** — IEEE Computer Society (capítulo sobre Software Quality e Verificação).

