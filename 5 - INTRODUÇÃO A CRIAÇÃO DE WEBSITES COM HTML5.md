# INTRODUÇÃO A CRIAÇÃO DE WEBSITES COM HTML5
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
