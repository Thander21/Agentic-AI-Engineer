# Documento Base — CAP-00: Setup, IDE, harness, git e loops

**ID:** CAP-00  
**Parte:** 0 — O Setup do Engenheiro Agêntico  
**Estado:** Planejado — novo ponto de entrada  

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Como estruturar um ambiente profissional de desenvolvimento onde agentes de IA operam com regras claras, contexto controlado, ferramentas delimitadas e loops de validação contínua sem comprometer a integridade do código?
* **Objetivo de estudo:** Compreender a infraestrutura que transforma o uso casual de LLMs em engenharia agêntica: o conceito de *Harness*, o protocolo MCP (*Model Context Protocol*), a especialização por *Skills* e *Subagentes*, a utilização do Git com *worktrees* para isolamento de contexto e o fechamento de loops de execução e feedback autônomo na IDE.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Um modelo de linguagem isolado em um chat web é apenas um gerador de texto. Ele não tem acesso ao sistema de arquivos, não roda testes, não compila código e não conhece as restrições da sua empresa. O engenheiro é quem desenha o "harness" (a armadura/ambiente) que dá olhos, mãos e limites seguros para os agentes atuarem.
* **Decisões sob responsabilidade do engenheiro:**
  * Delimitar as regras operacionais do repositório (ex.: `AGENTS.md`, diretrizes de commit, convenções de código).
  * Configurar ferramentas locais (MCP servers) e conceder apenas os privilégios necessários para cada agente.
  * Escolher a topologia de agentes: quando usar um único agente generalista versus subagentes especializados (pesquisador, redator, auditor).
  * Isolar tarefas concorrentes em *git worktrees* ou branches descartáveis para evitar conflitos de arquivos e contaminação de contexto.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** Uso básico de terminal, Git fundamental e familiaridade com uma IDE moderna.
* **Tópicos essenciais:**
  * **Anatomia do Modelo:** Janela de contexto (*context window*), atenção (*attention mechanisms*), tokenização, perda de foco (*context drift*) e custo de processamento.
  * **O Conceito de Harness:** O ecossistema em torno da LLM (prompts de sistema, regras de projeto, injeção dinâmica de contexto e catálogo de ferramentas).
  * **MCP (Model Context Protocol):** Padronização da conexão entre agentes e ferramentas (leitura de arquivos, acesso a banco, execução controlada).
  * **Skills e Subagentes:** Divisão de trabalho modular; agentes efêmeros com ferramentas restritas vs. agentes orquestradores.
  * **Git e Worktrees para IA:** Como ramificar workspaces fisicamente para múltiplos agentes trabalharem em paralelo sem colisões de branch.
  * **Loops de Automação e Feedback:** O ciclo *Instrução ➡️ Ação/Edição ➡️ Execução do Linter/Teste ➡️ Feedback do Erro ➡️ Correção*, permitindo que o agente se autoajuste antes da intervenção humana.

---

## 4. Prática e Evidência Esperada

* **Ambiente de referência delimitado:** Workspace local com IDE agêntica configurada, Git e suporte a subagentes/ferramentas locais.
* **Caso didático:** Criação de um ambiente de desenvolvimento isolado para um projeto com `AGENTS.md`, regras de linting, um servidor MCP e uma branch de trabalho dedicada via *worktree*.
* **Evidência esperada:** Demonstração prática de um agente recebendo uma tarefa delimitada, executando a alteração em uma *worktree* separada, rodando o linter automaticamente em background e submetendo a entrega pronta para validação humana.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtro em destaque:** *Filtro de Contenção de Contexto e Escopo*.
* **Pergunta de auditoria rápida:** "O agente tem acesso apenas aos arquivos estritamente necessários para a tarefa? O workspace está protegido contra alterações destrutivas acidentais fora da branch de trabalho?"

---

## 6. Fontes Primárias de Referência

1. **Anthropic Model Context Protocol (MCP) Specification:** Padrão aberto para integração segura de ferramentas e recursos a assistentes de IA ([modelcontextprotocol.io](https://modelcontextprotocol.io)).
2. **Git Documentation — Worktrees:** Gerenciamento de múltiplos diretórios de trabalho vinculados ao mesmo repositório ([git-scm.com/docs/git-worktree](https://git-scm.com/docs/git-worktree)).
3. **The Anatomy of an Agent Harness:** Princípios de injeção de contexto, ferramentas e loops autônomos em engenharia agêntica.

