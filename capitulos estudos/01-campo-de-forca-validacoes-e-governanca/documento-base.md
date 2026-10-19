# Documento Base — CAP-01: Campo de força, validações e governança prática

**ID:** CAP-01  
**Parte:** I — Governança Prática e Guardrails  
**Estado:** Planejado — novo ponto de entrada prático  
**Origem prática:** Laboratório vivo do PDV D+ (software fiscal emitindo NFC-e)

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como auditar e garantir a estabilidade, segurança e corretude do código gerado por agentes de IA sem precisar ler linha por linha das milhares de linhas que o modelo produz?
* **Objetivo de estudo:** Dominar a construção de um "Campo de Força" (*Guardrails* automáticos de engenharia) combinando análise estática rigorosa, validação comportamental por caixa-preta, inspeção de escopo via Git diff e oráculos de teste, garantindo governança técnica absoluta sobre o produto.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** A IA gera código com alta fluência sintática e aparência impecável ("código bonito"), mas frequentemente comete erros conceituais graves: violação de regras fiscais, remoção de validações de segurança para fazer um teste passar, ou injeção de dependências espúrias. O engenheiro não é mais um digitador de código; ele é o inspetor que define as regras do campo de força e audita os resultados pelo comportamento externo.
* **Decisões sob responsabilidade do engenheiro:**
  * Definir o "Campo de Força" inegociável do projeto: linters, formatadores, regras de tipo estritas e checagens pré-commit que barram qualquer alucinação na porta de entrada.
  * Estabelecer testes e oráculos de caixa-preta: validar se a saída (ex.: XML da NFC-e, cálculo de imposto) está matematicamente e legalmente correta de acordo com esquemas rígidos (JSON Schema / XSD), independente de como a IA implementou internamente.
  * Praticar a inspeção cirúrgica de escopo: verificar se o agente alterou estritamente o que foi autorizado ou se espalhou refatorações não solicitadas pelo sistema.
  * Julgar a plausibilidade versus a corretude: aprender a desconfiar do código que parece limpo, mas esconde falhas de borda perigosas.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-00: Setup, IDE, harness, git e loops](../00-setup-ide-harness-e-loops/documento-base.md).
* **Tópicos essenciais:**
  * **O Campo de Força (Automated Guardrails):**
    * Análise estática estrita (`analyzer`, linters com regras de erro, tipo estrito).
    * Pre-commit hooks e checagens automáticas de integridade.
  * **A Ilusão do Código Bonito:** A armadilha da sintaxe elegante vs. a realidade de execução (placebos e alucinações bem escritas).
  * **Auditoria Caixa-Preta (Black-Box Validation):**
    * Testar comportamento e contratos externos em vez de auditar detalhes de implementação.
    * Validação estrita por esquemas (XSD/JSON Schema) e asserções de oráculo.
  * **Auditoria de Escopo e Contenção de Danos:**
    * Análise rápida de `git diff` e `git status`: identificando arquivos "tocados" sem justificativa.
    * Métricas de sanidade: proporção de linhas modificadas vs. complexidade entregue.
  * **Governança e Soberania do Desenvolvedor:** Como o autor mantém a autoridade sobre o produto e rejeita entregas da IA sem hesitação.

---

## 4. Prática e Evidência Esperada

* **Ambiente de referência delimitado:** O caso prático do módulo fiscal do PDV D+ (geração e validação de schema de NFC-e).
* **Caso didático:** Uma alteração solicitada a um agente para incluir uma regra de desconto fiscal onde a IA entrega código visualmente impecável, mas altera uma validação de imposto e introduz uma dependência desnecessária.
* **Evidência esperada:** Demonstração dos 3 níveis de barreira do campo de força em ação:
  1. A análise estática e o linter barrando inconsistências de tipo.
  2. A validação por schema XSD rejeitando o XML malformado sem necessidade de leitura do código interno.
  3. A inspeção de diff identificando a invasão de escopo e revertendo cirurgicamente a alteração indevida.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 1 (Contratos e Tipos)* e *Filtro 4 (Auditoria do Teste e Escopo)*.
* **Pergunta de auditoria rápida:** "O que quebrou quando o schema estrito foi aplicado? O agente alterou arquivos além dos que constavam no contrato da tarefa?"

---

## 6. Fontes Primárias de Referência

1. **Clean Architecture: A Craftsman's Guide to Software Structure and Design** — Robert C. Martin (princípios de limites arquiteturais e isolamento de dependências).
2. **Building Evolutionary Architectures** — Neal Ford, Rebecca Parsons, Patrick Kua (conceito de *fitness functions* e testes automatizados de governança).
3. **Manual de Orientação do Contribuinte (MOC) — SEFAZ:** O exemplo definitivo de validação por esquemas estritos (XSD) e regras de validação por oráculo fiscal.

