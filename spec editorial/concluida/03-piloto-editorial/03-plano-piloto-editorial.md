# Plano 03 — Piloto editorial

**ID:** PLANO-EDITORIAL-003. **Versão:** 0.9 — 18/10/2026.
**Base:** [spec 03 v1.7](03-piloto-editorial.md), preparação 02 recebida e [guia vigente](../../GUIA_DE_OPERACAO.md). **Acompanhamento:** [tasks 03](03-tasks-piloto-editorial.md).

## Entregas, sequência e conferência

Base de caminhos: raiz. Pasta das peças: `registro da autoridade/publicacoes/01-novo-mundo-bagagem-antiga/`. Caminhos ainda sem arquivo são previstos.

| Entrega / origem | Resultado e local | Dependência / critério |
| --- | --- | --- |
| ENT03-01 / T01-018 | Ficha `ficha-editorial.md` e fontes identificadas | Preparação 02; contexto suficiente, lacunas/limites e referência recuperável das fontes. Já produzida; estado nas tasks. |
| ENT03-02 / T01-019 | Esboço `esboco.md` e artigo `artigo.md` | Ficha; primeiro rascunho fiel ao recorte e à atribuição de relatos. Já produzidos, sem aprovação presumida. |
| ENT03-03 / T01-019 | Ficha curta vinculada e `chamada-linkedin.md`, ID distinto | Artigo apreciado pelo autor; reconferir chamada existente após estabilização do artigo, com promessa e ligação fiéis, sem URL inventada. Ficha curta pode integrar a pasta da peça sem sobrescrever a base r01 do artigo. |
| ENT03-04 / T01-019 | Pareceres/decisões proporcionais em `revisao-e-integracao.md` e versões integradas | Por peça, primeiro artigo e depois chamada conforme RA03-03; estrutura/fatos/voz antes de acabamento, achados resolvidos/justificados e reconferência. Saída pronta para leitura autoral, sem prova final antecipada. |
| ENT03-05 / T01-020 / PEN-03 | Retorno do autor, ajustes autorizados e reconferência | Versão identificada de ENT03-04 e retorno real, primeiro artigo; somente depois retomar chamada e sua apreciação. Sem resposta não concluir. |
| ENT03-09 / T01-019 | Prova final registrada no acompanhamento da peça | ENT03-05; língua, títulos, links, resíduos e integridade da versão resultante. Mudança substancial volta à etapa responsável. |
| ENT03-06 / T01-021 | Avaliação aplicada nas tasks | Entregas editoriais e retorno/prova; ganhos/perdas, esforço observado e decisões de simplificar/manter/ajustar, com cobertura não exercitada individualizada. |

ENT03-07/T03-007 e ENT03-08/T03-008 são entregas históricas de organização já ocorridas; conservar origem/evidências, sem duplicar sua execução ou reabri-las por atualização de procedimento. 05 responde pela correção atual do método.

## Contexto e procedimentos

Usar preparar para ficha completa do artigo e breve da chamada; redigir para esboço/rascunho; revisar perfis pertinentes; integrar para alterações autorizadas; reconferir versão nova; receber leitura do autor; ajustar e provar. Não impor nove documentos. P03 trata apenas conceitos presentes, P04 recorte e relação entre peças; P08 é impressão situada da IA, com apreciação real reservada ao autor.

D05-01 governa preservação antes da edição de texto; não substituir versão comparável sem recuperação, criar backup ou executar commit. Fonte factual ausente volta à preparação/autor; mudança de intenção à spec. Reaproveitar contexto/ficha/esboço e exercícios EX02-A/B no alcance existente; modo novo ou refatoração substancial sem cobertura exige exame dirigido antes do uso.

## Cobertura planejada

| Requisitos herdados de 01 | Entregas / evidência adequada |
| --- | --- |
| REQ-01/02/03 | ENT03-01/02/04: leitor/contribuição, afirmações-fontes e natureza de fato/metáfora. |
| REQ-04/16 | ENT03-04/05: voz/interesse com trechos e retorno autoral, sem reconhecimento humano pela IA. |
| REQ-05/07 | ENT03-01/03/04: origem única, continuidade e vínculo entre peças/estudos sem capítulo obrigatório. |
| REQ-06/11 | ENT03-04: parecer por versão/contexto e especialidade pertinente. |
| REQ-08/12 | ENT03-01/04/06: proporção, estrutura antes do acabamento e esforço observado. |
| REQ-09 | ENT03-04/05/06: impacto e encaminhamento da mudança. |
| REQ-10/13/15 | ENT03-04/05/09: estados separados, língua/voz, decisões e encerramento. |
| REQ-14 | ENT03-04/06: comparação com sentido preservado e mudança que exige reconsiderar a spec, ou cobertura ausente/destino. |
| REQ-17/18/19/20 | ENT03-06: spec, plano e tasks distintos, conferência pertinente e resultados no acompanhamento. |

**Parecer v0.4:** apto ao acompanhamento, mesma IA com histórico. Sequência e critérios reconciliados com spec v1.0/guia 1.0, incluindo ENT03-09/T03-009. Cobertura planejada não demonstra eficácia ou texto aprovado. Dependência de método satisfeita em T05-004 em 17/10/2026; produção seguinte respeita o escopo autorizado para o piloto.

**Ajuste v0.5 — RA03-03:** execução por peça: artigo → revisão → autor/ajustes → retomada da chamada → revisão → autor/ajustes → provas/avaliação. T03-004/005 podem permanecer em execução enquanto uma peça aguarda retorno; não exigir as duas prontas para apreciar o artigo. Conferida ausência de ciclo nessa passagem. Dispensada preservação via commit da versão de trabalho nesta reescrita, por autorização explícita; demais limites de fontes e publicação mantidos.

**Ajuste v0.6 — RA03-04:** revisar preparação/esboço e artigo pelo ponto de vista retrospectivo: presente após dez meses → origem e percurso → fundamentos para próxima etapa. Mesmas entregas/IDs e sequência por peça; chamada continua dependente do artigo apreciado. Critério adicional: distinguir uso já iniciado de IA/harnesses/SDD de aprofundamento futuro, com nível/ermitão como metáforas.

**Ajuste v0.7 — RA03-05:** mesmas entregas e dependências; conferir marco dos dez meses como projeto grande, uso anterior de IA e material já levantado ainda a publicar. Após a conquista em homologação, ligar aprofundamento às responsabilidades percebidas para uso real, sem transformar o relato em instrução fiscal ou garantia técnica.

**Ajuste v0.8 — RA03-06:** reabrir preparação/redação e revisão da chamada. Equipe autorizada: proposta de redação, parecer de gancho/voz e integração pela coordenadora. Chamada como unidade autônoma de tensão/contexto/convite, sem resumo do percurso. Mesmos arquivos e IDs; artigo preservado. Entrega da versão integrada ao autor, prova após retorno.


**Conferência de encerramento v0.9 — 18/10/2026:** mesmas entregas e dependências, sem ciclo; ENT03-01–06/09 e entregas históricas 07/08 têm resultado nas tasks. A matriz T03-006 cobre individualmente REQ-01–20, ganhos/perdas e limites dos dois casos de alteração; cobertura ausente recebe destino condicionado, sem iniciar nova produção. Contrato/base reconciliados com spec v1.7 e guia v1.3; peças e publicação não alteradas por esta conferência.
