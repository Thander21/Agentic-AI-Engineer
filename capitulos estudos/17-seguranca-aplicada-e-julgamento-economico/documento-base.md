# Documento Base — CAP-17: Segurança aplicada e julgamento econômico

**ID:** CAP-17  
**Parte:** VII — Evolução, Manutenção e Resiliência em Produção  
**Estado:** Planejado — aguardando conclusão de CAP-09 e CAP-14  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como auditar vulnerabilidades críticas de segurança (OWASP Top 10, criptografia inadequada, vazamento de credenciais) introduzidas pelo agente de IA e equilibrar essas defesas com os custos reais de desenvolvimento, infraestrutura e manutenção (economia do software)?
* **Objetivo de estudo:** Dominar práticas fundamentais de Segurança da Informação Aplicada (criptografia de dados em trânsito e em repouso, gerenciamento de segredos, OWASP Top 10) e desenvolver o Julgamento Econômico de Engenharia (Trade-offs de custo de infraestrutura, Total Cost of Ownership - TCO e retorno sobre investimento de qualidade).

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes frequentemente inserem chaves de API *hardcoded* no código, utilizam funções de hash fracas ou obsoletas (como MD5 ou SHA-1 para senhas) e sugerem arquiteturas na nuvem com dezenas de instâncias que geram faturas astronômicas sem necessidade real de negócio.
* **Decisões sob responsabilidade do engenheiro:**
  * Rejeitar código que contenha credenciais, conexões desprotegidas ou riscos de injeção (SQL/Command Injection).
  * Exigir hashing robusto (bcrypt, Argon2) e gerenciamento seguro de variáveis de ambiente.
  * Julgar a viabilidade econômica de cada decisão técnica, comparando o custo de implementação e manutenção com o risco de falha.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-09: Escolhas arquiteturais](../09-escolhas-arquiteturais/documento-base.md) e [CAP-14: Mensageria, APIs e sincronização](../14-mensageria-apis-e-sincronizacao/documento-base.md).
* **Tópicos essenciais:**
  * Fundamentos de Criptografia Aplicada: simétrica (AES-GCM), assimétrica (RSA, Ed25519), funções de derivação de chaves e hashing de senhas seguro (Argon2, bcrypt).
  * OWASP Top 10 (Injection, Broken Authentication, Sensitive Data Exposure, Security Misconfiguration).
  * Gestão de Segredos e Conformidade (*Principle of Least Privilege*).
  * Economia do Software: Custo Total de Propriedade (TCO), custos de nuvem (FinOps básico) e julgamento pragmático de engenharia (*good enough vs. overengineering*).

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Submissão de um fluxo de autenticação e armazenamento de dados gerado por agente a uma análise de risco e segurança, apontando falhas e readequando o módulo com padrões criptográficos seguros.
* **Evidência esperada:** Matriz de risco e análise de trade-off econômico documentando as vulnerabilidades encontradas, a correção implementada e o impacto no custo e na manutenibilidade da solução.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Filtro 1 (Contratos e Tipagem)* e *Filtro 2 (Efeitos Colaterais e Segredos)*.
* **Pergunta de auditoria rápida:** "Há alguma chave secreta ou credencial exposta no código? Como as senhas ou dados sensíveis estão sendo criptografados e armazenados?"

---

## 6. Fontes Primárias de Referência

1. **Security Engineering: A Guide to Building Dependable Distributed Systems** — Ross J. Anderson.
2. **OWASP Top 10 Application Security Risks** ([owasp.org/www-project-top-ten](https://owasp.org/www-project-top-ten/)).
3. **Software Engineering Economics** — Barry Boehm.

