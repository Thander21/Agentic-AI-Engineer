# Documento Base — CAP-10: Execução, runtime e memória

**ID:** CAP-10  
**Parte:** V — Computação e Runtime  
**Estado:** Preparação conferida — estudo a iniciar  
**Ficha editorial correspondente:** [ficha-editorial.md](ficha-editorial.md)

---

## 1. Pergunta Central e Objetivo de Estudo

* **Pergunta norteadora:** Quando uma funÃ§Ã£o chama outra e cria um objeto, o que precisamos compreender sobre execuÃ§Ã£o, stack, heap e gerenciamento de memÃ³ria para explicar a vida desse objeto e os limites dessa explicaÃ§Ã£o?
* **Objetivo de estudo:** Compreender como a mÃ¡quina fÃ­sica e o runtime executam instruÃ§Ãµes de software, alocam dados na memÃ³ria (pilha de execuÃ§Ã£o vs. heap) e liberam recursos (garbage collection / desalocaÃ§Ã£o), relacionando essa base fÃ­sica ao cÃ³digo gerado por agentes de IA.

---

## 2. O Papel do Engenheiro AgÃªntico

* **Por que a IA nÃ£o substitui esse conhecimento:** Agentes geram cÃ³digo sintaticamente vÃ¡lido, mas sÃ£o cegos ao consumo fÃ­sico de recursos. Uma IA pode facilmente criar referÃªncias estÃ¡ticas circulares que retÃªm gigabytes no heap, instanciar objetos pesados dentro de loops crÃ­ticos ou ignorar o ciclo de vida do runtime.
* **DecisÃµes sob responsabilidade do engenheiro:**
  * Identificar se objetos temporÃ¡rios estÃ£o sendo liberados ou retidos indevidamente no heap.
  * Avaliar se variÃ¡veis locais estÃ£o limitadas ao seu quadro de pilha (*stack frame*) ou se estÃ£o escapando para o heap.
  * Reconhecer o comportamento do Garbage Collector e saber quando uma lentidÃ£o no sistema Ã© causada por pausas de coleta e pressÃ£o de memÃ³ria.

---

## 3. Conceitos-Chave e PrÃ©-requisitos

* **PrÃ©-requisitos:** Leitura bÃ¡sica de fluxo sequencial, condicionais, funÃ§Ãµes e chamadas. Nenhum capÃ­tulo anterior Ã© exigido.
* **TÃ³picos essenciais:**
  * Papel do Runtime: mÃ¡quina virtual, compilaÃ§Ã£o JIT vs. AOT, interpretador.
  * Stack (Pilha de ExecuÃ§Ã£o): chamadas de funÃ§Ã£o, quadros de ativaÃ§Ã£o (*stack frames*), escopo de variÃ¡veis locais e retorno.
  * Heap (Ãrea Livre de AlocaÃ§Ã£o): alocaÃ§Ã£o dinÃ¢mica de objetos, ponteiros e referÃªncias.
  * Gerenciamento de MemÃ³ria: ciclo de vida de objetos, raiz de retenÃ§Ã£o (*root objects*), alcanÃ§abilidade e coleta de lixo (*Garbage Collection*).
  * Limites de observaÃ§Ã£o: a diferenÃ§a entre o modelo mental conceitual e a alocaÃ§Ã£o fÃ­sica real realizada pelo compilador/SO.

---

## 4. PrÃ¡tica e EvidÃªncia Esperada

* **Ambiente de referÃªncia delimitado:** Dart no desktop.
* **Caso didÃ¡tico:** Fluxo sÃ­ncrono enxuto de chamadas, condicional e retorno, com instanciaÃ§Ã£o de um objeto simples para rastrear sua criaÃ§Ã£o e referÃªncia.
* **EvidÃªncia esperada:** Fluxo comentado passo a passo demonstrando a abertura/fechamento dos quadros de pilha na stack e a alocaÃ§Ã£o do objeto no heap, com demarcaÃ§Ã£o clara do ponto em que o objeto deixa de ser alcanÃ§Ã¡vel.

---

## 5. AplicaÃ§Ã£o dos Filtros de Leitura DiagnÃ³stica

* **Filtro em destaque:** *Filtro 2 (Efeitos Colaterais e Recursos)* e *Filtro 5 (InspeÃ§Ã£o Viva)*.
* **Pergunta de auditoria rÃ¡pida:** "Onde as variÃ¡veis deste mÃ©todo estÃ£o sendo criadas? Alguma referÃªncia viva permanece apontando para este objeto apÃ³s o encerramento do mÃ©todo, impedindo o coletor de atuar?"

---

## 6. Fontes PrimÃ¡rias de ReferÃªncia

1. **Dart Overview:** Plataformas, compilaÃ§Ã£o nativa e responsabilidades do Dart Runtime ([dart.dev/overview](https://dart.dev/overview)).
2. **Flutter/Dart DevTools Memory:** Conceitos fundamentais de memÃ³ria, objetos raiz, caminhos de retenÃ§Ã£o e alcanÃ§abilidade ([docs.flutter.dev/tools/devtools/memory](https://docs.flutter.dev/tools/devtools/memory)).
3. **Dart Functions & Debugger:** ExecuÃ§Ã£o de funÃ§Ãµes, main, call stack e quadros de inspeÃ§Ã£o ([dart.dev/language/functions](https://dart.dev/language/functions)).

