# 10. Texto anexo — A provação do código

[Etapa da jornada](10-a-provacao-do-codigo.md) · [Índice](README.md) · [Mapa de origem](MAPA_ORIGEM.md)

Este anexo reúne 23 trechos: 20 principais e 3 cópias relacionadas. A organização abaixo identifica o que a conversa já oferece e o que ainda precisa ser aprofundado.

As sínteses são uma leitura editorial do material. Os blocos identificados como fonte preservam literalmente perguntas, respostas, exemplos e versões anteriores; sugestões da outra IA não passam a ser decisões aprovadas ou resultados comprovados por estarem neste anexo.

## Mapa de aprofundamento

| Assunto | O que já temos | O que aprofundar |
| --- | --- | --- |
| [A dificuldade de ler sem anos de programação](#assunto-01) | Você expõe a dificuldade; a IA responde com lacunas de leitura, riscos e analogias sobre reconhecimento. | Desenhar prática de leitura e diagnóstico e avaliar o que as analogias deixam sem resposta. |
| [As versões dos cinco filtros](#assunto-02) | Os filtros aparecem em uma explicação inicial, no blueprint e na sequência de estudos. | Consolidar um protocolo de triagem com alcance e limites explícitos, sem pressupor suficiência ou tempo universal. |
| [Exemplo completo para examinar](#assunto-03) | O caso da fatura inclui spec, implementação, diagnóstico, teste e logs. | Reavaliar os diagnósticos e as correções propostas antes de transformar o caso em exercício validado. |
| [Testes, propriedades e verificação](#assunto-04) | A conversa reúne BDD, propriedades, mutação e verificação e validação. | Definir testes que discriminem comportamento correto e incorreto e revisar as alegações de prova matemática. |
| [Métricas e auditoria estática](#assunto-05) | Há sugestões de métricas de complexidade, acoplamento e análise estática. | Examinar contexto, limitações e critérios de interpretação das métricas antes de automatizar decisões. |
| [Experimentação e alcance das conclusões](#assunto-06) | Laboratórios de falha e conclusões sobre o exercício são apresentados como meios de desenvolver julgamento. | Separar a detecção de um problema num exemplo da capacidade de auditar um sistema completo. |

## Texto de referência por assunto

<a id="assunto-01"></a>

### 1. A dificuldade de ler sem anos de programação

**O que já temos:** Você expõe a dificuldade; a IA responde com lacunas de leitura, riscos e analogias sobre reconhecimento.

**Para aprofundar:** Desenhar prática de leitura e diagnóstico e avaliar o que as analogias deixam sem resposta.

<a id="fonte-f041"></a>

#### F041 — Relato pessoal e dúvida sobre aprender a ler código

Origem histórica: conversa original, linhas 662–664. Cópia relacionada para este assunto. Destino principal: [anexo 01](01-texto-anexo.md#fonte-f041).

<!-- FONTE: F041 INICIO -->
> Sim
> Mas nesse caso a conta não fecha, e o mesmo que ensinar alguém a dirigir mostrando como a ia dirige se a pessoa não dirigir não vai saber realmente dirigir, mas se nunca precisar dirigir mas só saber orientar a aí vai chegar onde quer, então como aprender e ler código sem realmente passar anos programando? Eu mesmo não sei ler todo o código mas entendo todos os conceitos por anos de trabalho com tecnologia, sistemas e banco de dados, servidores etc... Como posso aprender a ler o código se não ficar programando ?
> 

<!-- FONTE: F041 FIM -->

<a id="fonte-f034"></a>

#### F034 — Lacuna de leitura e auditoria

Origem histórica: conversa original, linhas 562–579. Trecho principal desta etapa.

<!-- FONTE: F034 INICIO -->
> 1. Literacia de Leitura (Saber Ler Código 
> ≠
> 
> = Saber Digitar Código)
> O Gap: Eliminar a digitação manual de sintaxe não significa eliminar a necessidade de ler e rastrear código fluentemente.
> 
> O Risco na Tomada de Decisão: A IA vai gerar código com bugs sutis de lógica, loops com complexidade assintótica oculta (
> O
> (
> N
> 2
> )
> O(N 
> 2
>  )) ou vazamento de conexões. Se o engenheiro orquestrador não consegue bater o olho em um trecho de código gerado e apontar: "aqui você está abrindo uma transação no banco antes de fazer uma chamada HTTP externa", a spec falha na implementação.
> 
> O que falta: Treinamento deliberado em Auditoria e Leitura Crítica de Código, focado em fluxo de controle, variáveis de escopo e chamadas assíncronas.
> 

<!-- FONTE: F034 FIM -->

<a id="fonte-f039"></a>

#### F039 — Riscos e proposta de leitura diagnóstica

Origem histórica: conversa original, linhas 627–649. Trecho principal desta etapa.

<!-- FONTE: F039 INICIO -->
> 
> O primeiro motivo é o risco dos testes tautológicos. Quando um operador não lê código e pede à IA para "implementar a funcionalidade e cobrir com testes", o agente frequentemente cria testes que passam sozinhos. A IA pode mockar o próprio comportamento que deveria testar, validar apenas o que ela mesma escreveu ou criar asserções vazias. Para o operador leigo, a suíte de testes está 100% verde e a especificação parece cumprida, mas em produção o sistema quebra na primeira requisição real. Sem capacidade de auditar o código do teste, você não tem uma rede de segurança, tem apenas um placebo visual.
> 
> O segundo motivo são os defeitos invisíveis à especificação. Uma IA pode implementar perfeitamente a sua regra de negócio de faturamento e, ao mesmo tempo, introduzir uma consulta ao banco dentro de um loop (
> N
> +
> 1
> N+1), segurar uma transação aberta durante uma chamada externa de rede ou vazar memória mantendo referências estáticas. A regra de negócio teórica está impecável, mas o servidor cai com cinquenta clientes simultâneos. Nenhum conceito puramente teórico de alto nível avisa que uma biblioteca externa gerou um gargalo de I/O bloqueante.
> 
> O terceiro motivo é a perda total de soberania sobre o produto. No momento em que um sistema atinge um erro crítico em produção — um deadlock de banco, dados corrompidos por race condition ou um pacote com vulnerabilidade de segurança —, a IA muitas vezes entra em loops de alucinação, tentando corrigir o bug gerando ainda mais código desconexo. Se a pessoa que comanda não sabe abrir os arquivos críticos, inspecionar a árvore de execução e dizer "o problema está nesta linha porque você instanciou essa conexão fora do escopo", ela se torna refém da ferramenta, não uma engenheira.
> 
> Isso não significa, de forma alguma, que o engenheiro precisa continuar digitando código manualmente como no passado. O que muda radicalmente é a natureza da leitura de código.
> 
> Um engenheiro civil não assenta tijolos nem bate concreto, mas ele é obrigado a saber ler uma planta estrutural e calcular a carga da viga. Um diretor financeiro não passa o dia digitando notas fiscais, mas sabe bater o olho em um balanço patrimonial e identificar uma inconsistência contábil em segundos.
> 
> No desenvolvimento orquestrado por IA, o profissional não lê o código como um revisor gramatical lendo um romance página por página. Ele pratica leitura diagnóstica de fronteiras:
> 
> Ele não lê os 500 métodos utilitários gerados, mas lê com lupa as interfaces de contrato e os modelos de domínio.
> 
> Ele inspeciona as consultas geradas ao banco de dados para garantir que índices e transações façam sentido.
> 
> Ele lê as asserções dos testes para garantir que a máquina está sendo testada contra a realidade, e não contra uma ilusão.
> 

<!-- FONTE: F039 FIM -->

<a id="fonte-f042"></a>

#### F042 — Analogias sobre reconhecimento e criação de código

Origem histórica: conversa original, linhas 665–674. Trecho principal desta etapa.

<!-- FONTE: F042 INICIO -->
> A analogia de dirigir é excelente para expor a tensão, mas o código possui uma dinâmica diferente: programar é uma habilidade de síntese (escrever do zero), enquanto auditar é uma habilidade de reconhecimento (leitura crítica).
> 
> Pense em um contrato jurídico ou em uma planta de engenharia:
> 
> Um empresário ou diretor não passa cinco anos redigindo contratos de 60 páginas, mas ele sabe bater o olho nas 3 cláusulas críticas que definem multa rescisória, foro e responsabilidade solidária.
> 
> Um engenheiro clínico não constrói um tomógrafo peça por peça, mas ele sabe interpretar os parâmetros de calibração e os alertas de erro para saber se a máquina é segura para o paciente.
> 
> A sua própria experiência comprova isso: você compreende o funcionamento de sistemas, bancos de dados, servidores e lógica de negócio. Você não precisa passar anos digitando sintaxe para ser capaz de auditar código. Você só precisa aprender a ler por amostragem e fronteiras, e não linha a linha como quem lê um romance.
> 

<!-- FONTE: F042 FIM -->

<a id="assunto-02"></a>

### 2. As versões dos cinco filtros

**O que já temos:** Os filtros aparecem em uma explicação inicial, no blueprint e na sequência de estudos.

**Para aprofundar:** Consolidar um protocolo de triagem com alcance e limites explícitos, sem pressupor suficiência ou tempo universal.

<a id="fonte-f043"></a>

#### F043 — Formulação inicial dos cinco filtros

Origem histórica: conversa original, linhas 675–732. Trecho principal desta etapa.

<!-- FONTE: F043 INICIO -->
> Como Ler e Auditar Código Sem Passar Anos Programando
> Para quem orquestra e especifica, o código gerado pela IA não é lido de cima para baixo. Ele é submetido a cinco filtros de verificação visual rápida:
> 
> [Código Gerado pela IA]
>         │
>         ├─► 1. Contrato: O que entra e o que sai? (Assinaturas)
>         ├─► 2. Invariante: Onde o IF impede a regra de quebrar?
>         ├─► 3. Efeito Colateral: Onde ele toca em Banco, Rede ou Disco?
>         ├─► 4. Rede de Proteção: O teste valida o comportamento ou é farsa?
>         └─► 5. Execução Viva: O dado que passa no log/debugger faz sentido?
> 1. O Filtro de Contrato (Inputs, Outputs e Tipagem)
> Você não precisa ler o corpo da função para saber se ela faz sentido. Leia apenas a assinatura:
> 
> Pergunta de auditor: O que essa função recebe? O que ela devolve?
> 
> Exemplo prático: Se a sua regra fiscal diz que o cálculo precisa do tipo de emitente, da UF de destino e do código NCM, e a função gerada pela IA recebe apenas CalcularImposto(decimal valor), você sabe em 2 segundos — sem ler uma única linha interna — que o código está errado. O contrato não tem os dados necessários para cumprir a regra.
> 
> 2. O Filtro dos Efeitos Colaterais (I/O, Banco e Rede)
> Código puro em memória quase nunca quebra um sistema; o que derruba servidores são operações externas (chamar banco de dados, abrir arquivos, chamar APIs).
> 
> Técnica: Em vez de ler 200 linhas, procure apenas por palavras-chave de chamada externa (SELECT, INSERT, httpClient.Post, await, repository.Save).
> 
> Pergunta de auditor: Essa chamada externa está dentro de um loop (for / while)? Ela está segurando uma conexão desnecessariamente?
> 
> Reconhecer um loop chamando o banco 50 vezes requer apenas identificar onde o loop abre e onde o banco é chamado. Qualquer pessoa treinada reconhece esse padrão em 10 segundos.
> 
> 3. Leitura Orientada por Hipótese (Usar a Spec como Gabarito)
> Quem não programa do zero nunca deve abrir um arquivo e tentar adivinhar o que ele faz. Você sempre parte da sua Especificação (SDD) e faz uma checagem cruzada:
> 
> Sua spec define: "Se o desconto for maior que 20%, exige autorização de supervisor."
> 
> Você abre o arquivo gerado e faz uma busca por 0.20 ou Desconto.
> 
> Você olha apenas as 3 linhas ao redor do if:
> 
> Se o código estiver aplicando o desconto sem verificar o papel do usuário, a IA ignorou a restrição. Você rejeita a entrega sem precisar entender como a tela ou o banco foram estruturados.
> 
> 4. Auditar o Teste, Não a Implementação
> O código de teste é infinitamente mais simples de ler do que o código de produção, porque ele é puramente declarativo:
> 
> Dado: Uma venda de 100€
> Quando: Aplico cupom de 10%
> Então: O total deve ser 90€
> Para auditar a IA, você não precisa ler o motor de faturamento. Você lê o arquivo de teste e faz duas perguntas:
> 
> Os valores de entrada e saída no teste são os mesmos da regra de negócio?
> 
> Se eu alterar a resposta esperada para 95€ no teste e mandar rodar, o teste quebra? (Se o teste não quebrar com um valor errado, o teste é falso/tautológico).
> 
> 5. Inspeção Visual de Execução (Deixar a Máquina Mostrar o Fluxo)
> Engenheiros experientes não ficam "simulando a execução do código na cabeça" como se fossem compiladores humanos. Eles usam ferramentas visuais:
> 
> Logs estruturados: Ler uma saída em JSON no terminal mostrando: [PedidoCriado] -> [ValidandoRegra] -> [Erro: LimiteExcedido].
> 
> Breakpoints e Debugger: Parar o código no ponto crítico e olhar a caixinha de variáveis na tela para ver se o valor da variável bate com a realidade.
> 
> Métricas de Profiling: Ver um gráfico de uso de CPU subir para 100% durante uma requisição. Isso não exige ler código, exige interpretar telemetria.
> 

<!-- FONTE: F043 FIM -->

<a id="fonte-f057"></a>

#### F057 — Cinco filtros consolidados no blueprint

Origem histórica: conversa original, linhas 939–975. Trecho principal desta etapa.

<!-- FONTE: F057 INICIO -->
> ## 2. O Método dos 5 Filtros de Auditoria Rápida
> 
> Quando a IA entrega uma funcionalidade acompanhada de código e testes, o orquestrador submete os artefatos a uma triagem de até 3 minutos:
> 
> [Artefato Gerado pela IA]
> │
> ├──► 1. Contrato (Assinaturas): O que entra e o que sai é suficiente?
> ├──► 2. Efeitos Colaterais (I/O): Onde toca em rede, disco ou banco? Há loops ou transações abertas?
> ├──► 3. Invariante (Ctrl+F): A regra matemática ou de negócio foi respeitada no condicional?
> ├──► 4. Auditoria do Teste: O teste falha se eu alterar a expectativa para um valor incorreto?
> └──► 5. Inspeção Viva (Telemetria): O log/debugger mostra latência anormal ou contenção?
> 
> 
> ### Detalhamento dos Filtros
> 
> 1. **Filtro de Contrato (Assinatura e Tipagem):**
>    * *Ação:* Inspecionar exclusivamente os parâmetros de entrada e o objeto de retorno.
>    * *Pergunta de controle:* O contrato expõe todos os dados necessários para o chamador sem forçar consultas redundantes posteriores?
> 
> 2. **Filtro de Efeitos Colaterais (I/O, Banco e Rede):**
>    * *Ação:* Rastrear termos como `await`, `SELECT`, `transacao`, `HTTP` e chamadas a serviços externos.
>    * *Pergunta de controle:* Existem chamadas lentas de rede dentro de transações ACID? Existem consultas ao banco de dados presas dentro de laços (`for`/`foreach`)?
> 
> 3. **Filtro de Invariantes por Hipótese:**
>    * *Ação:* Buscar diretamente no código os valores-chave da regra de negócio (ex.: `0.15` para 15% de desconto, limites de crédito, faixas de alíquota).
>    * *Pergunta de controle:* A condição lógica representa a regra real ou confunde grandezas (ex.: porcentagem tratada como valor absoluto)?
> 
> 4. **Filtro de Auditoria do Teste:**
>    * *Ação:* Ignorar a taxa percentual de cobertura e ler diretamente as asserções (`Assert`) dos testes gerados.
>    * *Pergunta de controle:* O teste valida cálculos reais ou apenas confere se a função retornou sem disparar erro? Se o valor esperado for sabotado manualmente, o teste quebra?
> 
> 5. **Filtro de Inspeção Viva (Telemetria e Logs):**
>    * *Ação:* Observar a saída do terminal de execução, logs estruturados ou rastreamento de chamadas.
>    * *Pergunta de controle:* Qual foi a latência real entre o início e o fim da operação? Houve excesso de comandos disparados contra o banco?
> 
> ---
> 

<!-- FONTE: F057 FIM -->

<a id="fonte-f068"></a>

#### F068 — Primeira sequência: leitura e filtros de auditoria

Origem histórica: conversa original, linhas 1114–1128. Trecho principal desta etapa.

<!-- FONTE: F068 INICIO -->
> Fase 2: Literacia Diagnóstica e os 5 Filtros de Auditoria
> Objetivo: Adquirir a capacidade de inspecionar, criticar e rejeitar código gerado por IA em minutos sem precisar aprender a digitar sintaxe do zero.
> 
> O que estudar e praticar:
> 
> Leitura por amostragem: identificação rápida de contratos de entrada/saída, assinaturas de métodos e fluxo de dependências.
> 
> O método dos 5 Filtros na prática: Contrato, Efeitos Colaterais (I/O), Invariantes por Busca Rápida (Ctrl+F), Asserção de Teste e Inspeção de Logs.
> 
> Reconhecimento de armadilhas clássicas da IA: chamadas assíncronas bloqueantes, loops aninhados com chamadas externas (N+1) e dependências alucinadas.
> 
> A virada de chave: Compreender que auditar código é uma habilidade de reconhecimento de padrões, e não de digitação criativa.
> 
> Capítulo gerado: Auditoria Cirúrgica: Como Ler e Conter Código Sem Passar Anos Programando.
> 

<!-- FONTE: F068 FIM -->

<a id="assunto-03"></a>

### 3. Exemplo completo para examinar

**O que já temos:** O caso da fatura inclui spec, implementação, diagnóstico, teste e logs.

**Para aprofundar:** Reavaliar os diagnósticos e as correções propostas antes de transformar o caso em exercício validado.

<a id="fonte-f045"></a>

#### F045 — Exemplo didático: especificação e cenário de fatura

Origem histórica: conversa original, linhas 748–760. Trecho principal desta etapa.

<!-- FONTE: F045 INICIO -->
> Sim
> Sim
> 
> Vamos ver isso na prática com um cenário realista de negócio: emissão de fatura com cálculo tributário e desconto.
> 
> Imagine que você especificou para a IA (via SDD):
> 
> "Criar o serviço de emissão de fatura. Regras: (1) Desconto acima de 15% exige aprovação de gerente; (2) Calcular o imposto de cada item; (3) Gravar a fatura no banco de dados; (4) Notificar o serviço fiscal governamental por API externa."
> 
> A IA gerou o código abaixo, avisou que "o código foi implementado com sucesso e 100% dos testes passaram".
> 
> O Código Gerado pela IA (Parece perfeito à primeira vista)
> C#

<!-- FONTE: F045 FIM -->

<a id="fonte-f046"></a>

#### F046 — Exemplo didático: código da emissão de fatura

Origem histórica: conversa original, linhas 761–806. Trecho principal desta etapa.

<!-- FONTE: F046 INICIO -->
~~~~csharp
public class FaturaService
{
    private readonly BancoContext _banco;
    private readonly SefazApiClient _sefazApi;

    public FaturaService(BancoContext banco, SefazApiClient sefazApi)
    {
        _banco = banco;
        _sefazApi = sefazApi;
    }

    public async Task<Guid> EmitirFatura(PedidoDto pedido)
    {
        using var transacao = await _banco.Database.BeginTransactionAsync();

        var fatura = new Fatura { Id = Guid.NewGuid(), Data = DateTime.Now };

        foreach (var item in pedido.Itens)
        {
            var taxa = await _banco.Taxas.FirstOrDefaultAsync(t => t.Codigo == item.Ncm);
            var imposto = item.PrecoUnitario * (taxa?.Percentual ?? 0.18m);
            
            fatura.Itens.Add(new ItemFatura {
                Descricao = item.Descricao,
                Total = (item.PrecoUnitario * item.Quantidade) - item.Desconto + imposto
            });
        }

        // Regra de desconto
        if (pedido.DescontoTotal > 0.15m)
        {
            fatura.Status = "PendenteAprovacao";
        }
        else
        {
            fatura.Status = "Emitida";
            await _sefazApi.TransmitirNotaFiscalAsync(fatura);
        }

        await _banco.Faturas.AddAsync(fatura);
        await _banco.SaveChangesAsync();
        await transacao.CommitAsync();

        return fatura.Id;
    }
}

~~~~
<!-- FONTE: F046 FIM -->

<a id="fonte-f047"></a>

#### F047 — Exemplo didático: contratos, I/O e invariante

Origem histórica: conversa original, linhas 807–849. Trecho principal desta etapa.

<!-- FONTE: F047 INICIO -->
> Para um programador tradicional, a revisão exigiria ler linha por linha.
> 
> Para um engenheiro orquestrador, aplicam-se os 5 filtros em menos de 2 minutos:
> 
> Aplicando os 5 Filtros de Auditoria Rápida
> Filtro 1: Contrato (Entrada e Saída)
> Tempo: 15 segundos.
> 
> Onde olhar: Na primeira linha: public async Task<Guid> EmitirFatura(PedidoDto pedido)
> 
> A pergunta: O que entrou e o que saiu?
> 
> O diagnóstico: Entrou um PedidoDto e saiu apenas um Guid (o ID da fatura).
> 
> O problema: Quem chamou a emissão precisa saber o valor dos impostos calculados ou o status da nota? Devolver apenas um Guid obriga quem chamou a fazer outra consulta no banco logo em seguida para saber o resultado.
> 
> Comando para a IA: "Altere o contrato de retorno para ResultadoEmissaoFatura, contendo o ID, o total de impostos apurados e o Status da emissão."
> 
> Filtro 2: Efeitos Colaterais & I/O (Banco e Rede)
> Tempo: 30 segundos.
> 
> Onde olhar: Procure apenas as palavras transacao, await, _banco e chamadas de API (_sefazApi).
> 
> A pergunta: Onde estamos tocando em rede ou disco, e o que está dentro do quê?
> 
> O diagnóstico (Grave!):
> 
> Problema N+1: Dentro do foreach (var item in pedido.Itens), a IA colocou await _banco.Taxas.... Se a fatura tiver 50 itens, o sistema vai abrir 50 conexões ao banco em sequência.
> 
> Chamada de Rede dentro de Transação: A linha await _sefazApi.TransmitirNotaFiscalAsync(fatura) está dentro do bloco using var transacao = ... BeginTransactionAsync(). Se a API do governo demorar 10 segundos para responder ou oscilar, a transação do banco fica travada, bloqueando tabelas e derrubando o servidor.
> 
> Comando para a IA: "Remova a chamada HTTP externa de dentro da transação do banco de dados (chame apenas após o commit). Carregue todas as taxas dos itens de uma só vez antes do loop em memória."
> 
> Filtro 3: Invariantes por Hipótese (Ctrl + F na Regra)
> Tempo: 20 segundos.
> 
> Onde olhar: Você sabe que a regra é "desconto acima de 15%". Aperte Ctrl + F e busque 0.15 ou Desconto.
> 
> A pergunta: Como essa regra foi escrita?
> 
> O diagnóstico: A IA escreveu:
> 
> C#

<!-- FONTE: F047 FIM -->

<a id="fonte-f048"></a>

#### F048 — Exemplo didático: condição de desconto

Origem histórica: conversa original, linhas 850–850. Trecho principal desta etapa.

<!-- FONTE: F048 INICIO -->
~~~~csharp
if (pedido.DescontoTotal > 0.15m)

~~~~
<!-- FONTE: F048 FIM -->

<a id="fonte-f049"></a>

#### F049 — Exemplo didático: interpretação e introdução do teste

Origem histórica: conversa original, linhas 851–862. Trecho principal desta etapa.

<!-- FONTE: F049 INICIO -->
> A falha: pedido.DescontoTotal está em valor absoluto (ex: 20€) ou em porcentagem (0.20)? Se o pedido for de 1.000€ e o desconto for de 50€, 50 > 0.15 é verdadeiro, e o sistema vai travar o pedido exigindo gerente para um desconto de 5%! A IA confundiu porcentagem com valor monetário.
> 
> Comando para a IA: "A regra de desconto de 15% deve ser proporcional ao subtotal do pedido: (DescontoTotal / Subtotal) > 0.15m, e não um valor absoluto."
> 
> Filtro 4: A Auditoria do Teste (O Teste é Tautológico?)
> Tempo: 30 segundos.
> 
> Onde olhar: Abra o arquivo de teste que a IA disse que "passou com 100%".
> 
> O teste que a IA gerou:
> 
> C#

<!-- FONTE: F049 FIM -->

<a id="fonte-f050"></a>

#### F050 — Exemplo didático: teste da emissão

Origem histórica: conversa original, linhas 863–869. Trecho principal desta etapa.

<!-- FONTE: F050 INICIO -->
~~~~csharp
[Fact]
public async Task Deve_Emitir_Fatura_Com_Sucesso()
{
    // A IA mockou o banco, mockou a sefaz retornando sucesso
    var resultado = await service.EmitirFatura(pedido);
    Assert.NotEqual(Guid.Empty, resultado);
}

~~~~
<!-- FONTE: F050 FIM -->

<a id="fonte-f051"></a>

#### F051 — Exemplo didático: leitura do teste e introdução dos logs

Origem histórica: conversa original, linhas 870–883. Trecho principal desta etapa.

<!-- FONTE: F051 INICIO -->
> A pergunta: O teste valida a regra ou apenas se o código roda sem explodir?
> 
> O diagnóstico: O teste apenas conferiu se gerou um Guid diferente de zero! Ele não testou o cálculo do imposto, não testou o bloqueio com 16% de desconto e nem o que acontece se a Sefaz cair.
> 
> Comando para a IA: "Escreva três testes com BDD: (1) Pedido com 16% de desconto deve ter Status 'PendenteAprovacao'; (2) Item com alíquota de 18% deve ter imposto calculado exatamente em X; (3) Se a Sefaz retornar timeout, a fatura deve ser persistida com status 'ErroTransmissao'."
> 
> Filtro 5: Verificação Viva no Log
> Tempo: 15 segundos.
> 
> Onde olhar: No terminal de execução / saída de logs.
> 
> O que você vê:
> 
> Plaintext

<!-- FONTE: F051 FIM -->

<a id="fonte-f052"></a>

#### F052 — Exemplo didático: sequência de logs

Origem histórica: conversa original, linhas 884–888. Trecho principal desta etapa.

<!-- FONTE: F052 INICIO -->
~~~~text
[DEBUG] BEGIN TRANSACTION
[DEBUG] SELECT * FROM Taxas WHERE Codigo = '123'
[DEBUG] SELECT * FROM Taxas WHERE Codigo = '456'
[DEBUG] HTTP POST https://api.sefaz... (aguardando resposta 3200ms)
[DEBUG] COMMIT TRANSACTION

~~~~
<!-- FONTE: F052 FIM -->

<a id="fonte-f053"></a>

#### F053 — Exemplo didático: interpretação dos logs

Origem histórica: conversa original, linhas 889–890. Trecho principal desta etapa.

<!-- FONTE: F053 INICIO -->
> O diagnóstico visual: Você bate o olho e vê o tempo de 3.200ms entre o BEGIN e o COMMIT. Mesmo sem entender nada da sintaxe interna do C#, qualquer um entende que segurar uma transação aberta por 3 segundos é uma bomba-relógio para o banco de dados.
> 

<!-- FONTE: F053 FIM -->

<a id="assunto-04"></a>

### 4. Testes, propriedades e verificação

**O que já temos:** A conversa reúne BDD, propriedades, mutação e verificação e validação.

**Para aprofundar:** Definir testes que discriminem comportamento correto e incorreto e revisar as alegações de prova matemática.

<a id="fonte-f029"></a>

#### F029 — Qualidade, testes e revisão de código gerado

Origem histórica: conversa original, linhas 500–510. Trecho principal desta etapa.

<!-- FONTE: F029 INICIO -->
> Módulo 4: Redes de Contenção, Invariantes e Quality Gates
> Objetivo: Criar barreiras matemáticas e lógicas automatizadas que barram o código gerado por IA antes de qualquer deploy.
> 
> Engenharia de Testes de Comportamento (BDD): Escrita de critérios de aceitação executáveis em Gherkin antes da solicitação de código ao agente.
> 
> Testes Baseados em Propriedades (Property-Based Testing): Definição de invariantes universais (ex.: "saldo final = entradas - saídas") e geração aleatória massiva de cenários extremos para quebrar implementações sugeridas pela IA.
> 
> Testes de Mutação: Validação da eficácia da suíte de testes (garantir que os testes realmente falham quando regras são violadas).
> 
> Revisão Semântica de Código: Análise de vulnerabilidades sutis em código de IA: vazamentos de escopo, dependências fantasmas (package hallucinations) e complexidade ciclomática oculta.
> 

<!-- FONTE: F029 FIM -->

<a id="fonte-f070"></a>

#### F070 — Primeira sequência: testes e validação

Origem histórica: conversa original, linhas 1144–1158. Trecho principal desta etapa.

<!-- FONTE: F070 INICIO -->
> Fase 4: A Rede de Contenção (BDD, Testes de Propriedade e Anti-Tautologia)
> Objetivo: Dominar as técnicas que provam matematicamente se a implementação da IA funciona, eliminando falsos positivos.
> 
> O que estudar e praticar:
> 
> BDD com Gherkin: escrita de cenários executáveis baseados em comportamento de negócio antes de acionar a IA para codificar.
> 
> Desmascarando testes tautológicos: como verificar se um teste falha de verdade quando a regra é violada (testes de mutação conceituais).
> 
> Testes baseados em propriedades (Property-Based Testing): definição de invariantes globais e geração de centenas de entradas extremas para tentar quebrar a lógica gerada.
> 
> A virada de chave: Entender que a suíte de testes não serve para "agradar o pipeline", mas para ser a cerca elétrica que impede a IA de alucinar.
> 
> Capítulo gerado: Testes Reais vs. Testes Placebo: Construindo a Rede de Proteção Contra a IA.
> 

<!-- FONTE: F070 FIM -->

<a id="fonte-f083"></a>

#### F083 — Sequência revisada: verificação e validação

Origem histórica: conversa original, linhas 1339–1347. Trecho principal desta etapa.

<!-- FONTE: F083 INICIO -->
> Fase 5: Verificação, Validação (V&V) e Redes de Contenção
> A distinção clássica: "Estamos construindo o produto certo?" (Validação) vs. "Estamos construindo o produto do jeito certo?" (Verificação).
> 
> Engenharia de Software: Pirâmide e Troféu de Testes; BDD (Behavior-Driven Development) como especificação executável; Property-Based Testing e Invariantes Matemáticas; Testes de Mutação para auditoria da suíte de testes.
> 
> Engenharia de Contratos: Design by Contract (Pré-condições, Pós-condições, Invariantes).
> 
> Aplicação com IA: Gerar testes comportamentais antes da implementação do código e utilizar testes de mutação para expor testes tautológicos gerados pela IA.
> 

<!-- FONTE: F083 FIM -->

<a id="assunto-05"></a>

### 5. Métricas e auditoria estática

**O que já temos:** Há sugestões de métricas de complexidade, acoplamento e análise estática.

**Para aprofundar:** Examinar contexto, limitações e critérios de interpretação das métricas antes de automatizar decisões.

<a id="fonte-f076"></a>

#### F076 — Métricas estáticas e análise de mutação

Origem histórica: conversa original, linhas 1253–1268. Trecho principal desta etapa.

<!-- FONTE: F076 INICIO -->
> 3. Métricas de Código e Garantia de Qualidade de Software (SQA)
> Para quem não lê milhares de linhas geradas pela IA, a Engenharia de Software oferece métricas estáticas objetivas:
> 
> Complexidade Ciclomática (Thomas McCabe): Quantidade de caminhos de execução independentes no código. Se a IA entrega uma função com complexidade ciclomática 
> >
> 10
> >10, a função é matematicamente propensa a bugs e deve ser sumariamente rejeitada.
> 
> Instabilidade (
> I
> I) e Abstração (
> A
> A): As métricas de Robert Martin para pacotes: um módulo central deve ser altamente abstrato e estável; módulos de borda devem ser flexíveis.
> 
> Cobertura de Código Efetiva (Análise de Mutação): O conceito formal de Mutation Testing, onde ferramentas injetam falhas deliberadas no código para provar se a suíte de testes realmente detecta anomalias.
> 

<!-- FONTE: F076 FIM -->

<a id="fonte-f080"></a>

#### F080 — Sequência revisada: qualidade e auditoria

Origem histórica: conversa original, linhas 1312–1320. Trecho principal desta etapa.

<!-- FONTE: F080 INICIO -->
> Fase 2: Garantia da Qualidade (SQA), Métricas Estáticas e Auditoria
> A ciência da medição de código sem necessidade de leitura linha por linha.
> 
> Engenharia de Software: Análise Estática de Código (SAST), Complexidade Ciclomática (McCabe), Métricas de Acoplamento Aferente e Eferente, e Leis de Halstead.
> 
> Os 5 Filtros Enriquecidos: Auditoria visual de assinaturas, rastreamento de efeitos colaterais de I/O, verificação de invariantes, asserções de teste e profiling.
> 
> Aplicação com IA: Configurar linters e analisadores estáticos que barram automaticamente qualquer entrega de IA com complexidade ciclomática ou acoplamento excessivo.
> 

<!-- FONTE: F080 FIM -->

<a id="assunto-06"></a>

### 6. Experimentação e alcance das conclusões

**O que já temos:** Laboratórios de falha e conclusões sobre o exercício são apresentados como meios de desenvolver julgamento.

**Para aprofundar:** Separar a detecção de um problema num exemplo da capacidade de auditar um sistema completo.

<a id="fonte-f036"></a>

#### F036 — Repertório de falhas e laboratório

Origem histórica: conversa original, linhas 601–607. Cópia relacionada para este assunto. Destino principal: [anexo 08](08-texto-anexo.md#fonte-f036).

<!-- FONTE: F036 INICIO -->
> 5. Repertório de Falhas (A Ausência de "Cicatrizes de Produção")
> O Gap: Ninguém aprende a tomar boas decisões apenas lendo manuais de boas decisões. As decisões de arquitetura existem porque alguém sofreu com as consequências da abordagem oposta.
> 
> O Risco na Tomada de Decisão: A pessoa aplicará padrões de design sem saber a dor que eles curam. Usará Arquitetura Hexagonal para um script simples de automação, gerando uma complexidade desnecessária de interfaces e adaptadores que a IA terá de manter.
> 
> O que falta: Metodologia de "Engenharia Reversa de Desastres": colocar o aluno para ver sistemas quebrando sob carga, bancos caindo por falta de pool de conexões e filas travando por poison messages.
> 

<!-- FONTE: F036 FIM -->

<a id="fonte-f054"></a>

#### F054 — Conclusões e alcance atribuídos ao exercício

Origem histórica: conversa original, linhas 891–913. Cópia relacionada para este assunto. Destino principal: [anexo 11](11-texto-anexo.md#fonte-f054).

<!-- FONTE: F054 INICIO -->
> O Que Esse Exercício Prova
> Você não precisou:
> 
> Lembrar de cabeça a sintaxe de async/await ou using var.
> 
> Saber como o Entity Framework mapeia tabelas internamente.
> 
> Digitar 80 linhas de classes e métodos.
> 
> Você precisou apenas de:
> 
> Saber o que procurar: Onde o código fala com o mundo externo (banco e HTTP).
> 
> Checar o contrato: Entrada e saída.
> 
> Validar a invariante com busca direta: A regra do negócio (0.15).
> 
> Desconfiar do teste superficial: O teste validou o comportamento ou apenas um Guid?
> 
> Esse é o modelo exato que capacita um profissional sem anos de digitação de código a liderar e orquestrar agentes com segurança de nível sênior.
> 
> Quer transformar esse método dos 5 Filtros em um capítulo estruturado com exercícios no sumário do livro?
> 

<!-- FONTE: F054 FIM -->
