# Documento Base — CAP-08: Modularidade e dependências

**ID:** CAP-08  
**Parte:** IV — Modularidade e Arquitetura  
**Estado:** Planejado — aguardando conclusão de CAP-03 e CAP-05  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Qual Ã© o critÃ©rio matemÃ¡tico e formal correto para fatiar um sistema em mÃ³dulos para que uma mudanÃ§a solicitada pela IA nÃ£o quebre o restante da aplicaÃ§Ã£o?
* **Objetivo de estudo:** Compreender a Teoria Formal da Modularidade (David Parnas, W. P. Stevens), diferenciando tipos de acoplamento e coesÃ£o, aplicando os princÃ­pios SOLID sob a Ã³tica de controle de dependÃªncias e estabilidade arquitetural.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes tÃªm a tendÃªncia natural de agrupar cÃ³digo por similaridade superficial (ex.: juntar tudo que lida com texto no mesmo arquivo) ou de injetar dependÃªncias cruzadas e cÃ­clicas entre classes para resolver rapidamente um erro de compilaÃ§Ã£o imediato.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Aplicar *Information Hiding*: ocultar atrÃ¡s de uma interface exatamente as decisÃµes de design volÃ¡teis (ex.: a tabela de alÃ­quotas fiscais, o driver de banco de dados ou a API de pagamento).
  * Impor direÃ§Ã£o estrita nas dependÃªncias (mÃ³dulos estÃ¡veis nÃ£o devem depender de mÃ³dulos volÃ¡teis).
  * Validar a aplicaÃ§Ã£o do PrincÃ­pio da SubstituiÃ§Ã£o de Liskov (LSP) para garantir que subtipos gerados por IA preservem o contrato esperado pelos chamadores.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-03: Contratos e leitura diagnÃ³stica](../03-contratos-e-leitura-diagnostica/documento-base.md) e [CAP-06: Linguagem e fronteiras de domÃ­nio](../06-linguagem-e-fronteiras-de-dominio/documento-base.md).
* **TÃ³picos essenciais:**
  * O PrincÃ­pio de David Parnas (1972) â€” *On the Criteria To Be Used in Decomposing Systems into Modules* (*Information Hiding*).
  * O espectro de Acoplamento (ConteÃºdo, Comum, Controle, Dados) e CoesÃ£o (Coincidente, Temporal, Comunicacional, Funcional) de Stevens, Myers e Constantine.
  * SOLID como mÃ©tricas de engenharia e controle de dependÃªncias (SRP, OCP, LSP, ISP, DIP).
  * InversÃ£o de Controle (IoC) e InjeÃ§Ã£o de DependÃªncias aplicadas a fronteiras desacopladas.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** AnÃ¡lise de um mÃ³dulo com alto acoplamento e refatoraÃ§Ã£o dirigida por agente isolando uma decisÃ£o propensa a mudanÃ§as atrÃ¡s de uma abstraÃ§Ã£o de contrato estÃ¡vel.
* **EvidÃªncia esperada:** DemonstraÃ§Ã£o comparativa antes/depois documentando a eliminaÃ§Ã£o de dependÃªncias cruzadas e a proteÃ§Ã£o dos clientes contra alteraÃ§Ãµes internas no mÃ³dulo.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *Filtro 1 (Contratos e Assinaturas)* e *Filtro 2 (Efeitos Colaterais)*.
* **Pergunta de auditoria rÃ¡pida:** "Este mÃ³dulo expÃµe sua estrutura interna ou esconde a implementaÃ§Ã£o volÃ¡til atrÃ¡s de um contrato? Se eu trocar a tecnologia de persistÃªncia ou o serviÃ§o externo, quantos arquivos gerados precisarÃ£o ser alterados?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **On the Criteria To Be Used in Decomposing Systems into Modules** (Communications of the ACM, 1972) â€” David L. Parnas.
2. **Structured Design** (IBM Systems Journal, 1974) â€” W. P. Stevens, G. J. Myers, L. L. Constantine.
3. **Agile Software Development: Principles, Patterns, and Practices** â€” Robert C. Martin (seÃ§Ãµes sobre os princÃ­pios SOLID e PrincÃ­pios de Pacotes).

