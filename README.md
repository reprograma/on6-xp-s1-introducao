# on6-xp-s1-introducao

## Conceitos gerais

### Font-end
 
![GitHub Logo](https://cdn.cultofmac.com/wp-content/uploads/2016/10/CoM-The-Ultimate-Front-End-Development-Bundle-780x390.jpg)

O Front-end de uma aplicação é tudo aquilo que podemos enxergar através do navegador, logo definimos que a codificação do layout é responsabilidade do front-end, e para isso ele usa algumas tecnologias que são:
- HTML 
- CSS 
- Javascript - (**Vuejs**, **Reactjs**, **Angular**)

O código Front pode ser acessado pelo usuário, pois esse código fica todo do lado cliente, diferente do Back-end, e para realizar algumas funcionalidade o front se comunica com o Back-end através de requisições (pedidos).

### Back-end

![GitHub Logo](https://miro.medium.com/max/960/1*WyBYiUI5PlYJZIsOaWvebw.png)

O Back-end é a parte da aplicação que não é visível ao usuário, tratando das requisições feitas do lado Front-end, enviando, editando ou excluindo do banco de dados. No Back-end o código não pode ser acessado pelo lado cliente, sendo assim é a parte mais segura para poder trabalhar com o banco de dados.

Um exemplo de Back-end é quando vamos fazer o login, digitamos nossos dados e quando clicamos no botão para entrar, o Front-end faz um pedido para o Back-end para validar o usuário, com isso o Back verifica no banco a existência daquele usuário e se ele existir valida a senha, assim retornando uma chave de acesso caso tudo esteja correto ou  retorna um erro  se houver algum problema.

As principais tecnologias usadas pelo Back-end são:
- Java
- Python
- Ruby
- PHP
- Javascript (**Nodejs**)
- C#

### Banco de dados
![GitHub Logo](https://www.cetax.com.br/blog/wp-content/uploads/2016/04/dw.png)

Banco de dados são coleções de informações organizadas que podem se relacionar, ou seja, é um local onde armazenamos dados, que são organizados por assuntos. 
Os principais bancos:
- MySQL
- PostgreSQL
- SQLite
- MongoDB
- Redis

### Mobile
![GitHub Logo](https://s3-eu-west-1.amazonaws.com/engage-site-cms/craft/uploads/Blog/2018/Mobile-first-indexing/header.png?mtime=20180327170520)

Desenvolvedor Mobile é aquele que desenvolve aplicativos. Hoje temos dois sistemas operacionais que são android e o ios, cada um deles usam uma linguagem diferente para criar aplicações:
	Android - Kotlin (**Java**) 
	ios - Swift (**Objective-C**)
Essas são linguagens nativas para cada dispositivo, mas existem também outras que criam aplicações  híbridas para atender os dois tipos de dispositivos como:
- ionic (**Javascript**)
- Xamarin(**C#**)
- React Native (**Javascript**) 



## Termimal
![GitHub Logo](https://www.lucascaton.com.br/assets/images/2018/01/terminal-windows.png)

É através do terminal que podemos dar comandos ao computador, os comandos básicos são: 

- dir (windows)/ ls  - para listar os arquivos e pastas dentro de um diretório
- cd nome-da-pasta - para navegar entre diretórios
- cd .. -  sair de um diretório
- mkdir nome-da-pasta - cria uma pasta
- touch nome-do-arquivo - cria um arquivo
- del  nome-do-arquivo (windows) / rm nome-do-arquivo - deleta um arquivo
- rd nome-da-pasta (windows) / rmkdir nome-da-pasta - exclui um diretório
- cls (windows) /clear - limpa o terminal
- F7 (windows) / history - mostra o histórico de comandos


# Git & Github 

## Git
![GitHub Logo](https://media.giphy.com/media/kH6CqYiquZawmU1HI6/giphy.gif)

Git é um sistema de controle de versões distribuído, que permite versionar qualquer tipo de projeto. É uma ferramenta indispensável para um desenvolvedor, com ele podemos ter um histórico de tudo que já foi feito dentro do projeto.

### Instalação do Git
O git já vem instalado na maioria dos computadores Mac e Linux, se for o seu, apenas digite na linha de comando: git --version caso esteja instalado, esse comando mostrará a versão do git.

tutorial: https://woliveiras.com.br/posts/instalando-o-git-windows/

git para mac: https://git-scm.com/download/mac
git para windows: https://gitforwindows.org/
git para plataformas Linux/Debian, como o Ubuntu: digite na linha de comando _sudo apt-get install git_

### Git configuração
Para adicionar usuário:

git config --global user.name "fulano"
git config --global user.email “fulano@hotmail.com”
Para remover usuário:

git config --global --unset user.name "fulano"
git config --global --unset user.email “fulano@hotmail.com”

## GitHub
![GitHub Logo](https://media.giphy.com/media/du3J3cXyzhj75IOgvA/giphy.gif)

**GitHub** é uma plataforma de hospedagem de código-fonte com controle de versão usando o Git. Ele permite que qualquer usuário cadastrado na plataforma hospede seu código e contribua em projetos.

### Criando conta no GitHub
Acesse o link : [GitHub](http://github.com).

### Iniciando um projeto com Git

- No terminal dentro da pasta que vai conter todos os arquivos do seu projeto dê o comando ``git init``, com ele o git vai criar uma pasta oculta com o nome .git.
- Com o comando ``git status`` conseguimos ver o status do repositório que de início é ‘Untracked files’, esse status diz que não tem nenhum arquivo para ser rastreado ( para criar versões ).
- Para o arquivo ser rastreado usamos o comando ``git add nome-do-arquivo`` ou se desejar ``git add .`` que vai adicionar todos os arquivos de uma vez.
- Se dermos um ``git status`` novamente o status vai ser ‘Changes to be committed’, isso quer dizer que o arquivo pode ganhar uma versão.
- ``git commit -m “mensagem do commit” `` é o comando que rodamos para o projeto ganhar uma nova versão.
- ``git log `` é o comando que imprime todo o histórico de commits dados no projeto.

### Repositório remoto

- Primeiro iniciamos o repositório com ``git init, git add . , git commit`` 
- Criamos um repositorio no github 
- ``git remote add origin url-que-voces-copiaram-do-github`` conectamos aquele repositório local com um remoto
-``git push origin master`` é o comando que damos pra subir as alterações que fizemos no projeto para o github.

``git status`` Esse comando nos ajuda a ver os estágios dos arquivos. Antes do add e do commit podemos usá-lo para ver quais arquivos foram criados e ou modificados.

##### Files stages (Estágios do arquivo)

**untracked files** não deu instrução ao git do que fazer com o arquivo
**changes to be committed** adicionou, mas não deu o commit
**commited** commit foi feito


### Clone

Para trazer uma cópia de um repositório remoto para o seu computador usamos:

`` git clone ulr-do-repo-no-github ``

Usamos o comando ``git pull`` para atualizar nossa repositório local com o remoto.


### Branch

Branch são ramificações dentro do seu projeto, ou seja, uma branch é uma linha independente de desenvolvimento em que podemos comitar novas versões do código sem afetar o projeto.
![GitHub Logo](https://raw.githubusercontent.com/reprograma/on7-porto-s1-introducao/master/images/branch.png)

- ``git checkout -b nome-da-branch `` para criar uma branch
- `` git branch`` para visualizar as branchs existentes
- ``git checkout nome-da-branch`` para trocar de branch
- `` git merge nome-da-branch`` é o comando que uso para trazer as modificações de uma branch para outra. 

### Pull Request - PR

É através de pull request que podemos contribuir com outros projetos, e fica em responsabilidade do dono do repositório autorizar o merge da suas alterações, podendo ele negar, pedir correções entre outras coisas.
- Fork o repositório no github 
- Clonar repositório (git clone url-do-projeto)
- Criar sua branch para trabalhar git checkout -b nome-da-sua-branch
- Faça mudanças e: 
  - git add .
  - git commit -m "o que eu fiz"
  -  git push origin nome-da-sua-branch
- Agora vamos no github abrir a PR  :octocat: 


### Readme.md MARKDOWN
Arquivo essencial para todo repositório no github. onde explicamos o projeto e damos algumas instruções, caso necessário.

https://dillinger.io/

https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf

### links úteis:
https://medium.com/reprogramabr/git-e-github-por-onde-come%C3%A7ar-ca88a783c223 -> Medium Reprograma. Escrito por Thaylla <3

https://git-scm.com/book/pt-br/v1/Primeiros-passos-Sobre-Controle-de-Vers%C3%A3o -> Documentação oficial do git em português.

https://rogerdudler.github.io/git-guide/index.pt_BR.html -> git - guia prático












