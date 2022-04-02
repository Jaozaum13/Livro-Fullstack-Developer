# POSICIONANDO ELEMENTOS COM FLEXBOX EM CSS
## APRESENTAÇÃO DO CURSO
O objetivo desse curso é apresentar os fundamentos e aplicações da propriedade flexbox na criação de layouts responsivos, sem a necessidade de definição de valores fixos, ou seja, criar um site responsivo que se adaptará aos diversos tipos de resoluções e dispositivos.

## INTRODUÇÃO AO FLEXBOX
O QUE É O FLEXBOX?

O flexbox foi pensado como um modelo de layout unidimensional e como um método que pode oferecer distribuição de espaço entre itens em uma interface e recurso de alinhamento.

![NAVEGADORES QUE SUPORTAM O FLEXBOX.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/025e4b03-f80a-4633-a2bd-c4a85d3af43b/NAVEGADORES_QUE_SUPORTAM_O_FLEXBOX.png)

NAVEGADORES QUE SUPORTAM O FLEXBOX.

FLEX CONTAINER

O QUE É?

O flex container é a tag que envolve os itens, será nela que iremos aplicar a propriedade “display: flex”. Transformando seus itens filhos em flex itens, ou seja, esse itens se alinham a diversas resoluções. A partir do momento em que qualquer tag possuir itens filhos ela se torna passível de aplicar o item flex.

O flex container também possui propriedades relacionadas. Que são:

display - que é o inicializador do container

flex-direction - que vai fazer direcionamento desse itens, seja em linha, seja em coluna.

flex-wrap - vai se aplicar para quebra de linha ou não.

flex-flow - é a abreviação do direction e do wrap.

justify-content - vai alinhar os itens do container de acordo com a sua direção.

align-items - que vai alinhar esse itens de acordo com seu eixo no container.

align content - que vai alinhar as linhas desse container.

FLEX ITEM

O QUE É?

São os elementos filhos diretos do Flex Container. E também podem se tornar Flex Container, conseguimos aplicar a propriedade display para torná-los Flex Container.

![IMAGEM DO MODELO DE UM FLEX ITEM](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/46e97672-f4ed-4ac0-9a86-c9f027cf8524/IMAGEM_DE_UM_FLEX_ITEM.png)

IMAGEM DO MODELO DE UM FLEX ITEM

Os flex items também possuem propriedades relacionadas, que são:

flex-grow - vai definir o fator de crescimento

flex-basis - vai definir o tamanho inicial desse item antes da distribuição do espaço restante dentro do container.

flex-shrink - defini a capacidade de redução

flex - é a abreviação para as propriedades grow, basis e shrink.

order - é relacionado a ordem de distribuição e listagem desse itens.

align-self - defini o alinhamento de um item específico dentro do nosso container.

## ESTRUTURA BÁSICA DO “display: flex”
PARTE - 1

Iniciar uma tag qualquer HTML como “display: flex”, torna essa tag um elemento do tipo flex container, e assim automaticamente todos os filhos diretos dessa tag, tornam-se flex items. Sendo assim, trabalharemos toda a edição desse container, como por exemplo, como alinhar itens dentro desse container, como fazer quebra de linhas, como encaixar filhos dentro desse container para que os mesmos não vazem, etc.

OBS: Nós conseguimos aplicar a propriedade “display: flex” a qualquer tipo de tag em nosso HTML, assim como conseguimos fazer com que nossos flex items sejam flex container. Pode ser qualquer tag mesmo, div, span, section, h1-h6, tags de links.

PARTE - 2 → PRÁTICA COM “display: flex”

![CÓDIGO DO SITE COM FLEXBOX.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/231441d8-8ac7-4aea-8f69-ca431986b8f7/CDIGO_DO_SITE_COM_FLEXBOX.png)

CÓDIGO DO SITE COM FLEXBOX.

Para utilizar o snippet no HTML basta você digitar html e o auto completar irá completar com html : 5, ai basta você selecionar que ele irá te dar a programação básica de um HTML.

Se você usar a propriedade “div.item*3” e pressionar tab, você conseguirá abrir 3 elementos nomeados como item, a você só escreve a informação que pretende apresentar ao usuário do site. A parte “*3” da propriedade pode ser substituída por qualquer número que ele abrirá aquele número de elementos.

Caso você adicione “class=”flex”” na sua div, e adicione “display: flex;” no style “.flex”, você vai deixar cada item dentro de um determinado container e cada item ocupará apenas seu espaço de conteúdo.

![ITEM OCUPANDO SOMENTE SEU ESPAÇO DE CONTEÚDO E DENTRO DE UM CONTAINER.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8e14299c-2dbe-4398-b9dc-9d059d3d7d75/FLEXBOX_OCUPANDO_APENAS_SEU_ESPAO_DE_CONTEDO.png)

ITEM OCUPANDO SOMENTE SEU ESPAÇO DE CONTEÚDO E DENTRO DE UM CONTAINER.

Pode acontecer de aquele container não conseguir mais comportar esses items e acabar vazando. Aprenderemos como resolver esse vazamento um pouco mais pra frente.

Se você apertar f1 e digitar “Live Server”, o auto completar vai completar com “Live Server: Open with Live Server”, e agora qualquer mudança que você fizer no seu desenvolvimento ele irá automaticamente alterar na página web que está aberta.

Você também pode utilizar o plugin “Show Live Server Preview”, esse plugin abrirá uma aba ao lado do seu código para mostrar as alterações feitas em seu código automaticamente.

##  ESTRUTUTURA BÁSICA DO FLEX DIRECTION
PARTE - 1

Flex-direction é a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex items são colocados no flex container, temos basicamente dois eixos, o linha que é o horizontal e a coluna que é a vertical.

Os próximos valores que vamos trabalhar em cima deles são as posições reversas, ou seja, a ordenação inversa desses items. Uma vez que entendemos primeiro comportamento o segundo fica um pouco mais simples.

Os eixos...

row (padrão): à direção do texto, da esquerda para a direita.

![Modelo de um container organizado em row.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f1ac3714-0234-477b-a24b-9c98f66a5cd7/CONTAINER_ORDENADO_EM_ROW.png)

Modelo de um container organizado em row.

row-reverse: sentido oposto à direção do texto.

![Modelo de um container organizado em row-reverse.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ff1b8fce-d9fa-4aca-84a6-59b905bc1edf/CONTAINER_ORDENADO_EM_ROW-REVERSE.png)

Modelo de um container organizado em row-reverse.

column: ordenação de cima para baixo, em coluna única.

![Modelo de um container organizado em column.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d1a32316-5175-4eb3-aaa3-d9b55ecc92ca/CONTAINER_ORDENADO_EM_COLUMN.png)

Modelo de um container organizado em column.

column-reverse: ordenação inversa, de baixo para cima.

![Modelo de um container organizado em column-reverse.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6619e385-15dc-42a2-a71c-f0fcb079a28b/CONTAINER_ORDENADO_EM_COLUMN-REVERSE.png)

Modelo de um container organizado em column-reverse.

## PARTE - 2 → PRÁTICA COM FLEX DIRECTION
Nessa aula nós utilizamos o flexbox para alterar os eixos que foram citados acima.

![As quatro alterações dos eixos com flex-direction.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7907172a-d15b-46d8-816f-a85a311fdcfb/PRINT_DOS_EIXOS_COM_FLEX_DIRECTION.png)

As quatro alterações dos eixos com flex-direction.

Para ver como ficou o código desse html siga esse caminho: Atalhos Área de Trabalho/Ferramentas para programar/PROJETOS/AULA FLEXBOX.

## ESTRUTURA BÁSICA COM FLEX WRAP
PARTE - 1

É a propriedade que define se os flex itens devem ou não quebrar a linha.

Por padrão eles não quebram linha, isso faz com que os flex itens sejam compactados além do limite do conteúdo e também do limite do nosso container, e essa sobre carga do limite do container acaba por gerar um vazamento dos flex itens do container.

![CONTAINER COM VAZAMENTO DE CONTEÚDO.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/97ba23aa-9fd2-4501-8530-3e7d753d10a5/CONTAINER_COM_VAZAMENTO_DE_CONTEDO.png)

CONTAINER COM VAZAMENTO DE CONTEÚDO.

Note que o último flex item desse container, o número 5 está vazando.

Essa situação acima ocorre, pois por padrão do flex-container, a gestão de container setada é a nowrap.

NOWRAP

É o padrão, não permite a quebra de linha.

WRAP

Permite a quebra de linha assim que um dos flex itens não puder mais ser compactado, logo ele colocará esse flex itens na linha de baixo.

![CONTAINER COM WRAP.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1bc088e8-51b9-4f3c-bd2b-fb5dcd1d232c/CONTAINER_COM_WRAP.png)

CONTAINER COM WRAP.

Com essa adaptação, o problema do vazamento do flex item é resolvido, porém surgirá outro problema. Esse problema é o espaçamento que ficará entre o último flex item e o final do container, mas esse é um problema que aprenderemos a resolver mais para frente.

WRAP-REVERSE

Permite a quebra de linha, porém é como se nós estivéssemos escrevendo e sempre que completasse uma linha nós apertássemos enter e voltasse para a linha de cima, assim mantendo-se sempre na primeira linha.

![CONTAINER COM WRAP REVERSE.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/25f090e4-78e4-4db3-aef6-81a972845796/CONTAINER_COM_WRAP-REVERSE.png)

CONTAINER COM WRAP REVERSE.

## PARTE - 2 → PRÁTICA COM FLEX WRAP

Nessa aula nós aprendemos na prática como mudar as configurações de wrap do html.

Para ver como ficou o código desse html siga esse caminho: Atalhos Área de Trabalho/Ferramentas para programar/PROJETOS/AULA FLEXBOX.

Uma dica importante é que da para mexer no flex wrap com o flex direction que você quiser, ou seja, row, row-reverse, column ou column-reverse.

## ESTRUTURA BÁSICA E PRÁTICA COM FLEX FLOW
O flex-flow é um atalho para as propriedades flex-direction e flex-wrap. Porém seu uso não é tão comum, visto que, quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.

Nessa aula nós usamos o flex-flow em todos as combinações possíveis de se fazer com flex-direction e flex-wrap.

Para ver como ficou o código desse html siga esse caminho: Atalhos Área de Trabalho/Ferramentas para programar/PROJETOS/AULA FLEXBOX.

## ESTRUTURA BÁSICA COM JUSTIFY CONTENT
PARTE - 1

Essa propriedade se encarrega de cuidar do alinhamento dos itens dentro do container e trata também da distribuição de espaço entre eles.

OBS: caso seus itens estejam ocupando 100% do container, ela não se aplica.

Essa propriedade possui algumas variações, que são:

flex-start - vai fazer o alinhamento no início desse container.

flex-end - vai fazer o alinhamento no final do container.

center - vai fazer o alinhamento ao centro do container.

space-between - cria um espaçamento igual entre os elementos, mas tem um porém, ele vai pegar o primeiro elemento e colocar muito próximo ao início do container e o último elemento irá ser posicionado bem próximo ao final desse container.

space-around - vai tratar do espaçamento ao meio tornando-os duas vezes maior que o do início e do final.

## PARTE - 2 → PRÁTICA COM JUSTIFY CONTENT

Nessa aula nós trabalhamos com o justify content e todas as suas variações, porém sendo aplicadas somente com o flex direction em row.

Para ver como ficou o código desse html siga esse caminho: Atalhos Área de Trabalho/Ferramentas para programar/PROJETOS/AULA FLEXBOX/4-justify-content.

## PARTE - 3 → PRÁTICA COM JUSTIFY CONTENT 2

Nessa aula nós trabalhamos com justify content e todas as sua variações, aplicando-os com o flex direction em column.

Para ver como ficou o código desse html siga esse caminho: Atalhos Área de Trabalho/Ferramentas para programar/PROJETOS/AULA FLEXBOX/4-justify-content.

## ESTRUTURA BÁSICA E PRÁTICA COM ALIGN ITEMS 
Trata do alinhamento dos itens de acordo com o eixo do container.

O alinhamento é diferente para quando os itens estão em colunas ou linhas.

Essa propriedade permite o alinhamento central quando estivermos no eixo vertical.

Nós contamos com alguns tipos de alinhamentos possiveis quando tratamos de align items, que são:

center - alinhamento dos itens ao centro.

stretch - padrão, os itens crescem igualmente.

flex-start - alinhamento dos itens no início.

flex-end - alinhamento dos item no final do container.

baseline - alinhamento de acordo com a linha base da tipografia dos itens.

Nessa aula nós também usamos todos esse alinhamentos citados acima, para vê-los basta você seguir o seguinte caminho: Atalhos Área de Trabalho/Ferramentas para programar/PROJETOS/AULA FLEXBOX/5-align-items.

Nós também alinhamos um item ao centro da tela, que é o ultimo elemento do nosso código. Para isso foram necessárias 2 novas class, que são: “.central” e “.central .item”.
