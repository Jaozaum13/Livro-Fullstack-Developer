# INTRODUÇÃO A CRIAÇÃO DE WEBSITES COM HTML5

## HTML5

## ESTRUTURA BÁSICA
A HISTÓRIA DO HTML

O HTML foi criado em 1991 por Tim Bernes-lee. O HTML surge da necessidade de Tim em compartilhar algumas informações com seus colegas de trabalho.

O processo de criação do HTML não foi muito rápido, Tim começou a esboçar a linguagem em 1980, mas só apresentou o HTML em 1991. Desde 1991, surgiram 5 versões. Sendo a mais atualizada de 2014.

APROFUNDANDO EM HTML

Para escrever em HTML precisa entender como funciona um elemento, o elemento é a base do HTML. Tudo dentro do arquivo HTML é um elemento.

ESTRUTURA DO ELEMENTO HTML

Para se iniciar um elemento HTML, nós usamos uma tag de abertura dizendo qual é o tipo daquele elemento, o que ele irá fazer. Essa tag pode ainda conter um atributo, que muda uma funcionalidade, aparência ou dizer algo ao navegador. Logo após, nós temos o conteúdo do elemento e por fim a tag de fechamento.

!DOCTYPE html

html

head

meta

title title

head

body

body

html

Na escada acima temos a estruturação do elemento HTML. Nela temos de inicio o comando chamado “!DOCTYPE html” que não é o elemento HTML ainda, você só está dizendo ao navegador o que você está escrevendo. Logo após, nós temos a abertura da tag do elemento HTML, aonde todo o nosso conteúdo estará dentro. Depois nós iniciamos o elemento, dentro desse elemento nós teremos algumas metas informações, informações que um navegador necessita. No exemplo, temos a tag, que tem várias funções, uma delas é o “charset”, que consiste em como o navegador vai fazer o encode dos caracteres. Em seguida, abrimos a tag title , essa tag fica encarregada de colocar o título na aba do navegador, por fim, fecha-se a tag title e também o elemento head. Por último, nós abrimos o elemento body, que é aonde ficará contido todo o conteúdo da nossa página, o fechamos e fechamos o elemento html. Assim temos a estrutura básica.

Proposto o exercício de criar a estrutura básica de um site pessoal.

## SEMÂNTICA PARTE 1 E 2
AULA 002 PARTE 1

Durante muitos anos, os desenvolvedores tinham de usar como elemento padrão “divs”, isso transformava tudo numa bagunça, pois eles indicavam “div” em toda linha e tinham de buscar significado para os elementos de outra formar, como dentro de classes, todo esse processo deixava o código bem mais sujo e mais complexo para o entendimento.

Com o HTML 5, isso mudou, eles adicionaram outros elementos que trouxeram mais significados para o HTML. Alguns deles são:

Section

Representa uma seção genérica de conteúdos, como por exemplo, uma lista de artigos.

Header

Usado para definir o cabeçalho da sua página ou de uma section dentro da sua página.

Article

representa um conteúdo relevante dentro da sua página, como um artigo de um blog.

Aside

Representa um conteúdo relacionado ao conteúdo principal da sua página, como uma biografia de um autor, links relacionados e é representado normalmente por uma barra lateral.

Footer

Que pode ser o rodapé da sua página ou de sections da sua página.

H1 - H6
 
 Representa a importância de um título da sua página, por exemplo o h1 pode representar o título principal da sua página, o h2 o título de uma section e o h3 o título de um artigo. Pode ser usados como bem entender, porém só pode haver 1 h1 por página.

AULA 002 PARTE 2

Proposto o exercício de aprimorar a estrutura do site pessoal.

## TAGS PARA TEXTOS	
A estilização de texto e link dentro de um site é algo extremamente importante, pois pode ajudar a deixar o site mais fluído visualmente, além de deixá-lo mais bonito. A seguir serão mostrados algumas tags de textos e links para incrementar seus sites.

H1 - H6

Como já citado na aula anterior, as tags de h1 - h6 podem ser usadas para modificar o tamanho dos seus textos, sendo h1 o mais importante e podendo haver apenas 1 por página e todas as outras podendo ser usadas inúmeras vezes.

P

<p> - Utilizado para acrescentar textos mais complexos e longos ao seu site, como parágrafos. Ele suporta também outros tipos de arquivo, como imagens, códigos, vídeos e vários outros tipos de conteúdo.

## TAGS PARA LINKS
Outro elemento extremamente necessário na Web é o “a”.

A

Este elemento é a âncora, que interliga vários conteúdos na Web. Este elemento contém vários atributos, entre eles estão o “href” e o “target”.

HREF

“href=” - Este atributo é o hiperlink para onde sua âncora está apontando, pode ser uma página no seu site ou um site externo. Ele pode apontar também para emails e até telefones.

Quando este atributo aponta para um email, tem de ser usado um prefixo, que é o “mailto:” (mail para, do inglês) + email apontado.

Quando este atributo for apontar para um telefone, o prefixo que precisa ser utilizado é o “tel:” + telefone desejado.

Só lembrando que a estrutura com o atributo href e target ficará da seguinte maneira:

<a href =”link para o qual quer apontar”> + texto que criará o hiperlink + a

a target=”blank” + texto que criará o hiperlink + a

TARGET

“target=” - Este atributo serve para indicar como o nosso link vai ser aberto, inicialmente aprenderemos somente um valor, que é o “_blank”, ele diz para nossa página abrir esse link numa nova aba.

O exercício proposto será adicionar um texto a nossa página e adicionar alguns links dentro desse texto.

## TAGS PARA IMAGENS
Agora a questão é como representar imagens na Web? Simples! Basta você usar a tag img.

IMG
 Essa tag é usada para representar as imagens do seu site, uma informação importante de saber é que esse elemento não possui tag de fechamento, logo você so precisa abri-lo. Este é um elemento bem simples e que possui apenas 2 atributos próprios, que são o sourch e o alt.

Sourch

img src=”img/avatar.jpg” - Este é um atributo obrigatório, pois guarda o caminho da imagem, pode ser uma imagem dentro do seu próprio site ou de outro lugar.

ALT

<img alt=”foto de João Gabriel”> - Mesmo esse não sendo um elemento obrigatório, ele é recomendado por melhorar a acessibilidade, ele mostra a descrição da imagem quando ela não é carregada e leitores de tela usam essa descrição para mostrar para os usuários o que ela significa.

Proposto o exercício de adicionar uma imagem ao cabeçalho da página e outra a postagem.

DICA: Despois de escolher as imagens, vá até o site TinyPNG e passe elas lá para retirar informações desnecessárias delas e assim deixar mais leve.

## TAG PARA LISTAS LI, UL E OL
Listas servem para agrupar coleção de itens, como por exemplo, uma lista de ingredientes ou como veremos, uma lista com contatos.

UL

Representa uma lista em que a ordem dos itens não é importante.

OL

Representa uma lista em que a ordem dos itens é importante, portanto eles são representados por números, letras ou algarismos romanos.

LI

É um item dessas listas.

Proposto o exercício de adicionarmos uma lista de contatos no rodapé do nosso site pessoal.

# CSS3

## INTRODUÇÃO AO CSS3
Após a criação do HTML, a necessidade de formatar páginas ficou bem clara. A sintaxe é bem simples, você cria regras de estilo para elementos ou grupos de elementos.

Uma regra CSS é formada por um seletor ou um grupo de seletores, os seletores são apenas elementos HTML . Então dentro de um par de chaves ( {} ), nós temos as declarações. As declarações são formadas por uma propriedade e por um valor.

![Estrutura de um CSS.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/92337c78-8d88-47c8-8f09-cc04401e693a/ESTRUTURA_DO_CSS.png)

Estrutura de um CSS.

No exemplo acima vimos que “a, p, h1, h3”, são os seletores. E as declarações são as duas linhas entre colchetes. Aonde as funções “color” e “font-size” são as propriedades e “blue” e “14px” são oa valores. Nota-se que com essa estrutura muda-se a cor dos textos daqueles seletores e o seu tamanho, porém isso significa que qualquer elemento HTML desses tipos dentro daquela página irão ter essa aparência. Se você procura modificar apenas 1 elemento, porém existem mais de 1 desse elemento na sua página, precisará usar ID E CLASS.

ID E CLASS

Os ID E CLASS podem representar qualquer tipo de elemento. Para declarar o seu ID ou CLASSE no HTML, você usa a palavra ID/CLASS. Já para declara-los no CSS, você usará a tecla “.” (para o CLASS) e “#” (para a ID). Atente-se que o ID só pode ser usado 1 vez na página.

## CONCEITOS BÁSICOS
Quando programamos o layout de um site, o navegador representa cada elemento HTML como uma caixa retangular, chamado de box model. Com o CSS nós conseguimos alterar a aparência dessa caixa.

O Box Model tem 4 áreas, a margem, a borda, o padding e o conteúdo. As margens são os espaçamentos entre elementos. A borda circula o padding e o conteúdo e nós conseguimos mudar a aparência dela como largura e cor. O Padding é o espaçamento entre a borda e o conteúdo. O conteúdo é o que o seu bloco representa, um texto uma imagem ou um vídeo. Para enxergarmos o box model, iremos mudar as cores de alguns elementos no nosso site pessoal.

![Código CSS com todas as modificações que fizemos no HTML até o momento.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/46f35a55-d28b-45bc-afb7-44109f800375/CSS_CODE.png)

Código CSS com todas as modificações que fizemos no HTML até o momento.

Nota-se que quando chamamos o seletor body, adicionamos a propriedade background para modificar todo o fundo da página.

Quando usamos o seletor post, mudamos a cor do conteúdo, do padding, da borda e da margem.

![Print site pessoal.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ca9e5630-df76-4a7a-a56c-301c022895d2/PRINT_SITE_PESSOAL.png)

Print site pessoal.

Foi dessa maneira que ficaram as modificações.

## ESTILIZANDO ELEMENTOS
Agora vamos repassar pelas propriedades citadas para ver com maior detalhe e deixar nosso site mais bonito.

PADDING E MARGIN

Até então só usamos esses elementos com um único valor de tamanho, mas podemos adicionar tamanhos diferentes se quisermos. Existem 3 maneiras de fazer isso.

1°Maneira

Nessa primeira maneira, nós adicionamos um valor para a parte superior e inferior, depois para os lados esquerdo e direito.

![TAMANHO DE PROPRIEDADES NO CSS.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b88eaee9-e182-47ec-b9b8-a6a4994219ab/TAMANHO_DE_PROPRIEDADES_NO_CSS.png)

Nessa imagem o valor “10px” se refere ao eixo y, ou seja partes superior e inferior. Já o valor “5px” se refere ao eixo x, lados direitos e esquerdos.

2°Maneira

Nessa maneira nós adicionamos valores diferentes para cada lado.

![2°TAMANHO DE PROPRIEDADES NO CSS.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7f40cf39-199c-4447-9dea-a0b43af7eacf/2TAMANHO_DE_PROPRIEDADES_NO_CSS.png)

Nessa imagem o valor de “15px” descreve o topo, “10px” descreve a direita, “5px” descreve a parte inferior e 0 descreve a esquerda, note que quando o valor for 0, ele não necessita de unidade de medida.

3°Maneira

Nessa maneira você descreve item a item. Não existe uma explicação melhor.

![3°TAMANHO DE PROPRIEDADES NO CSS.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ed97721e-4fd3-4228-bec6-1d1784b3694b/3TAMANHO_DE_PROPRIEDADES_NO_CSS.png)

Essa maneira é mais usada quando temos um padding com 3 lados iguais e somente 1 diferente, pois ai usamos o padding/margem com um valor só e colocamos a propriedade exata do lado que queremos alterar.

BACKGROUND

Essa propriedade também possui vários atalhos, com ela podemos mudar a cor de fundo, colocar uma imagem, alterar posicionamento dessa imagem. O melhor lugar para estudar isso é o site da Mozila Develop Network (NDN). Por enquanto vamos somente mudar a cor de fundo, há algumas formas de fazer isso.

1°Maneira

Utilizando a propriedade “background-color” com o nome da cor em inglês.

2°Maneira

Utilizando a mesma propriedade, mas com o número hexadecimal daquela cor.

3°Maneira

Utilizando somente a propriedade “background” com o nome da cor em inglês ou usando o número hexa decimal dessa cor.

BORDER

A propriedade Borda contém 3 valores largura(representada em pixels, centímetros ou milímetros...), cor (representada por nome da cor em inglês ou número hexadecimal) e estilo (sólida, pontilhada, tracejada...).

![PRINT DE O CÓDIGO DE UMA BORDA.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0c94f5b7-67db-4887-828c-fac0e573ec0a/PRINT_DE_O_CDIGO_DE_UMA_BORDA.png)

Nós também temos a opção de descrever o tamanho de cada lado da borda, e assim, você pode colocar a largura, a cor e o estilo diferente em cada lado.

Também podemos mudar o aspecto de uma borda só acrescentando a propriedade borda e o nome do lado que queremos juntamente com a característica que buscamos modificar.

BORDER-RADIUS

Essa propriedade permite arredondar o canto do elemento. Com ele nós podemos usar várias unidades de medida, mas as mais comuns são os pixels e as porcentagens. Colocando apenas um valor nós alteramos todos os cantos de um elemento, mas se seguimos a mesma ordem vista no PADDING E MARGEM, topo, direita, inferior e esquerda. Uma dica interessante é que se você quer deixar um elemento redondo, basta colocar 50% que esse objetivo será atingido.

## ESTILIZANDO TEXTOS
Agora aprenderemos propriedades para editar nosso texto.

FONT-FAMILY

Essa propriedade serve para editar a fonte do seu texto, tanto fontes online quanto fontes já instaladas na sua máquina. Por enquanto vamos utilizar as Web Safes Fonts, que são chamadas assim pois se encontram na maioria das máquinas. Uma informação interessante é que você consegue listar 2 para o CSS, caso uma não esteja funcionando, a segunda entra como backup.

FONT-SIZE

O font-size altera o tamanho do nosso texto. Existem diversas unidades que podemos usar para definir o tamanho da nossa fonte, mas os pixels são os mais interessantes.

FONT-STYLE

Altera a aparência do nosso texto. O valor “normal” é o padrão, ou seja, ele irá mostrar a fonte do jeito que ela foi desenhada. O valor “italic” deixa a fonte um pouquinho mais inclinada. Sempre preste atenção se sua fonte tem suporte para itálico, pois senão, seu navegador irá forçar essa inclinação e não ficará bonito.

FONT-WEIGHT

Altera o peso do texto. Existem várias palavras chaves para o valor e alguns valores numéricos também, mas eles são usados quando temos fontes mais complexas com diversos pesos. Em fontes normais somente o valor “normal” e “bold” já resolvem. O NORMAL seria o peso comum dessa fonte, o jeito que ela foi desenhada e o BOLD é o negrito.

TEXT-TRANSFORM

Essa propriedade altera o tipo de caractere entre maiúsculo e minúsculo.

O valor UPPERCASE deixa tudo em caixa alta.

Enquanto que o valor LOWERCASE coloca todo o texto em caixa baixa.

Já o valor CAPITALIZE coloca todas as primeiras letras de cada palavra em maiúsculo.

TEXT-DECORATION

Essa propriedade é muita usada para dar destaque a algum texto, pois ele coloca linhas.

O valor UNDERLINE coloca uma linha embaixo da palavra.

O valor OVERLINE coloca uma linho sobre a palavra.

O valor LINE-THROUGH coloca uma linha cortando essa palavra ao meio.

## ESTILIZANDO LISTAS
Como ja vimos anteriormente, existem 2 tipos de listas, as ordenadas e as não ordenadas. Para alterar os marcadores dessas listas nós usamos o list-style type. A seguir veremos alguns exemplos de edição de listas com list-style-type.

LISTA NÃO ORDENADA

list-style-type: square; - esse exemplo altera o símbolo de um marcador para um quadrado (com a palavra “square”).

Nós podemos mudar um marcador por um símbolo com: list-style-type: “\1F44D”; - esse exemplo altera o marcador por um emoji de joinha.

Numa lista não ordenada nós também podemos trocar o marcador por uma imagem com o seguinte código: list-style-image: url(”rocket.png”);

LISTA ORDENADA

list-style-type: upper-roman; - nesse exemplo alteramos o marcador para números romanos.

## PROPRIEDADES DE DIMENSÃO E ALINHAMENTO
Dimensões e alinhamento são elementos extremamente importantes dentro do nosso site, então agora iremos aprender a modifica-los.

WIDTH E HEIGHT

Servem para editar a largura e a altura. Eles aceitam como unidade de medida tanto o pixel quanto a porcentagem indicando o tamanho do elemento que vem de fora dele.

MAX-WIDTH E MAX HEIGHT

Essas propriedades se refeream a largura máxima e a altura máxima que aquele elemento pode ter.

MARGIN

Essa propriedade serve para colocar espaçamento entre elementos, mas se você adicionar o valor auto, ele alinha o elemento automaticamente.

TEXT ALIGN

Serve para alinhar textos. Podemos usá-lo para alinharmos a esquerda com o valor left, a direita com o valor right, ao centro com o valor center e podemos justificar o texto com o valor justify.

