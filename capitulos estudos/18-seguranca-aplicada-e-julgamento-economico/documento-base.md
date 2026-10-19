# Documento Base — CAP-18: Segurança aplicada e julgamento econômico

**ID:** CAP-18  
**Parte:** VII — Produção e Soberania  
**Estado:** Planejado — aguardando conclusão de CAP-09 e CAP-15  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como auditar vulnerabilidades crÃ­ticas de seguranÃ§a (OWASP Top 10, criptografia inadequada, vazamento de credenciais) introduzidas pelo agente de IA e equilibrar essas defesas com os custos reais de desenvolvimento, infraestrutura e manutenÃ§Ã£o (economia do software)?
* **Objetivo de estudo:** Dominar prÃ¡ticas fundamentais de SeguranÃ§a da InformaÃ§Ã£o Aplicada (criptografia de dados em trÃ¢nsito e em repouso, gerenciamento de segredos, OWASP Top 10) e desenvolver o Julgamento EconÃ´mico de Engenharia (Trade-offs de custo de infraestrutura, Total Cost of Ownership - TCO e retorno sobre investimento de qualidade).

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes frequentemente inserem chaves de API *hardcoded* no cÃ³digo, utilizam funÃ§Ãµes de hash fracas ou obsoletas (como MD5 ou SHA-1 para senhas) e sugerem arquiteturas na nuvem com dezenas de instÃ¢ncias que geram faturas astronÃ´micas sem necessidade real de negÃ³cio.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Rejeitar cÃ³digo que contenha credenciais, conexÃµes desprotegidas ou riscos de injeÃ§Ã£o (SQL/Command Injection).
  * Exigir hashing robusto (bcrypt, Argon2) e gerenciamento seguro de variÃ¡veis de ambiente.
  * Julgar a viabilidade econÃ´mica de cada decisÃ£o tÃ©cnica, comparando o custo de implementaÃ§Ã£o e manutenÃ§Ã£o com o risco de falha.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-09: Escolhas arquiteturais](../09-escolhas-arquiteturais/documento-base.md) e [CAP-14: Mensageria, APIs e sincronizaÃ§Ã£o](../14-mensageria-apis-e-sincronizacao/documento-base.md).
* **TÃ³picos essenciais:**
  * Fundamentos de Criptografia Aplicada: simÃ©trica (AES-GCM), assimÃ©trica (RSA, Ed25519), funÃ§Ãµes de derivaÃ§Ã£o de chaves e hashing de senhas seguro (Argon2, bcrypt).
  * OWASP Top 10 (Injection, Broken Authentication, Sensitive Data Exposure, Security Misconfiguration).
  * GestÃ£o de Segredos e Conformidade (*Principle of Least Privilege*).
  * Economia do Software: Custo Total de Propriedade (TCO), custos de nuvem (FinOps bÃ¡sico) e julgamento pragmÃ¡tico de engenharia (*good enough vs. overengineering*).

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** SubmissÃ£o de um fluxo de autenticaÃ§Ã£o e armazenamento de dados gerado por agente a uma anÃ¡lise de risco e seguranÃ§a, apontando falhas e readequando o mÃ³dulo com padrÃµes criptogrÃ¡ficos seguros.
* **EvidÃªncia esperada:** Matriz de risco e anÃ¡lise de trade-off econÃ´mico documentando as vulnerabilidades encontradas, a correÃ§Ã£o implementada e o impacto no custo e na manutenibilidade da soluÃ§Ã£o.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 1 (Contratos e Tipagem)* e *Filtro 2 (Efeitos Colaterais e Segredos)*.
* **Pergunta de auditoria rÃ¡pida:** "HÃ¡ alguma chave secreta ou credencial exposta no cÃ³digo? Como as senhas ou dados sensÃ­veis estÃ£o sendo criptografados e armazenados?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Security Engineering: A Guide to Building Dependable Distributed Systems** â€” Ross J. Anderson.
2. **OWASP Top 10 Application Security Risks** ([owasp.org/www-project-top-ten](https://owasp.org/www-project-top-ten/)).
3. **Software Engineering Economics** â€” Barry Boehm.

