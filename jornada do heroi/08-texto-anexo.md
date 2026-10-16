# 08. Texto anexo — A primeira missão real

[Etapa da jornada](08-a-primeira-missao-real.md) · [Índice](README.md) · [Mapa de origem](MAPA_ORIGEM.md)

Este anexo reúne 15 trechos: 3 principais e 12 cópias relacionadas. A organização abaixo identifica o que a conversa já oferece e o que ainda precisa ser aprofundado.

As sínteses são uma leitura editorial do material. Os blocos identificados como fonte preservam literalmente perguntas, respostas, exemplos e versões anteriores; sugestões da outra IA não passam a ser decisões aprovadas ou resultados comprovados por estarem neste anexo.

## Mapa de aprofundamento

| Assunto | O que já temos | O que aprofundar |
| --- | --- | --- |
| [Escolha do recorte prático](#assunto-01) | A conversa sugere usar um módulo existente e oferece faturamento, regras fiscais e estoque como possíveis fios condutores. | Escolher um recorte, documentar a situação inicial e definir o resultado que será observável. |
| [Laboratórios de falha](#assunto-02) | A IA sugere estudar sistemas quebrando para desenvolver repertório de diagnóstico. | Planejar experimentos delimitados, com hipótese, condições de reprodução e critério de encerramento. |
| [Caso didático completo de emissão de fatura](#assunto-03) | Há uma especificação, código C#, análise de contratos e I/O, regra de desconto, teste e logs de exemplo. | Revisar o caso antes de executá-lo ou ensiná-lo. Ele foi apresentado pela IA e não constitui evidência de um problema observado no seu produto. |
| [Do experimento ao registro](#assunto-04) | O ciclo proposto liga dor real, leitura, refatoração e escrita. | Definir o que será registrado antes, durante e depois do experimento. |

## Texto de referência por assunto

<a id="assunto-01"></a>

### 1. Escolha do recorte prático

**O que já temos:** A conversa sugere usar um módulo existente e oferece faturamento, regras fiscais e estoque como possíveis fios condutores.

**Para aprofundar:** Escolher um recorte, documentar a situação inicial e definir o resultado que será observável.

<a id="fonte-f004"></a>

#### F004 — Estudo aplicado ao próprio produto

Origem histórica: conversa original, linhas 124–136. Cópia relacionada para este assunto. Destino principal: [anexo 06](06-texto-anexo.md#fonte-f004).

<!-- FONTE: F004 INICIO -->
> O Caminho Rápido para Fechar a Lacuna
> Não tente ler manuais de 1.000 páginas do início ao fim sem contexto. Use o método de reengenharia reversa do seu próprio produto:
> 
> Pegue um módulo crítico que você já codificou (ex.: emissão de documento, cálculo de alíquotas ou sincronização com a nuvem).
> 
> Estude o livro de referência sobre o tema (veja referências como Domain-Driven Design de Eric Evans, Designing Data-Intensive Applications de Martin Kleppmann, ou Clean Architecture de Robert Martin).
> 
> Mapeie o que você fez versus o padrão formal: documente as diferenças, os atalhos tomados e como aquele módulo seria desenhado sob os padrões da indústria.
> 
> Esse exercício fornece tanto o vocabulário sênior quanto conteúdo de alto nível para artigos e discussões técnicas no LinkedIn.
> 
> Quer que eu monte um plano de estudos estruturado para os próximos 3 meses com os livros e referências essenciais?
> 

<!-- FONTE: F004 FIM -->

<a id="fonte-f014"></a>

#### F014 — Como estudar enquanto mantém as entregas

Origem histórica: conversa original, linhas 220–229. Cópia relacionada para este assunto. Destino principal: [anexo 06](06-texto-anexo.md#fonte-f014).

<!-- FONTE: F014 INICIO -->
> Como Estudar sem Parar as Entregas Práticas
> Para quem já tem anos de prática e projetos rodando, o método mais eficiente é o estudo aplicado por refatoração:
> 
> Escolha um livro por vez: Comece por Unit Testing (Khorikov) ou Domain-Driven Design Distilled (Vernon).
> 
> Identifique um trecho do seu sistema: Pegue uma regra que hoje está densa, difícil de testar ou que depende diretamente de uma tabela do banco de dados.
> 
> Aplique o padrão estudado no código real: Reescreva a camada isolando o domínio e escreva os testes cobrindo as invariantes.
> 
> Esse ciclo fecha a lacuna teórica imediatamente e gera material concreto para documentações técnicas e artigos de autoridade.

<!-- FONTE: F014 FIM -->

<a id="fonte-f015"></a>

#### F015 — Possibilidade de aplicação ao domínio fiscal

Origem histórica: conversa original, linhas 230–232. Trecho principal desta etapa.

<!-- FONTE: F015 INICIO -->
> 
> Quer que eu detalhe como aplicar o isolamento de domínio e testes comportamentais especificamente em um módulo fiscal/faturamento?
> 

<!-- FONTE: F015 FIM -->

<a id="fonte-f023"></a>

#### F023 — Escolha de caso condutor para o capítulo

Origem histórica: conversa original, linhas 436–436. Trecho principal desta etapa.

<!-- FONTE: F023 INICIO -->
> Qual domínio ou caso de uso prático você prefere usar como fio condutor nos exemplos de código desse capítulo piloto: regras de cálculo de faturamento/impostos ou validação de concorrência em estoque?

<!-- FONTE: F023 FIM -->

<a id="assunto-02"></a>

### 2. Laboratórios de falha

**O que já temos:** A IA sugere estudar sistemas quebrando para desenvolver repertório de diagnóstico.

**Para aprofundar:** Planejar experimentos delimitados, com hipótese, condições de reprodução e critério de encerramento.

<a id="fonte-f036"></a>

#### F036 — Repertório de falhas e laboratório

Origem histórica: conversa original, linhas 601–607. Trecho principal desta etapa.

<!-- FONTE: F036 INICIO -->
> 5. Repertório de Falhas (A Ausência de "Cicatrizes de Produção")
> O Gap: Ninguém aprende a tomar boas decisões apenas lendo manuais de boas decisões. As decisões de arquitetura existem porque alguém sofreu com as consequências da abordagem oposta.
> 
> O Risco na Tomada de Decisão: A pessoa aplicará padrões de design sem saber a dor que eles curam. Usará Arquitetura Hexagonal para um script simples de automação, gerando uma complexidade desnecessária de interfaces e adaptadores que a IA terá de manter.
> 
> O que falta: Metodologia de "Engenharia Reversa de Desastres": colocar o aluno para ver sistemas quebrando sob carga, bancos caindo por falta de pool de conexões e filas travando por poison messages.
> 

<!-- FONTE: F036 FIM -->

<a id="assunto-03"></a>

### 3. Caso didático completo de emissão de fatura

**O que já temos:** Há uma especificação, código C#, análise de contratos e I/O, regra de desconto, teste e logs de exemplo.

**Para aprofundar:** Revisar o caso antes de executá-lo ou ensiná-lo. Ele foi apresentado pela IA e não constitui evidência de um problema observado no seu produto.

<a id="fonte-f045"></a>

#### F045 — Exemplo didático: especificação e cenário de fatura

Origem histórica: conversa original, linhas 748–760. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f045).

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

Origem histórica: conversa original, linhas 761–806. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f046).

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

Origem histórica: conversa original, linhas 807–849. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f047).

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

Origem histórica: conversa original, linhas 850–850. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f048).

<!-- FONTE: F048 INICIO -->
~~~~csharp
if (pedido.DescontoTotal > 0.15m)

~~~~
<!-- FONTE: F048 FIM -->

<a id="fonte-f049"></a>

#### F049 — Exemplo didático: interpretação e introdução do teste

Origem histórica: conversa original, linhas 851–862. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f049).

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

Origem histórica: conversa original, linhas 863–869. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f050).

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

Origem histórica: conversa original, linhas 870–883. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f051).

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

Origem histórica: conversa original, linhas 884–888. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f052).

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

Origem histórica: conversa original, linhas 889–890. Cópia relacionada para este assunto. Destino principal: [anexo 10](10-texto-anexo.md#fonte-f053).

<!-- FONTE: F053 INICIO -->
> O diagnóstico visual: Você bate o olho e vê o tempo de 3.200ms entre o BEGIN e o COMMIT. Mesmo sem entender nada da sintaxe interna do C#, qualquer um entende que segurar uma transação aberta por 3 segundos é uma bomba-relógio para o banco de dados.
> 

<!-- FONTE: F053 FIM -->

<a id="assunto-04"></a>

### 4. Do experimento ao registro

**O que já temos:** O ciclo proposto liga dor real, leitura, refatoração e escrita.

**Para aprofundar:** Definir o que será registrado antes, durante e depois do experimento.

<a id="fonte-f072"></a>

#### F072 — Ciclo proposto de estudo, aplicação e escrita

Origem histórica: conversa original, linhas 1204–1214. Cópia relacionada para este assunto. Destino principal: [anexo 06](06-texto-anexo.md#fonte-f072).

<!-- FONTE: F072 INICIO -->
> A Dinâmica do Estudo Aplicado
> Para manter a consistência e não transformar o processo em uma sobrecarga teórica, cada fase deve seguir o mesmo ciclo de execução:
> 
> A Dor Real (1 semana): Identifique no seu sistema atual onde essa fase dói (ex.: na Fase 6, uma venda que trava o banco ou uma sincronização offline com conflito).
> 
> O Estudo Focado (1 semana): Leia os capítulos correspondentes dos livros clássicos (Kleppmann para dados, Khorikov para testes, Vernon para domínio) anotando apenas o que resolve aquela dor específica.
> 
> A Refatoração via IA (1 semana): Escreva a Spec técnica (SDD), submeta à IA, aplique os filtros de auditoria e implemente a correção no seu software.
> 
> O Registro do Capítulo (1 semana): Escreva o capítulo do livro detalhando: qual era o erro original, qual foi o raciocínio arquitetural aplicado, como a IA foi direcionada e qual foi o código resultante.
> 

<!-- FONTE: F072 FIM -->
