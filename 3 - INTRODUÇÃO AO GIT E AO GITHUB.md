# INTRODUÇÃO AO GIT E AO GITHUB
## ENTENDO O QUE É GIT E SUA IMPORTÂNCIA
O GIT foi criado em 2005 e é um sistema de versionamento de código distribuído, e ele foi criado por Linus Torvalds, o criador do Linux.

O Linus não foi a pessoa que inventou o sistema de versionamento de código, mas foi a pessoa que criou o sistema de versionamento de código do GIT, pois estava muito descontente com o sistema de versionamento da época dele. Ele estava trabalhando para desenvolver o Linux e tinha membros de sua equipe distribuídos pelo mundo inteiro, sendo assim eles precisavam de compartilhar versões do mesmo código em tempo real e muitas vezes sendo editadas mesmas linhas do código em diversas localizações do mundo.

Sendo assim, o Git foi criado sobre o contexto de trabalho em equipe para desenvolver um software, ou seja, softwares são criados em conjuntos e nunca em trabalhos de uma pessoa solo.

O GIT e o GITHUB não são a mesma coisa. O GIT é o código do software de versionamento de dados, enquanto que o GITHUB é a empresa que vai armazenar o seu repositório nas nuvens da Microsoft.

## COMANDOS BÁSICOS PARA UM BOM DESEMPENHO NO TERMINAL
Muitos softwares de hoje usam o GUI (Grafical User Interface), que é uma interface gráfica para o usuário conseguir interagir, onde ele pode arrastar, puxar, clicar, etc. Porém o software que usaremos (GIT) não tem essa interface de interação com o usuário, e sim adota o CLI (Command Line Interface) que é a linha de comando como interação com o usuário.

Dentro do CLI nós iremos aprender os seguintes conceitos:

-   Mudar de pastas
-   Listar as pastas
-   Criar pastas/arquivos
-   Deletar pastas/arquivos

Para abrir o Prompt de comando do Windows, basta você ir no campo de pesquisa localizado na barra de ícones e digitar “cmd”.

Se você digitar “dir” no Prompt de comando, ele irá listar todas as pastas que estão dentro do seu usuário atualmente logado, sendo assim, você conseguirá localizar-se.

Se você digitar “cd /” no Prompt, você conseguirá navegar diretamente para a base do diretório, deixando assim de localizar-se em um usuário específico dentro do seu SO.

Para mover-se para dentro de uma pasta específica basta você digitar “cd + o nome da pasta”. Depois que você localizar-se dentro de uma pasta, você pode digitar o “dir” para listar todos os itens presentes dentro dessa pasta.

Para voltar para o repositório anterior basta você digitar “cd ..” para retroceder.

Conforme você vai navegando no Terminal, você vai perceber que ele vai ficando sujo, carregado. Então se você digitar o comando “cls” no terminal, você irá limpá-lo, assim ficando mais fácil a navegação dentro do mesmo.

Na plataforma Bash, do Windows, da pra você utilizar a tecla TAB para auto completar os nomes que deseja encontrar de pastas/arquivos. Como por exemplo, se você digitar “cd + W (maiúsculo) + TAB”, a plataforma automaticamente encontrará o a pasta WINDOWS e completará o nome para você. Assim facilitando o seu trabalho e evitando erros humano na digitação.

Para criar pastas dentro da plataforma, basta você digitar “mkdir”, dar espaço e digitar o nome que vocês querem dar a pasta. Ao dar enter é provável que nada aconteça, se o terminal não falar nada é porque o processo que você estava realizando deu certo.

Para criar arquivos direto de dentro da plataforma, basta você digitar o comando “echo + o nome do arquivo + . +o tipo do arquivo (por exemplo .txt para arquivos de texto).

Para deletar arquivos, basta você ir para a base dos repositórios (C:/) e digitar o comando “del + o conteúdo do repositório que você deseja deletar”. Lembre-se que esse comando deleta só o conteúdo do repositório e não o repositório inteiro, então tenha atenção, pois ele vai deletar tudo de dentro daquele repositório selecionado.

Você pode usar a seta para cima para navegar por todos os comandos executados naquele terminal e assim você conseguirá restaurar arquivos que excluiu antes de fechar a plataforma.

Para remover repositórios basta você digitar o comando “rmdir + o nome do repositório +/S +/Q.

As duas flags que foram usadas acima são para dizer a Plataforma que ela pode excluir todas as pastas presentes dentro do repositório “Workspace” e para dizer que não precisa aparecer nenhuma confirmação.

-   TERMINAL DO GIT BASH

No terminal do Git BASH, se você utilizar o comando “pwd” ele irá listar exatamente o caminho que você está percorrendo. Já o comando “ls” é usado para listar todos os itens que estão dentro daquele diretório.

Para criar uma nova chave SSH, você entra no Git Bash e adiciona o seguinte comando: “ssh-keygen -t ed25519 -C + o email que você usa na conta do GitHub.

Para tudo funcionar, você precisa inicializar o SSH agent que vai ficar responsável por lidar com todas as chaves. Para inicializa o SSH agent, você precisa usar o seguinte comando: “eval $(ssh-agent -s)” e ele irá dar start em um novo processo. Com o processo iniciado, você precisa dar as chaves para ele, para fazer isso você precisa listar as chaves e digitar a chave privada no seguinte comando: “ssh-add + a chave privada”, assim, sempre que chegar uma mensagem criptografada, o agente ficará responsável por descriptografar essa mensagem usando a chave privada.

Para clonar um repositório usando o SSH, você precisa escolher na opção “code” do GitHub a opção “SSH” ao invés de “HTTPS”. Depois você copia o link daquele repositório e cola no GIT BASH com o seguinte comando: “git clone + o link do repositório.

PARA LIMPAR O TERMINAL DO GIT BASH, VOCÊ USARÁ O ATALHO CTRL + L.

Flag -a para ver arquivos ocultos dentro de um repositório.

Para checar a configuração do git, basta você usar o comando git config --list e o git irá listar muitas coisas, entre elas estão o seu nickname e seu email.

## TÓPICOS FUNDAMENTAIS PARA ENTENDER O FUNCIONAMENTO DO GIT
Existem 4 tópicos fundamentais do GIT, que são:

-   SHA1
    
    A sigla SHA1 significa Secure Hash Algorithm (Algoritmo de Hash Seguro), é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos Estados Unidos. A grosso modo: o SHA1 vai pegar qualquer tipo de arquivo e embaralha-lo de uma forma muito específica.
    
    Ele se torna tão importante para nós pois, a encriptação gera um conjunto de caracteres identificador de 40 dígitos. Sendo assim, se você tiver um arquivo de texto muito grande e você usar o SHA1, ele será reduzido a uma chave de 40 caracteres único. O que tornará mais fácil do GIT encontrar tal arquivo, além de encurtar o mesmo.
    
    O comando para utilizar o SHA1 é:
    
    “openssl + sha1 + nome do arquivo com o tipo dele no final (ex: .txt)”
    
    Se você usar o comando SHA1 em um arquivo e depois mudar uma virgula desse arquivo e usar SHA1 novamente, ele irá gerar duas chaves diferentes, mas se você voltar a configuração inicial ele irá gerar o mesmo código.
    
-   OBJETOS FUNDAMENTAIS
    

No GIT nós temos três tipos básicos de objetos, que são:

-   BLOBS

Cada arquivo no **Git é** armazenado como um objeto **blob**, por exemplo, a partir do conteúdo do arquivo logo. png ele gera um hash que será armazenado em algum lugar endereçável como aa1b2fb696a831c89c53f787e03d863691d2b671 . O mesmo ocorre com o arquivo app.

-   TREES

As TREES armazenam e apontam as estruturas de Blob diferentes. Além de guardar os Blobs, a Árvore (Tree), também é responsável por guardar o nome do arquivo. Os Blobs só guardam os Shad dos arquivos. Então a Árvore é a responsável por montar a estrutura para armazenar os arquivos e onde estão organizados.

As Árvores pode apontar tanto para os Blobs quanto para outras Árvores, pois dentro de um diretório pode haver outro diretório.

As Árvores também tem um sha1 criptografado das árvores, então se você mudar um alguma coisa de um arquivo, você irá mudar toda a estrutura desse arquivo, Blobs, Árvores, etc.

-   COMMITS

O Commit é o objeto que vai juntar tudo, ele irá dar sentido para o que você está fazendo.

O Commit pode apontar para uma Árvore, para um parente (commit anterior a ele), para um autor, para uma mensagem.

O Commit também possui uma encriptação que é a geração do Hash do se código identificador de 40 caracteres.

Como todo Commit aponta para um familiar dele e isso forma uma estrutura de Commits, é impossível alguém de forma maliciosa alterar o seu código sem que você saiba, pois você terá a linha do tempo dos Commits e a chave de 40 dígitos será alterada. Por isso o Git é tão confiável.

Esses são os objetos que são responsáveis pelo versionamento do nosso código.

-   SISTEMA DISTRIBUÍDO SEGURO

O Git é um Sistema Distribuído Seguro, pois os Commits são quase impossíveis de ser alterados, então se você tiver um código sendo distribuído com 30 pessoas no mundo, todos as versões dos 31 programadores será extremamente confiável.

## CHAVE SSH E TOKENS
Esses dois conceitos referem-se diretamente ao GitHub e não ao GIT. Acontece que visando trazer mais segurança para seus usuários, o GitHub decidiu abandonar a forma de autenticação de usuário por Nome do Usuário e Senha. Mas dentro do Git você ainda poderá usar este tipo de autenticação caso queira, pois a mudança foi decidida apenas pelo GitHub.

-   O QUE SÃO CHAVES SSH

Chave SSH é uma forma de estabelecer uma conexão segura e criptografada entre duas máquinas. Que no nosso caso são os servidores do GitHub e nossas máquinas. Sendo assim, precisamos configurar nossa máquina para o GitHub entender que ela é uma máquina segura, para isso necessitamos da criação de duas chaves, uma pública (que você irá colocar no GitHub), e uma chave privada. A partir dai, o GitHub irá reconhecer a nossa máquina, então qualquer repositório que você tiver no computador, você conseguirá manda-lo para o GitHub. Com essa conexão estabelecida, você não precisará nem colocar senha.

## INICIANDO O GIT E CRIANDO UM COMMIT
Nesta aula nós vamos executar nossos primeiros comandos no Git. Faremos os seguintes comandos:

-   Iniciar o Git
-   Iniciar um versionamento
-   Criar um Commit

Para iniciar o repositório do Git, você precisa ir até a pasta (repositório) que deseja, pela plataforma do Git Bash e utilizar o seguinte comando “git init”. Pronto! Você iniciou o repositório Git na pasta desejada, porém, se você der um ls dentro dessa pasta não mostrará nada, pois esse repositório do git é uma pasta oculta. Para você conseguir vê-lo, é necessário usar a flag “ls -a”.

Antes de você criar um arquivo, o Git solicitará um Nickname e um email para te identificar como autor daquele commit.

-   Para identificar o email, você usará o seguinte comando: “git config --global user.email “o seu email"”.
-   Já para definir o Nickname, você usará o seguinte comando: “git config --global [user.name](http://user.name/) + o seu Nickname.

Trabalharemos com o Markdown, que é uma forma bem parecida, mas mais simples de se escrever HTML. Todo arquivo Markdown tem a extensão “.md” e definiremos o software Typora para ler esse tipo de extensão.

Para definir um título principal no Typora, basta você digitar “CTRL + 1” ou para definir título de outros tamanhos, basta você digitar “CTRL + o número (tamanho) que deseja”.

Para deixar em negrito basta digitar “** + texto + **”.

Para deixar em itálico basta digitar “_ + texto +_”.

Para fazer lista numerada com as bolinhas basta digitar “ - “.

Para fazer um commit desse arquivo, você precisa usar os comandos “git add *” e depois “git commit -m “commit inicial”.

## PASSO A PASSO NO CICLO DE VIDA
Nesta aula entenderemos melhor o que acontece com cada operação que vimos na aula anterior.

Dois conceitos bem importantes para entendermos são os de Tracked e Untracked. Tracked é aquele arquivo rastreável pelo Git e Untracked é aquele arquivo que o Git não consegue rastrear.

Dentro dos Trackeds, temos três categorias: unmodified, modified e staged.

-   Unmodified é o arquivo que ainda não sofreu modificação.
-   Modified é o arquivo que já sofreu modificação. Automaticamente, quando você abre o arquivo e o modifica, ele muda de Unmodified para modified.
-   E o Staged é aonde os arquivos que estão se preparando para fazer parte de outro agrupamento ficam.

Quando nós usamos o comando “git init”, nós tornamos aquele arquivo tracked pro Git, pois antes nós só tínhamos criado o arquivo [Batatalhoada.md](http://Batatalhoada.md). Quando usamos o comando “git add”, nós mandamos o arquivo direto pro staged, pois ele estava naquele estagio de esperar o próximo agrupamento que iria.

Quando nós movemos o arquivo para Staged, ele está se preparando para fazer parte de um commit. Então quando nós colocamos um objeto em Backstage e adicionamos um autor para ele, uma data, uma descrição. Ele deixa de ser Staged para se tornar um Commit. E o Commit retorna todos os arquivos para Unmodified novamente, pois está esperando você editá-lo novamente e assim por diante. Sendo assim, Unmodified, modified e Staged, formam um ciclo.

Nós temos a separação em dois ambientes que o 1° É o ambiente da nossa máquina e o 2° É o servidor. E é aqui que diferencia quando você faz alguma mudança na sua máquina e essa mudança não interfere no servidor, a nãos ser que você execute um conjunto de códigos específicos para realizar essa mudança.

No Ambiente do Seu Computador tem o Diretório de Trabalho que é o diretório que você está trabalhando agora, a Staging Area que é a area aonde os arquivos ficam esperando para descobrir aonde irão, como falamos acima, o importantíssimo Staged. E quando este arquivo se torna um Commit, ele passa a ser o Repositório Local, que pode ser empurrado para um Repositório Remoto, saindo do seu Ambiente de Máquina e indo parar no Servidor. Lembrando que dentro do Repositório Local só são aceitos Commits, para assim irem para o Repositório Remoto.

Ok, vimos tudo isso, mas como saber em qual desses estágios meu arquivo está? Para isso você vai usar o comando “git status” e ele vai apresentar diversas informações sobre o arquivo.

## TRABALHANDO COM O GITHUB
É interessante que o seu email e o seu nickname do Git e do GitHub estejam sempre de acordo, pois assim você terá mais facilidade na hora de empurrar um commit para o Repositório Remoto, depois que você definiu seu Nickname no Git, para mudá-lo, basta você usar o comando “git config --global [user.name](http://user.name/) "o nickname desejado". O mesmo serve para o email.

Para entrar nas configurações e ver seu email e nickname, basta usar o comando “git config — list”.

Para colocar o arquivo do Repositório Local para o Repositório Remoto, você entra no GitHub e vai em Your Repositories (Seus Repositórios), clica em New (Novo), escolhe as configurações do seu novo repositório em nuvem, pega a URL do seu repositório em “...**or push an existing repository from the command line”, abre o Git Bash e digita o seguinte código, “git remote add origin nome do repositório + a URL do repositório que você pegou no GitHub”. Para ver se deu certo, você o usa o código “**git remote -v”, se aparecer essas mensagens: ”origin livro-receitas (fetch) origin livro-receitas (push)”, significa que ta dando certo.

Agora você precisa empurrar o arquivo para o Repositório Remoto, para isso, você vai usar o comando “git push origin master”.

## COMO OS CONFLITOS ACONTECEM NO GITHUB E COMO RESOLVÊ-LOS
Os conflitos são bem comuns nos sistemas de versionamento de código, mas não se preocupe pois não é um bicho de 7 cabeças.

Imagina que você e mais uma pessoa estão mexendo no mesmo código, na mesma hora, no momento em que vocês mandarem esse código pro GitHub, ele irá pegar ambos e juntar as alterações, a não ser que tenha duas alterações na mesma linha, ai o GitHub deixa você ir pegar aquele código para alterar aquela linha.

Quando tiver alguma alteração no seu repositório no GitHub, você não conseguirá empurrar novas alterações para esse repositório, a não ser que puxe a alteração do GitHub primeiro. Para fazer isso, use o comando “git pull origin master”.

COMO BAIXAR O CÓDIGO DO GITHUB PARA MEXERMOS NELE?

Você seleciona o repositório que tem interesse e clica em “CODE”, você vai ter diversas opções, abrir com CODESPACE, GITHUB ONLINE E BAIXAR ZIP, mas nós queremos baixar ele com a plataforma do Git Bash, então copia a URL dele e abre o Git Bash. Agora você vai navegar até a pasta que deseja colocar o repositório e use o comando “git clone + URL do repositório”, simples assim. Quando você baixa um repositório ele já vem com uma pastinha .git, o que mostra para onde este repositório está apontado, isso é que vai diferenciar aquele arquivo de uma simples pasta.
