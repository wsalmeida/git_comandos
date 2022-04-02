# Anotações importante sobre Git e Github

## Configurando
- username: `git config --global user.name "username"`
- email: `git config --global user.email "email"`
- editor: `git config --global core.editor "editor"`
- Exibir username: `git config user.name`
- Exibe email: `git config user.email`
- Exibe lista de configuração: `git config --list`

Atenção:
Os arquivos de configurações do git se localiza na pasta `$USER` com o
nome de `.gitconfig` 

## Inicializando repositório
- Crie uma pasta para seu projeto: `mkdir projeto`
- Entre na pasta: `cd projeto`
- Inicie projeto: `git init`
- visualize projeto: `ls -la`

## File Status Lifecycle
- Untracked file: criado mas não reconhecido pelo git
- Unmodified: Naõ teve modificação
- modified: Editado mas não foi levado
- Stage Changes to be committed: Pronta para ser comitado

<p align="center"> <img src="https://github.com/wsalmeida/git_comandos/blob/main/src/lifecycle.png">

## Comandos básicos
- lista estado: `git status`
- adicionando arquivo: `git add <file>`
- comitando: `git committ -m "modificação"`

## Comandos de logs
- logs: `git log`
- logs com mais informações: `git log --decorate`
- logs pelo autor: `git log --author="nome_autor"`
- logs de autores e committ feitos: `git shortlog`
- logs numeros de committ: `git shortlog -sn`
- logs com gráficos: `git log --graph`
- logs especifico: `git show hash`

## Mudanças antes do committ
- visualiza modificação antes do committ: `git diff`
- visualize somente nome arquivo modificado: `git diff --name-only`

## Setar Token de Acesso pessoal
Token no git é um maneira segura de autenticação entrerepositórios local e 
remotos como esse comando você evita ficar digitando usuário e senha a cada push.
 - Crie o token no github `profile->settings->developer->settings-personal->
 acess token->generetion token` coloque não esxprira e marque dando todos permissões
 - Clone seu repositório remoto
 - Aplica as modificações locais e commit e push digitando usuário e senha
É necessaŕio realizar esse processo antes de setar o token depois disso basta
aplicar o comando para setar o token 
`git config --global credential.helper cache`
Após esse processo todos os push sobem sem a necessidade de digitar usuário e 
senha.

Esse tipo de configuração torna as configurações salvas somente quando a sessão
estiver ativa após o reinicio do sistema é necessaŕio repetir o procedimento

# Continua... seu 
