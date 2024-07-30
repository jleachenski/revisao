# GIT/GITHUB

# Repositorio

A pasta do projeto imbuida com o software git, que contem os arquivos e o histórico de alteração do projeto.

# Github

Hospedagem de repositório (Github, Gitlab e Bitbucket)

# Branches (Galhos ou Ramificações)

Linha de desenvolvimento paralela/independente do projeto/repositório (existe apenas em um projeto git), muito utilizada para o desenvolvimento em equipes, para um não afetar/alterar o trabalho do outro.

# Git

Ferramenta de software para versionamento/controle de versões de um projeto qualquer, quando se cria um projeto git, se cria automaticamente um repositório

# Comandos do Git

`git clone <url-do-repositorio-remoto>`:  Clone/Cópia de um repositório remoto (nesse curso, no Github) e cria uma pasta no local (inicializando um repositório local com o git)

`git add <nome-do-arquivo>`: Seleciona os arquivos que vão ser salvos no próximo commit.

`git commit -m "<mensagem-do-commit>"`: É a forma de salvar as alterações feitas no repositório/branch (local) onde o usuário está trabalhando (modificando arquivos), o git commit apnas salva as alterações selecionadas pelo commando git add

`git status`: Mostra para o usuário o estado atual (as mudanças feitas/selecionadas) do galho onde o usuário está trabalhando

`git branch <nome-do-galho>`: Cria um novo ramo/galho/branch de desenvolvimento no repositório atual
pull
`git branch`: Lista os galhos do repositório, e também mostra em qual galho você está.

`git checkout <nome-do-galho>`: Para mudar de galho atual (ir para outro galho de desenvolvimento).

`git branch -d <nome-do-galho>`: Remove um galho do repositório em que o usuário está trabalhando.

`git push -u origin <nome-do-galho>`: Manda/envia as alterações do local para a hospedagem/repo/repositório remota.

`git pull origin <nome-do-galho>`:  Faz o download das alterações do galho indicado no comando, as alterações baixadas são realizadas/inseridas no galho atual do usuário

`git init`: Cria um repositório local (repo inicial denominado master, não é igual ao Github que cria como main)

`git merge <nome-do-galho>`: "Junta"/merge as alterações do galho indicado no galho atual

# Pull Request

Ele é um pedido de merge dentro do repositório remoto (Github), se caso esse pedido de merge for aceito, resultará no merge dos galhos envolvidos.

# FUNÇÕES/MÉTODOS/PROCEDIMENTOS

Uma função evita a repetição de código, pois sempre que aquele código é necessário, ele pode ser invocado/chamado a partir da função. Deixa também o código mais organizado e significativo.

Um bloco de código nomeado, que pode ou não conter parâmetros/argumentos e pode ou não conter um retorno.

# Parâmetro

É a variável que quem invoca a função dispoẽ para ela, o parâmetro/argumento modifica o comportamento da função.

# Retorno

É o resultado (valor) que função retorna para quem a invocou

# function declaration

f1() // invoco a função antes de declará-la / funciona

function f1(<os parametros vem aqui>) { // sofre hosting - sofre o elevamento
    //qualquer código
    return // o retorno sempre é opcional e pode ser de qualquer tipo
}

# function expression

f2() // vai quebrar o código, acessando uma variável antes de defini-la

// função anonima
const f2 = function(<os parametros vem aqui>) { 
    //qualquer código
    return // o retorno sempre é opcional e pode ser de qualquer tipo
}

f3()

// arrow/lambda function
const f3 = (<os parametros vem aqui>) => {
     //qualquer código
    return // o retorno sempre é opcional e pode ser de qualquer tipo
}

// se apenas houver um parametro, pode-se remover os parenteses
// também se houver apenas uma linha de código, pode-se remover a declaração do bloco

const f4 = arg => console.log(arg)


# MÓDULOS

Módulo é um arquivo que contém código. Utilizado para organizar a aplicação/software em uma estrutura mais lógica e significativa.

Os módulos/arquivos por padrão não se comunicam entre si, deve-se utilizar funções para exportar e importar o código de outro arquivo.

# Importar

// coloca o código exportado do arquivo modulo.js na variável mod
const mod = require("./modulo.js") // o .js em node é opcional, porém é uma boa prática sempre colocá-lo.

# Exportar

module.exports = {
    // exportando a função/variavel f1, onde outros arquivos poderão utilizá-la agora
    f1,
}