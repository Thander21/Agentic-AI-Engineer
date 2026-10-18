---
name: sdd-editorial-tarefas
description: Decompõe um plano editorial conferido e acompanha estado, artefatos, critérios, evidências e pendências numa tabela atual. Use para organizar ou conferir execução; não define intenção nem substitui as skills de produção.
metadata:
  version: "0.2"
---

# Organizar e acompanhar tasks editoriais

## Entrada e modos

Receber pedido/limite, spec e plano identificados, parecer do plano e artefatos existentes. Modos: decompor, acompanhar ou conferir acompanhamento. Listar/revisar tasks não inicia produção sem autorização. Consultar [guia](../../GUIA_DE_OPERACAO.md) e [modelo de tasks](../../modelos/tasks.md) conforme necessidade.

## Decompor

Uma task tem ID estável, entrega/requisitos, dependências, resultado/caminho previsto e critério de conclusão. Agrupar atividades com a mesma saída/critério; separar retorno autoral e prova final quando suas condições diferirem. Não criar task por vírgula, nove perfis ou arquivo de registro.

Conferir cobertura das entregas, dependências sem ciclos e fase/skill necessária. Não introduzir requisito: intenção volta à spec, estratégia ao plano. Antes de executar, conferir consistência spec → plano → tasks no próprio acompanhamento, sem outro documento.

## Acompanhar numa fonte atual

| Estado | Uso |
| --- | --- |
| Pendente | Não iniciado, inclusive por dependência futura. |
| Em execução | A atividade efetivamente começou. |
| Produzida/aguardando conferência | Saída existe; critério ainda não atendido/conferido integralmente. |
| Concluída | Resultado e critério conferidos com evidência suficiente, sem impeditivo aberto. |
| Bloqueada com motivo | Tentativa encontrou impedimento concreto; registrar parte afetada e condição de retomada. |

A tabela única concentra ID, estado, artefato/revisão, critério/evidência e pendência/próxima ação. Explicação adicional apenas quando necessária para interpretar decisão, correção ou reabertura; não repetir base, alterações de arquivos e negativas a cada rodada. Git preserva versões, não criar diário de sessão ou histórico duplicado.

## Conferir e retornar

Não concluir por arquivo existente ou marcação antiga. Distinguir produção, estrutura conferida, procedimento exercitado, retorno humano e publicação. Registrar só o observado, com contexto/limite; não inventar tempo, aprovação ou independência. Uma task pode concluir o rascunho sem concluir a revisão da peça; deixar a próxima condição explícita.

Mudança que invalide evidência reabre somente o aspecto afetado e examina dependentes. Manter IDs e referência ao resultado anterior. Sem retorno do autor, a entrega humana permanece pendente; prova final da peça vem depois do retorno e ajustes. Impeditivo não é transferido para aparentar conclusão.

Próxima ação deve ser inequívoca. Com execução autorizada, continuar até a entrega combinada/dependência real, sem pedir “continue” por task. Solicitar commit apenas no ponto de preservação de texto definido pelo guia; continuar partes independentes.
