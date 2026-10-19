# Documento Base — CAP-18: Orquestração, contexto e governança de agentes

**ID:** CAP-18  
**Parte:** Transversal — Orquestração, Contexto e Governança de Agentes  
**Estado:** Planejado — consolidação transversal  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como desenhar um ecossistema completo de desenvolvimento agêntico onde múltiplos agentes operam sob especificações formais, com harnesses de contexto otimizados, testes automatizados para os próprios prompts/specs (*evals*) e governança técnica contínua?
* **Objetivo de estudo:** Consolidar a disciplina de Engenharia de Contexto, arquitetura de harnesses de agentes, criação de suítes de avaliação automatizada (*Evals*) e governança de artefatos gerados por IA, integrando todas as competências desenvolvidas ao longo dos 17 capítulos anteriores.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes não governam a si mesmos. Sem um engenheiro que estabeleça limites de atenção (*context window management*), regras rígidas de projeto (`.cursorrules`, `AGENTS.md`, specs) e testes para as especificações, os agentes degradam em alucinações cumulativas e corrompem o repositório.
* **Decisões sob responsabilidade do engenheiro:**
  * Desenhar a arquitetura de contexto e o roteamento de ferramentas/skills para cada tipo de agente.
  * Criar pipelines de avaliação contínua (*Evals*) que testem a assertividade das instruções e especificações antes de enviar para execução.
  * Auditar licenças de código aberto, segurança e integridade de todos os artefatos produzidos por agentes.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** [CAP-07: SDD e rastreabilidade](../07-sdd-e-rastreabilidade-no-desenvolvimento/documento-base.md) e [CAP-11: Propriedades, mutação e eficácia dos testes](../11-propriedades-mutacao-e-eficacia-dos-testes/documento-base.md). Praticado transversalmente desde o CAP-01.
* **Tópicos essenciais:**
  * Engenharia de Contexto (*Context Engineering*): limites de atenção de LLMs, compressão de contexto, estruturas de regras de projeto (`AGENTS.md`, `.cursorrules`, subagentes).
  * Harness de Agentes e MCP (*Model Context Protocol*): como expor ferramentas, leitura e controle com segurança para agentes de IA.
  * Pipelines de Avaliação Automatizada (*Evals*): criação de testes de regressão que avaliam a acurácia dos prompts, especificações e respostas dos agentes.
  * Governança Técnica e Auditoria: rastreabilidade de código gerado por IA, conformidade de licenças e qualidade arquitetural continuada.

---

## 4. Prática e Evidência Esperada

* **Caso didático:** Criação de um harness completo com spec formal, regras de escopo e pipeline de avaliação (*evals*) para um agente autônomo resolver uma tarefa de engenharia sob restrições estritas.
* **Evidência esperada:** Demonstração do ciclo completo de orquestração: especificação -> injeção de contexto -> execução pelo agente -> execução dos evals/testes -> auditoria pelos 5 filtros e aprovação fundamentada da entrega.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtros em destaque:** *Aplicação integrada de todos os 5 Filtros de Auditoria Visual*.
* **Pergunta de auditoria rápida:** "O harness do agente forneceu contexto suficiente sem dispersar a atenção? O pipeline de avaliação capturou desvios de especificação antes de qualquer alteração no repositório principal?"

---

## 6. Fontes Primárias de Referência

1. **Building Effective Agents** — Anthropic Research ([anthropic.com/research/building-effective-agents](https://www.anthropic.com/research/building-effective-agents)).
2. **Model Context Protocol Specification** — Anthropic ([modelcontextprotocol.io](https://modelcontextprotocol.io)).
3. **Evaluating Large Language Model Systems** — Hamel Husain et al. (princípios de Evals e regressão de IA).

