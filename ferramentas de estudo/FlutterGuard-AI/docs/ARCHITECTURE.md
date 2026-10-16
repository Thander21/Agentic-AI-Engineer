# Arquitetura do Sistema: FlutterGuard AI

## 1. Visão Arquitetural

O FlutterGuard AI é projetado como uma esteira autônoma e reativa composta por quatro subsistemas orquestrados:

```
┌────────────────────────────────────────────────────────────────────────┐
│                       ORQUESTRADOR DE HARNESS                          │
│                                                                        │
│  1. SPECIFICATION PHASE (SDD)                                          │
│     Requisito do Desenvolvedor -> Especificação -> Contratos & Test RED│
│                                                                        │
│  2. IMPLEMENTATION PHASE (Code Generation)                             │
│     Implementação Mínima Guiada por Contratos e Tipos Estritos         │
│                                                                        │
│  3. DETERMINISTIC EXECUTION GATE (AST & Test Harness)                  │
│     Dart Analyzer (Fatal Infos) + AST Inspector + flutter test         │
│                                                                        │
│  4. MULTIMODAL VISUAL GATE (Headless Rendering & Segmentation)         │
│     WidgetTester Headless Snapshot -> Bounding Box & Margin Analysis    │
│                                                                        │
│  5. FEEDBACK & AUTO-HEALING LOOP (Just-in-Time Canonical Recipes)      │
│     Injeção cirúrgica de receita Before/After em caso de falha         │
└────────────────────────────────────────────────────────────────────────┘
```

---

## 2. Subsistemas Detalhados

### 2.1. Spec-Driven Development Engine (SDD Engine)
* **Objetivo:** Impedir que o modelo de IA comece escrevendo a tela ou o código final.
* **Mecanismo:** 
  1. A IA arquiteta quebra o problema em **Contratos de Dados** (Entities/DTOs imutáveis) e **Máquinas de Estado** (sealed classes exaustivas).
  2. É gerada uma suíte de testes unitários que falham intencionalmente (**Fase RED**).
  3. A esteira grava o estado inicial no log de telemetria `evidence.jsonl`.

### 2.2. AST & Static Governance Inspector (Dart Analyzer Harness)
* **Objetivo:** Auditar a árvore de sintaxe abstrata (AST) do Dart antes e durante a execução.
* **Mecanismo:**
  * Uso do pacote oficial `analyzer` do Dart SDK para percorrer nós do código.
  * Validação de camadas arquiteturais: proíbe classes de UI acessarem bancos de dados ou serviços remotos diretamente.
  * Detecção de anti-patterns de estado: acusa criação de controllers e listeners no corpo do método `build()`.
  * Flags do compilador: execução com `dart analyze --fatal-infos` (zero warnings tolerados).

### 2.3. Deterministic Test Harness (Loop Red/Green)
* **Objetivo:** Garantir que o código novo cumpra 100% dos requisitos sem regressão de código legado.
* **Mecanismo:**
  * Execução local de `flutter test` de forma isolada.
  * Se o teste falhar, o stack trace exato e a asserção violada são capturados de forma estruturada (JSON) para alimentar a fase de auto-correção.

### 2.4. Multimodal Visual Inspector (Segmentação de UI)
* **Objetivo:** Identificar regressões de layout, sobreposições e problemas de `RenderFlex overflowed`.
* **Mecanismo:**
  * O teste de widget monta a tela em modo headless usando `WidgetTester.pumpWidget()` e renderiza o layout sob restrições extremas de resolução (ex.: 800×600, proporção tablet e mobile).
  * O frame é exportado como imagem PNG.
  * O modelo de visão/segmentação processa os componentes visuais, calculando o espaçamento entre elementos e identificando cortes de texto ou overflow de pixels.

### 2.5. Feedback & Auto-Healing Loop (Receitas Canônicas)
* **Objetivo:** Fazer o agente convergir em 1 ou 2 turnos sem tentar adivinhar a correção.
* **Mecanismo:**
  * Cada erro emitido pelo AST Inspector ou pelo Test Harness possui um código único (ex.: `FG-ST-001`, `FG-LAY-004`).
  * O orquestrador busca na biblioteca local a **Receita Canônica** correspondente.
  * A receita contém a explicação da causa raiz, o padrão proibido (*Before*) e a solução canônica (*After*).
  * O agente recebe apenas esse contexto cirúrgico e reescreve exclusivamente o bloco defeituoso.

---

## 3. Modelo de Dados de Telemetria (`evidence.jsonl`)

Cada ciclo executado pelo framework registra um evento atômico estruturado para garantir rastreabilidade completa:

```json
{
  "timestamp": "2026-10-14T20:30:00Z",
  "phase": "DETERMINISTIC_GATE",
  "rule_id": "FG-ST-001",
  "file": "lib/features/cart/presentation/cart_page.dart",
  "status": "FAILED",
  "error_message": "ScrollController instantiated inside build() method",
  "recipe_injected": "RECIPE_DISPOSE_SAFE_CONTROLLER",
  "iteration": 1,
  "action": "AUTO_HEALING_DISPATCHED"
}
```
