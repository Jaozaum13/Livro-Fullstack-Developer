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

PARTE - 2 → PRÁTICA COM FLEX DIRECTION
