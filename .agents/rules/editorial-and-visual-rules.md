# Diretrizes Editoriais e Visuais do Projeto

Esta regra estende as diretrizes do `AGENTS.md` e do agente `editorial` do AIOX.

## 1. Chamadas de Redes Sociais (LinkedIn)
- **Nunca resumir:** Arquivos `chamada-linkedin.md` jamais devem ser resumos, sinopses executivas ou listas ponto a ponto dos fatos do artigo.
- **Texto independente e magnético:** Construa uma reflexão autoral original sobre a dor prática, o paradoxo ou o choque de realidade enfrentado, gerando curiosidade visceral para direcionar o leitor ao artigo completo via CTA claro.

## 2. Direção de Arte e Prompts de Imagem
- **Universo Estético:** Exclusivamente **Fantasia Medieval RPG / Isekai ("Reencarnei no Reino dos Agentes")**. É expressamente proibido gerar estéticas sci-fi, cyberpunk, neon ou futuristas.
- **Metáforas do Mundo Medieval:**
  - Código/Sistemas -> Grimórios ancestrais, runas de poder, pergaminhos com selos de cera reais.
  - Testes/Harness/Pipelines -> Forjas de ferreiro místico, rédeas de ferro, barreiras rúnicas e campos de força mágicos.
  - Masmorra -> Ambiente de pedra bruta, tochas de parede e brasas incandescentes.
- **Consistência do Protagonista (Image-to-Image / Prompt Reference):**
  - Manter sempre os atributos visuais do mesmo protagonista estabelecido nos episódios anteriores (mesmo corte de cabelo, traços faciais, manto/túnica de artesão-mago de couro rústico e detalhes característicos).
  - Incluir explicitamente instruções de consistência e parâmetros de referência (`--cref`, `character reference`, ou descrição âncora idêntica).
- **Formatos:**
  - **Capa do Artigo (Hero Image):** Proporção 16:9 (`--ar 16:9`).
  - **Stub / Open Graph do LinkedIn:** Proporção 1.91:1 / 1200:630 (`--ar 1200:630`), composição centralizada, alto contraste para telas mobile e sem poluição de microtextos.
