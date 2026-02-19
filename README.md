# notas-estudo
minhas notas de estudo do técnico senac 2026


markdown

## Configurndo git 

Para ultilizar o git na minha maquina qu preciso configurar determinados comandos, sendo eles: 

```bash
git --version
```

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

##
