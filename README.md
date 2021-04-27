# Anotações importante sobre Git e Github

## Configurando
- username: `git config --global user.name "username"`
- email: `git config --global user.email "email"`
- editor: `git config --global core.editor "editor"`
- Exibir username: `git config user.name`
- Exibe email: `git config user.email`
- Exibe lista de configuração: `git config --list`

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

[1](lifecycle_git.png)

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

## Desfazendo edições
- Estudar um pouco mais esse assunto

## Fontes 
https://www.udemy.com/course/git-e-github-para-iniciantes/
