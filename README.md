# notas-estudo
minhas notas de estudo do técnico senac 2026


markdown

## Configurndo git 

Para ultilizar o git na minha maquina qu preciso configurar determinados comandos, sendo eles: 

```bash
git config --gobal
```
```bash
git config --global user.name "seu nome"
git config --global user.email "seuEmail@gmail.com"
```
depois é nescessariáio criar uma conta no site oficial do github 

hattps://github.com

## criando chave ssh

 Feito isso, deve-se configurar a maquina com a chave ssh com os seguintes comandos:

ultilize esse código para verificar se já existe chave ssh:
 ```bash
 lS -al ~/.ssh
```
para adicionar uma nova chave escreva o cógdigo:
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```
 para inicializar o agente-ssh digite:

 ```bash
 eval "$(ssg-agent -s)"
```
agora adicione a chave ssh ao agente, com este código:

```bash
ssh-add ~/.ssh/id_ed25519
```
para copiar a chave ssh digite:
```bash
clip < ~/.ssh/id_ed255519.pub
```
## Adicionando a chave no github

Primeiro acese o gitbub no seu navegador, e entre na sua conta do github(nessa conta deve constr o mesmo email que voce programou) Depois entre em settings, depois entre em SSH and GPG key, e em seguida clique em colar, coloque um titulo e identifique a chave (interessante colocar o local fisico onde a chave está, poe exemplo: senac-sala-106)

markdown

## Atalhos 

```bash

contol + d = seleciona todas as palavaras iguais de um qrquivo se eu quiser mudar
control + k + control +o = abre a pasta de arquivos para salvar as notas 
control + c = copiar 
control + v = colar 
control + z = desfazer a última ação realizada 
control + s = salvar anotações desde de a última alterção

markdonw 

## Revisão
 
Conteúdo da avaliação
 
Git hub
 
1 passo
 
Primeiro abra o seu git hub no navegador
Depois clica no foto de perfil
Criar um repositório
Nome do repositório (Exemplo de batata ) sem caractere especial
Descrição ( aquilo que vai ter no repositório ) ( ex : aula para avaliação )
Depois marque o redame e sempre em public.
 
2 passo  ( Clonar  )
 
Vai no repositório que tu criou e vai no code e copia o código
Depois vai no git bash 
 
Vai colocar esse comado :
 
$ cd documents/
 
$git clone , botão direito e cola
 
Depois o nome do repositório , enter
 
Vai aparecer o ( main ) , depois
 
Code .( código )
 
Pronto abriu o teu vs code
 
3 passo ( criar pastas ) 
 
Vai ter a pasta readme.md
 
Clica no vazio e cria um
 
Clica com o botão direito new file , ( index.html )
Depois vai no espaço vazio , botão direito new folder ( script )
Em cima do folder ( script ) clica em new file e cria ( nome da avaliação.js )
 
4 passo ( configurando o index.html )
 
Vai no index.html
 
Digita lá ( Ctrl 1 = ! )
 
La em cima em ( lang ) vai estar em ( en ) = english
Muda para “ pt-br”
 
Depois disso vai em baixo do    ( <body> )
Em baixo do body digita script
 
PRESTA ATENÇÃO !!!!!
Vai estar assim <script>
Você vai fazer isso aqui = <script src
Depois disso você vai escrever esse comando ( src="./scripts/avaliacao.js" )
E vai selecionar script>/avaliação
 
Depois disso você vai fazer o botão
 
Escreve “button” vai aparecer <button></button>
Dentro dessa merda aqui ( > )
 
Dentro dessa merda ali você vai escrever(  ID=”exercicio1” )
Depois da control V nesse código que você fez !!
 
<button id="exercicio1" >exercicio 1</button>
<button id="exercicio2" >exercicio 2</button>
<button id="exercicio3" >exercicio 3</button>
 
Só muda depois os número né
 
5 passo  ( dentro da pasta da avaliação )
 
function exemplo1( ) {
alert("funcionou aqui ")
}
 
Primeira coisa que você vai fazer é essa função
 
Depois disso vai por esse código aqui
 
const buttonexemplo1 = document.getElementById("exercicio1") //
buttonexemplo1.addEventListener('click', () => { exemplo1() }) //aqui faz referencia ao nome da function 
 
