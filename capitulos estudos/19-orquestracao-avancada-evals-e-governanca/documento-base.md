# Documento Base — CAP-19: Orquestração avançada, evals e governança

**ID:** CAP-19  
**Parte:** VII — Produção e Soberania  
**Estado:** Planejado — aguardando conclusão de CAP-04, CAP-07 e CAP-17  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como desenhar um ecossistema completo de desenvolvimento agÃªntico onde mÃºltiplos agentes operam sob especificaÃ§Ãµes formais, com harnesses de contexto otimizados, testes automatizados para os prÃ³prios prompts/specs (*evals*) e governanÃ§a tÃ©cnica contÃ­nua?
* **Objetivo de estudo:** Consolidar a disciplina de Engenharia de Contexto, arquitetura de harnesses de agentes, criaÃ§Ã£o de suÃ­tes de avaliaÃ§Ã£o automatizada (*Evals*) e governanÃ§a de artefatos gerados por IA, integrando todas as competÃªncias desenvolvidas ao longo dos 17 capÃ­tulos anteriores.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes nÃ£o governam a si mesmos. Sem um engenheiro que estabeleÃ§a limites de atenÃ§Ã£o (*context window management*), regras rÃ­gidas de projeto (`.cursorrules`, `AGENTS.md`, specs) e testes para as especificaÃ§Ãµes, os agentes degradam em alucinaÃ§Ãµes cumulativas e corrompem o repositÃ³rio.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Desenhar a arquitetura de contexto e o roteamento de ferramentas/skills para cada tipo de agente.
  * Criar pipelines de avaliaÃ§Ã£o contÃ­nua (*Evals*) que testem a assertividade das instruÃ§Ãµes e especificaÃ§Ãµes antes de enviar para execuÃ§Ã£o.
  * Auditar licenÃ§as de cÃ³digo aberto, seguranÃ§a e integridade de todos os artefatos produzidos por agentes.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** [CAP-07: SDD e rastreabilidade](../07-sdd-e-rastreabilidade-no-desenvolvimento/documento-base.md) e [CAP-11: Propriedades, mutaÃ§Ã£o e eficÃ¡cia dos testes](../11-propriedades-mutacao-e-eficacia-dos-testes/documento-base.md). Praticado transversalmente desde o CAP-01.
* **TÃ³picos essenciais:**
  * Engenharia de Contexto (*Context Engineering*): limites de atenÃ§Ã£o de LLMs, compressÃ£o de contexto, estruturas de regras de projeto (`AGENTS.md`, `.cursorrules`, subagentes).
  * Harness de Agentes e MCP (*Model Context Protocol*): como expor ferramentas, leitura e controle com seguranÃ§a para agentes de IA.
  * Pipelines de AvaliaÃ§Ã£o Automatizada (*Evals*): criaÃ§Ã£o de testes de regressÃ£o que avaliam a acurÃ¡cia dos prompts, especificaÃ§Ãµes e respostas dos agentes.
  * GovernanÃ§a TÃ©cnica e Auditoria: rastreabilidade de cÃ³digo gerado por IA, conformidade de licenÃ§as e qualidade arquitetural continuada.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Caso didÃ¡tico:** CriaÃ§Ã£o de um harness completo com spec formal, regras de escopo e pipeline de avaliaÃ§Ã£o (*evals*) para um agente autÃ´nomo resolver uma tarefa de engenharia sob restriÃ§Ãµes estritas.
* **EvidÃªncia esperada:** DemonstraÃ§Ã£o do ciclo completo de orquestraÃ§Ã£o: especificaÃ§Ã£o -> injeÃ§Ã£o de contexto -> execuÃ§Ã£o pelo agente -> execuÃ§Ã£o dos evals/testes -> auditoria pelos 5 filtros e aprovaÃ§Ã£o fundamentada da entrega.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtros em destaque:** *AplicaÃ§Ã£o integrada de todos os 5 Filtros de Auditoria Visual*.
* **Pergunta de auditoria rÃ¡pida:** "O harness do agente forneceu contexto suficiente sem dispersar a atenÃ§Ã£o? O pipeline de avaliaÃ§Ã£o capturou desvios de especificaÃ§Ã£o antes de qualquer alteraÃ§Ã£o no repositÃ³rio principal?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Building Effective Agents** â€” Anthropic Research ([anthropic.com/research/building-effective-agents](https://www.anthropic.com/research/building-effective-agents)).
2. **Model Context Protocol Specification** â€” Anthropic ([modelcontextprotocol.io](https://modelcontextprotocol.io)).
3. **Evaluating Large Language Model Systems** â€” Hamel Husain et al. (princÃ­pios de Evals e regressÃ£o de IA).

