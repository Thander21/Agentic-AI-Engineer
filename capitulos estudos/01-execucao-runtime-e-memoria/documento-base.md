# Documento Base — CAP-01: Execução, runtime e memória

**ID:** CAP-01  
**Parte:** I — Computação e Runtime  
**Estado:** Preparação conferida — estudo a iniciar  
**Ficha editorial correspondente:** [ficha-editorial.md](ficha-editorial.md)

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Quando uma função chama outra e cria um objeto, o que precisamos compreender sobre execução, stack, heap e gerenciamento de memória para explicar a vida desse objeto e os limites dessa explicação?
* **Objetivo de estudo:** Compreender como a máquina física e o runtime executam instruções de software, alocam dados na memória (pilha de execução vs. heap) e liberam recursos (garbage collection / desalocação), relacionando essa base física ao código gerado por agentes de IA.

---

## 2. O Papel do Engenheiro Agêntico

* **Por que a IA não substitui esse conhecimento:** Agentes geram código sintaticamente válido, mas são cegos ao consumo físico de recursos. Uma IA pode facilmente criar referências estáticas circulares que retêm gigabytes no heap, instanciar objetos pesados dentro de loops críticos ou ignorar o ciclo de vida do runtime.
* **Decisões sob responsabilidade do engenheiro:**
  * Identificar se objetos temporários estão sendo liberados ou retidos indevidamente no heap.
  * Avaliar se variáveis locais estão limitadas ao seu quadro de pilha (*stack frame*) ou se estão escapando para o heap.
  * Reconhecer o comportamento do Garbage Collector e saber quando uma lentidão no sistema é causada por pausas de coleta e pressão de memória.

---

## 3. Conceitos-Chave e Pré-requisitos

* **Pré-requisitos:** Leitura básica de fluxo sequencial, condicionais, funções e chamadas. Nenhum capítulo anterior é exigido.
* **Tópicos essenciais:**
  * Papel do Runtime: máquina virtual, compilação JIT vs. AOT, interpretador.
  * Stack (Pilha de Execução): chamadas de função, quadros de ativação (*stack frames*), escopo de variáveis locais e retorno.
  * Heap (Área Livre de Alocação): alocação dinâmica de objetos, ponteiros e referências.
  * Gerenciamento de Memória: ciclo de vida de objetos, raiz de retenção (*root objects*), alcançabilidade e coleta de lixo (*Garbage Collection*).
  * Limites de observação: a diferença entre o modelo mental conceitual e a alocação física real realizada pelo compilador/SO.

---

## 4. Prática e Evidência Esperada

* **Ambiente de referência delimitado:** Dart no desktop.
* **Caso didático:** Fluxo síncrono enxuto de chamadas, condicional e retorno, com instanciação de um objeto simples para rastrear sua criação e referência.
* **Evidência esperada:** Fluxo comentado passo a passo demonstrando a abertura/fechamento dos quadros de pilha na stack e a alocação do objeto no heap, com demarcação clara do ponto em que o objeto deixa de ser alcançável.

---

## 5. Aplicação dos Filtros de Leitura Diagnóstica

* **Filtro em destaque:** *Filtro 2 (Efeitos Colaterais e Recursos)* e *Filtro 5 (Inspeção Viva)*.
* **Pergunta de auditoria rápida:** "Onde as variáveis deste método estão sendo criadas? Alguma referência viva permanece apontando para este objeto após o encerramento do método, impedindo o coletor de atuar?"

---

## 6. Fontes Primárias de Referência

1. **Dart Overview:** Plataformas, compilação nativa e responsabilidades do Dart Runtime ([dart.dev/overview](https://dart.dev/overview)).
2. **Flutter/Dart DevTools Memory:** Conceitos fundamentais de memória, objetos raiz, caminhos de retenção e alcançabilidade ([docs.flutter.dev/tools/devtools/memory](https://docs.flutter.dev/tools/devtools/memory)).
3. **Dart Functions & Debugger:** Execução de funções, main, call stack e quadros de inspeção ([dart.dev/language/functions](https://dart.dev/language/functions)).

