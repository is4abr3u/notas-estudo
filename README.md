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
 eval"$(ssg-agent -s)"
```
agora adicione a chave ssh ao agente, com este código:

```
