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

isadora61190376@JLE106D060741 MINGW64 ~
$ cd documents/
isadora61190376@JLE106D060741 MINGW64 ~/Documents
$ git clone git@github.com:is4abr3u/Outrorepo.git
Cloning into 'Outrorepo'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

isadora61190376@JLE106D060741 MINGW64 ~/Documents
$ cd Outrorepo/

isadora61190376@JLE106D060741 MINGW64 ~/Documents/Outrorepo (main)
$ code .

isadora61190376@JLE106D060741 MINGW64 ~/Documents/Outrorepo (main)
$ ^C

isadora61190376@JLE106D060741 MINGW64 ~/Documents/Outrorepo (main)
$

// ---------------------SOBRE REACT------------------//

npm create vite@latest

crie um novo repositorio e clone 
ignore files and continue 
selecione react 
selecione javascript 
selecione yes
depois faz: npm install 
e dps: npm run dev 
agora crie a pasta componentes

faça 3 pastas dentro- footer/list/header

import './style.css'

function Footer() {
    return (
      <footer id='Footer'>
        <p>Minha primeira API react - &copy; Todos os direitos reservado</p>
      </footer>
    )
}
export default Footer

na pasta list

import './style.css'

function Section({
  title, 
  subtitleSecondList
}) {
  return (
    <section>
      <h2 id="exemplo-h2">{title}</h2>
      
      <h3>
        {subtitleSecondList }
      </h3> 

      <ul id="ul">
        <li>Brownie</li>
        <li>Bolo de cenoura</li>
        <li>Kiner Bueno white</li>
      </ul>

      <h3>Coisas que eu mais gosto de fazer em casa:</h3>
      <ol>
        <li>Tomar banho e ficar cheirosa</li>
        <li>Comer</li>
        <li>Dormir</li>
      </ol>

    </section>
  )
}
export default Section

in pages/ about 

import { Link } from 'react-router-dom'
import './style.css'

function About() {
    return (
        <>
            <>OUTRA PÁGINA</>
            <Link to="/">
                <button >Back to home page</button>
            </Link>
        </>
    )
}
export default About    

in app.jsx

import Footer from './componentes/Footer'
import Header from './componentes/Header'
import List from './componentes/List'
import './App.css'
import { Route, Routes } from 'react-router-dom'
import Home from './pages/Home'
import About from './pages/About'
import Singup from './pages/Singup'


function App() {

  return (
    <>
      <Header /> 
      
      <Routes>
        <Route path='/' element={<Home />} />
        <Route path='/about' element={<About />} />
        <Route path='/signup' element={<Singup />} />
      </Routes>

      <Footer />
    </>
  )
}

export default App

in pages/signup

import { useState } from "react";
import "./style.css";

function Singup() {
    const[ nome,setNome ] = useState("batata")
    const[email,setEmail] = useState("batata")
    const[senha, setSenha] = useState("batata")
    const [resultado, setResultado] = useState()
    //variaveis e funçoes criar aqui 
function handleSubmit(event) {
event.preventDefault();
console.log(nome, email, senha)
setResultado(nome);
}
    return (
        <>
            <h2>Cadastro</h2>
            <form onSubmit={handleSubmit}>
                <label>Digite sue nome completo:</label>
                <input
                    type="text"
                    value={nome}
                    onChange={(e) => setNome(e.target.value) }
                />
                <label>Informe seu e-mail</label>
                <input
                    type="e-mail"
                    value={email}
                    onChange={(e)=> setEmail(e.target.value) }
                    
                />

                <label>Crie uma senha</label>
                <input
                    type="password"
                    value={senha}
                    onChange={(e)=> setSenha(e.target.value) }
                />
                <p>{resultado}</p>
<button type="submit">Cadastre-se</button>
            </form>
        </>
    )
}
export default Singup

in pages/ home

import { Link } from 'react-router-dom'
import './style.css'

function Home() {
    return (
        <>
        <h2>Bem vindo ao meu sistema</h2>
        <Link to="/about">
        <button >Go to about page</button>
        </Link>
        </>
    )
}

export default Home

 
