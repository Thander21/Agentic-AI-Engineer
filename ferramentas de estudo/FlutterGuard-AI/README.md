# FlutterGuard AI
### Autonomous Reactive & Blocking Quality Harness for Flutter / Dart

> **Transformando IA de geradora complacente de código em engenheiro de software sênior determinístico através de Spec-Driven Development (SDD), Análise Reativa de AST, Verificação Visual Multimodal e Gates Bloqueantes.**

---

## 🎯 O Que é o Projeto?
O **FlutterGuard AI** é um framework e orquestrador autônomo (*closed-loop agentic harness*) desenvolvido especificamente para o ecossistema **Flutter/Dart**. Ele resolve o maior gargalo atual do desenvolvimento com IA: a geração de código frágil, poluição de ciclo de vida de widgets, descolamento de estado (*state anti-patterns*), falhas silenciosas de concorrência e quebras visuais (`RenderFlex overflowed`) que linters tradicionais não conseguem detectar.

O projeto funciona como uma barreira física e pedagógica (*fail-closed*): nenhum código gerado por IA é aprovado sem antes passar por um contrato estrito de especificação, validação estática de AST, testes com telemetria determinística e inspeção visual automatizada.

---

## 🚀 Trilhas de Execução (Modulares e Desacopladas)

O projeto foi desenhado com arquitetura de LLM/Model agnóstica:

1. **[Trilha 1: Meta Muse Hackathon](docs/META_HACKATHON_TRACK.md)**  
   * Arquitetura especializada para submissão no Hackathon Global da Meta.
   * Modelos: **Meta Muse Spark** (Arquiteto SDD), **Meta Muse Code** (Worker), **SAM 3.1 & Meta Muse Image** (Auditor Visual de UI/Layout).
2. **[Trilha 2: Local & Multi-Agent (Gemini / Claude Code)](docs/LOCAL_AGENTS_TRACK.md)**  
   * Arquitetura autônoma para rodar no ambiente local integrado com **Gemini CLI, Claude Code, Antigravity ou modelos locais (Ollama/Llama 3)**.
   * Utiliza CLI local, AST analyzer em Dart e headless test runner.

---

## 📚 Mapa da Documentação

* 📖 **[Visão Geral e Problema](docs/PROJECT_OVERVIEW.md):** Diagnóstico de mercado, dores reais e proposta de valor.
* 🏛️ **[Arquitetura do Sistema](docs/ARCHITECTURE.md):** Fluxo reativo, AST Engine, loops de feedback e injeção cirúrgica de contexto.
* 🛡️ **[Campo de Força & Gates](docs/methodology/CAMPO_DE_FORCA_HARNESS.md):** Princípios da esteira determinística e bloqueio *fail-closed*.
* 🔄 **[Metodologia SDD + TDD + BDD + XP](docs/methodology/SPEC_DRIVEN_DEVELOPMENT.md):** O ciclo de vida que elimina alucinações e respostas complacentes.
* 💡 **[Catálogo de Receitas Canônicas](docs/methodology/CANONICAL_RECIPES_CATALOG.md):** Biblioteca de padrões de correção (*Before/After*) para auto-recuperação da IA.
* 🔗 **[Ponte de Referência ERP PDV D+](docs/REFERENCE_PDVDMAIS.md):** Mapeamento e consulta das regras reais testadas em produção no PDV D+.

---

## ⚡ Pilares Fundamentais

1. **Reativo:** Monitora a AST e as mutações de código no instante em que ocorrem.
2. **Bloqueante (*Fail-Closed*):** Código não aprovado em 100% dos gates é sumariamente revertido.
3. **Didático / Pedagógico:** Não apenas aponta o erro, mas injeta a receita canônica (*Just-in-Time Canonical Recipe*) para a IA corrigir em 1 turno.
4. **Multimodal:** Não confia apenas em texto e compiladores; inspeciona a tela renderizada contra quebras de layout.
