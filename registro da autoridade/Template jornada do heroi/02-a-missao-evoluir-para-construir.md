# 02. A missão: evoluir para construir

*(Aceitei a missão principal. Devia ter lido as letras miúdas.)*

[Índice da jornada](README.md) · [Etapa anterior](01-novo-mundo-bagagem-antiga.md) · [Próxima etapa](03-a-classe-engenheiro-agentico.md)

**Na prática:** Tese central, o choque da alucinação de layout, o nascimento do harness e o campo de força de 9 validações que prepara o Capítulo 0.

---

## O relato da etapa: As letras miúdas do contrato

Terminei o primeiro capítulo da minha história com a primeira vitória concreta no inventário: a Nota Fiscal de Consumidor Eletrônica tinha saído em homologação. Para quem entrou na masmorra munido apenas da bagagem de décadas em TI, muita teimosia e uma IA cuspindo código na tela, ver a autorização da SEFAZ brilhar verde no ambiente de testes deu aquela sensação inconfundível de conquista de RPG: subida de nível, fanfarra tocando ao fundo e a ilusão reconfortante de que o pior já tinha ficado para trás.

Eu estava no nível 10. Sentia que já entendia um pouco do mapa.

Diante de mim reluzia a missão principal: transformar aquele protótipo no **PDV D+**, um sistema de frente de caixa completo para rodar no comércio de verdade. E a escolha dessa masmorra específica não teve nada de aleatória ou vaidade técnica; ela nasceu da mais pura estratégia de sobrevivência comercial da Sampa TI.

No dia a dia da minha empresa, o PDV é o nosso produto "faca de entrada": é barato, enxuto na usabilidade e é a ferramenta que nos permite abrir as portas dos clientes de forma rápida e direta. Só que ele também era a nossa maior fonte de dor de cabeça com parceiros de software. O problema nunca foi defeito no código alheio, mas os custos pesados de repasse e a vulnerabilidade de ficar sem suporte emergencial quando o cliente estava parado no balcão e mais precisava de nós. 

Eu conheço os pormenores fiscais do comércio de ponta a ponta. Muitas vezes eu me antecipava às mudanças regulatórias e tributárias antes mesmo das software houses parceiras ou dos próprios escritórios de contabilidade. Depender de terceiros para o nosso principal produto de tração era uma loucura operacional. Ter o controle do PDV nas minhas mãos significava soberania de negócio, margem saudável e a segurança de nunca mais deixar um cliente na mão.

Apertei o botão de aceitar a missão. O detalhe é que eu devia ter inspecionado com mais cuidado as letras miúdas do contrato com a inteligência artificial.

---

A empolgação com a primeira vitória costuma durar até o momento em que a poeira baixa e você encara o que realmente sustenta uma operação fiscal.

Muitos desenvolvedores acham que o maior pavor de um sistema de caixa é a tela travar com fila no sábado à noite. Eu não tinha esse receio. As regras de negócio do PDV D+ estavam sob meu controle absoluto porque projetei o sistema com blindagens ativas na raiz — o que no jargão técnico chamam de invariantes e *fail-fast*:
1. O PDV simplesmente **não abre** se houver qualquer parâmetro ou configuração do ambiente inválida;
2. Um produto **não entra** na venda se faltar um único dado fiscal obrigatório;
3. O cadastro de mercadorias **não salva** se a tributação for incompatível, eliminando cadastros errados antes mesmo que eles cheguem perto da frente de caixa.

O meu verdadeiro choque de realidade com as letras miúdas da IA não estava na venda de balcão. Estava na camada invisível e punitiva da responsabilidade fiscal.

A IA gera código com facilidade espantosa, mas nenhuma inteligência artificial assume o CNPJ da empresa ou a responsabilidade civil perante o Fisco. Quando fui desenhar as entranhas da operação, as perguntas que tiravam o sono eram outras:
* *Como blindar o sistema para garantir que nenhuma numeração de nota fiscal seja pulada perante a SEFAZ?*
* *Como garantir a geração e exportação impecável do relatório fiscal e do lote de XMLs para o contador no fim do mês?*
* *Como validar a integridade estrutural e o schema de cada XML retornado após a autorização?*

A IA acelera a digitação, mas devolve para o desenvolvedor, com juros compostos, o peso de todas as garantias arquiteturais e legais que ela é incapaz de conceber sozinha.

---

Nesse ponto da travessia, você descobre que o mercado lá fora está contaminado por dois tipos muito barulhentos de conselheiros.

O primeiro grupo é a guilda dos **manuais arcaicos**. É o pessoal que decreta que você não tem direito de construir nada com IA enquanto não passar quatro anos decorando sintaxe de ponteiros, memorizando tabelas de APIs e sofrendo para digitar cada ponto e vírgula na mão. Para eles, o mérito de um desenvolvedor é medido pela tendinite e pelo calo nos dedos, ignorando que a geração de sintaxe virou uma commodity instantânea.

O segundo grupo é a seita do **hype irresponsável**. São os gurus de internet que vendem a ilusão de que qualquer um vira engenheiro de software em três dias apenas colando "prompts mágicos" em um chat. 

Eu olhei para os dois caminhos e recusei categoricamente os dois. 

Eu tinha uma armadura dupla contra essas armadilhas. Primeiro, como **desenvolvedor low-code**, eu já sabia muito bem que existem formas rápidas e seguras de acelerar a entrega de valor; eu já tinha uma sólida base de lógica de programação e de regras de negócio. O que me faltava não era aprender a pensar, mas sim um meio de gerar código de baixo nível de forma concisa e veloz. Segundo, porque eu já trabalhei profissionalmente com **marketing digital**. Eu conheço a mecânica da persuasão, os gatilhos e a engenharia reversa que os vendedores de fórmulas mágicas usam para empurrar ilusões para quem é leigo.

Eu sabia que nenhum extremo se sustentava. Se você amarrar uma arquitetura sólida — mesmo que simples — e aplicar validações rigorosas na raiz, a IA é uma alavanca brutal de produtividade. Mas se você acreditar em mágica, você cria castelos de cartas e **testes tautológicos**: agentes escrevendo testes que só servem para aprovar as próprias alucinações que acabaram de inventar, entregando sistemas ocos com 100% de cobertura verde que explodem na primeira semana de operação.

A minha tese de trabalho nasceu dessa recusa:

> *Você não precisa passar anos decorando sintaxe do zero para ser um arquiteto e engenheiro respeitado na era da IA. Mas você precisa, obrigatoriamente, dominar os modelos mentais da computação, a arquitetura de sistemas e a capacidade diagnóstica para governar, conter e auditar o código que os agentes entregam.*

A habilidade mais rara e valiosa migrou da **síntese** (a digitação braçal da sintaxe) para o **reconhecimento analítico** (a auditoria de fronteiras e a governança de contratos).

---

## O Clímax: A Alucinação Destrutiva e o "Campo de Força"

Só que toda teoria desmorona no primeiro contato com o caos. E o meu batismo de fogo aconteceu quando a inteligência artificial mostrou a sua face mais destrutiva.

Eu estava com o motor fiscal funcionando, notas sendo homologadas e a estrutura estável. Foi quando pedi um ajuste simples, quase inofensivo: mudar o espaçamento e alinhar elementos visuais do layout de tela. 

A IA foi lá e executou. Mas, junto com a folha de estilo, ela simplesmente **destruiu o código que já funcionava**. Ela refizera classes inteiras do motor fiscal sem que ninguém pedisse, trocara tipos de dados homologados, apagara validações prévias e quebrara o fluxo de emissão — tudo para conseguir mexer num botão de tela.

Ali caiu a última ficha. O perigo dos agentes não é a falta de capacidade técnica; é a total ausência de disciplina de fronteira e de memória operacional. Se você não coloca rédeas de ferro na máquina, ela conserta a maçaneta da porta implodindo os alicerces da casa.

Chega de pedir por favor com prompts bonitos. A engenharia tinha que entrar em ação.

Comecei, linha por linha, a construir o meu próprio sistema de contenção: o **harness** do projeto. Regras de contenção, guardrails estritos, skills especializadas e servidores MCP (Model Context Protocol), tudo configurado na unha. Cada alucinação da IA, cada linha destruída sem autorização e cada erro de sintaxe eram capturados e transformados imediatamente em uma nova regra explícita no sistema.

No começo, era um arquivo de regras monolítico, gigante e pesado. Conforme as IDEs evoluíam e eu devorava a documentação oficial, fui refatorando tudo: quebrei o monólito em índices modulares e arquivos específicos para cada segmento tecnológico do ecossistema.

E para garantir que nada passasse despercebido, forjei o meu **"Campo de Força"**: um pipeline automatizado de validação de código. 

Ele nasceu humilde, com 9 pequenas checagens essenciais de linter, formatação de código e análise estática. Conforme as batalhas avançavam, ele foi crescendo até virar uma muralha impenetrável. Hoje, esse campo de força pega absolutamente tudo o que o agente costuma errar: de deslizes bobos de sintaxe a reuso indevido de layout que quebra o domínio. O validador aponta o erro cirurgicamente, obriga a IA a entrar em um loop fechado de autocorreção e ainda alimenta o harness para que a máquina nunca mais cometa a mesma falha.

O que começou como um esforço intuitivo de sobrevivência nos últimos 10 meses de autoestudo transformou-se em uma metodologia concisa de governança agêntica.

---

## O Gancho da Próxima Fase: A Fundação Revelada

Eu não sou mais um profissional de TI brigando com um gerador de texto. Eu me tornei um orquestrador com um sistema operacional próprio de engenharia.

O **PDV D+** é o meu laboratório vivo, com exigência fiscal implacável e clientes de carne e osso. O **livro técnico** que estou estruturando é o mapa onde organizo cada modelo mental compreendido, eliminando a dispersão para quem precisa construir sistemas de missão crítica. E esta **jornada autoral** é o registro honesto da travessia.

O contrato foi assinado e as letras miúdas foram domadas pelo nosso próprio campo de força. O tutorial da empolgação ficou definitivamente para trás.

No próximo passo, eu não vou apenas contar mais uma história. Nós vamos abrir as portas do **Capítulo 0 — A Fundação**: vou detalhar a anatomia exata desse harness, as engrenagens desse campo de força de validações e os modelos mentais que transformam um profissional experiente em um verdadeiro **Engenheiro Agêntico**.

A missão principal foi aceita. E agora, as regras da masmorra são as nossas.

---

## Acompanhamento e Evidências da Etapa

* **Data de consolidação:** 20 de outubro de 2026.
* **Arco:** I — Reencarnação: veterano em um mundo desconhecido.
* **Peça de publicação gerada:** [PUB-003 — A missão: evoluir para construir](<../publicacoes/02-a-missao-evoluir-para-construir/artigo.md>).
* **Marco alcançado:** Tese central fundamentada na estratégia real da Sampa TI, blindagem fiscal ativa, ceticismo embasado (low-code e marketing digital), o clímax da quebra de layout pela IA, o nascimento do harness modular e do "Campo de Força" (de 9 validações ao loop de autocorreção), estabelecendo o gancho definitivo para o Capítulo 0 (A Fundação) e para a Etapa 03.
* **Próxima passagem:** [03. A classe: engenheiro agêntico](03-a-classe-engenheiro-agentico.md).
