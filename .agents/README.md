# Hub de Agentes e Skills (.agents)

Este diretório contém as skills, regras e definições de agentes que conectam o assistente de IA (Antigravity) ao framework de orquestração **Synkra AIOX**.

---

## 1. Agentes Disponíveis

| Agente | Persona | Arquétipo / Função | Ponto de Entrada |
| :--- | :--- | :--- | :--- |
| **`editorial`** | **Scribe** | Senior Technical Writer & Wordsmith (Capítulos, Artigos, 4 Pilares de Qualidade) | [`skills/editorial/SKILL.md`](skills/editorial/SKILL.md) |
| **`aiox-master`** | **Master** | Orquestrador Central do Framework AIOX | [`skills/aiox-master/SKILL.md`](skills/aiox-master/SKILL.md) |
| **`po`** | **Pax** | Product Owner (Definição de Histórias e Critérios de Aceite) | [`skills/po/SKILL.md`](skills/po/SKILL.md) |
| **`dev`** | **Dex** | Full Stack Developer (Implementação de código) | [`skills/dev/SKILL.md`](skills/dev/SKILL.md) |
| **`qa`** | **Quinn** | Quality Assurance Specialist (Quality Gates e Testes) | [`skills/qa/SKILL.md`](skills/qa/SKILL.md) |
| **`architect`** | **Aria** | Software & Systems Architect | [`skills/architect/SKILL.md`](skills/architect/SKILL.md) |
| **`pm`** | **Morgan** | Project Manager (Visão e Cronograma) | [`skills/pm/SKILL.md`](skills/pm/SKILL.md) |
| **`analyst`** | **Atlas** | Business & Domain Analyst | [`skills/analyst/SKILL.md`](skills/analyst/SKILL.md) |
| **`sm`** | **River** | Scrum Master & Agile Facilitator | [`skills/sm/SKILL.md`](skills/sm/SKILL.md) |

---

## 2. Squads Especializados (.aiox-squads)

Módulos temáticos integrados ao ecossistema para impulsionar a escrita técnica e a autoridade:

### A. Para o Registro de Autoridade e Artigos (`.aiox-squads/autoridade/`)
| Squad | Orquestrador | Mentes de Referência | Finalidade no Projeto | Ponto de Entrada |
| :--- | :--- | :--- | :--- | :--- |
| **`brand`** | `brand-chief` | April Dunford, Marty Neumeier, Alexandra Watkins | Estratégia de posicionamento, autoridade profissional e diferenciação | [`skills/brand/SKILL.md`](skills/brand/SKILL.md) |
| **`curator`** | `curator-chief` | Robert McKee, Matthew Dicks, Jonah Berger | Mineração e decupagem de vivências reais sem inventar fatos | [`skills/curator/SKILL.md`](skills/curator/SKILL.md) |

### B. Para os Capítulos de Estudo e o Livro (`.aiox-squads/estudos/`)
| Squad | Orquestrador | Mentes de Referência | Finalidade no Projeto | Ponto de Entrada |
| :--- | :--- | :--- | :--- | :--- |
| **`education`** | `education-chief` | Wiggins, Sweller, Bloom, Merrill, Rosenshine | Design instrucional, otimização de carga cognitiva e progressão didática | [`skills/education/SKILL.md`](skills/education/SKILL.md) |
| **`deep-research`** | `dr-orchestrator` | Kahneman, Booth, Sackett, Forsgren | Pesquisa técnica primária, evidências e auditoria de viés | [`skills/deep-research/SKILL.md`](skills/deep-research/SKILL.md) |
| **`dispatch`** | `dispatch-chief` | Gene Kim, Deming, Goldratt | Execução em DAGs e arquitetura prática de agentes com subagentes | [`skills/dispatch/SKILL.md`](skills/dispatch/SKILL.md) |

---

## 3. Como Funciona a Orquestração

1. **Dual-Track AIOX:** O sistema opera em duas vias de entrega contínua:
   - **Engenharia de Software:** Histórias técnicas implementadas pelo `@dev` e validadas pelo `@qa`.
   - **Engenharia Editorial & Conteúdo:** Histórias de escrita implementadas pelo `@editorial` (Scribe) e auto-revisadas contra a **Matriz dos 4 Pilares** (Fatos, Didática, Voz e Norma).
2. **Soberania do Autor:** Toda entrega editorial tem como estágio final a leitura autoral humana para confirmação de tom de voz e aprovação de publicação.
3. **Diretrizes Globais:** Consulte [`../AGENTS.md`](../AGENTS.md) para regras de preservação, privacidade e fontes.
