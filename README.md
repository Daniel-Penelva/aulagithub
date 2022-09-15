![GitHub repo size](https://img.shields.io/github/repo-size/Daniel-Penelva/aulagithub)
![GitHub language count](https://img.shields.io/github/languages/count/Daniel-Penelva/aulagithub)
![GitHub top language](https://img.shields.io/github/languages/top/Daniel-Penelva/aulagithub)

# Aprendendo Git e Github 
#### LEGAL! Contudo, ainda aprendi sozinho README :+1:
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/Daniel-Penelva/exemplo-readme/blob/main/LICENCE)

## Curso autodidata quero aprender git e github 
<img src="https://github.com/Daniel-Penelva/aulagithub/blob/main/image/github-cat.gif" width="100px" height="100px" align="middle"> 

### Git
Git é um sistema de versionamento para gerenciar as suas versões. Ela permite manter os históricos, voltar as versões, permitir ver a(s) diferença(s) de uma versão da outra e vários outros recursos avançados.

O Git armazena o conteúdo do projeto representando as mudanças através de um **grafo de commits**.

![imagem_github](https://github.com/Daniel-Penelva/aulagithub/blob/main/image/estrutura-git.jpg)

O Git gerencia as mudanças de projetos, para isso existe uma espécie de containers onde são adicionados todos os tipos de arquivos e pastas que foram criados ou modificados. Usa-se o **_<$ git add>_** para adicionar os arquivos e pastas, o **_<$ git status>_** verifica o que está armazenado no container e o **_<$ git commit>_** identifica e armazena esse container no repositório local. 

### Github 
Gituhub é um serviço online de hospedagem de projeto gerenciado pelo git.

## Comandos primários no git

> ls - Lista arquivo(s) ou diretório(s) atual.

> ls -a - Exibir ou listar diretório(s) ocultos.

> cd - Acessa diretório.

> mkdir - criar diretório.

> touch - Criar arquivo.

> rmdir - Remover diretório.

> rm - Remover arquivo.

> pwd - Imprime o nome do diretório local em uma interface de linha de comando.

> nano - Mostrar o conteúdo do arquivo.

> cat - Mostrar no terminal git o conteúdo do arquivo.

> mv - Mover diretório ou arquivo.

> clear - limpar o terminal git.

## PASSO-A-PASSO: Salvar primeira versão de um projeto no Github

Sempre que criar um novo projeto os passos serão:
```
$ git init

$ git add .

$ git commit -m "descrição explicativa"

OBS. Vale ressaltar que o passo abaixo é gerado para você quando cria um repositório no github.

$ git remote add origin git@github.com: seuusuario/seurepositorio.git

$ git push
```
### Vamos as explicações :+1:
1. **_<$ git init>_** Para criar o repositório git, ou seja, vai criar a pasta .git no seu repositório local.

2. **_<$ git add .>_** Esse comando vai enviar os arquivos do seu projeto para uma área temporária chamada stage.

> **OBS.** O ponto “.” depois do add é para capturar a pasta com todos os arquivos que você está manipulando o projeto.

> **OBS.** Para enviar apenas um arquivo basta utilizar o comando **_<$ git add nome_arquivo.txt>_**

3. **_<$ git commit -m "descrição explicativa">_** Esse comando vai salvar efetivamente essa nova versão no repositório git.

> **OBS.** O comando **_<$ git status>_** vai mostar o status da branch.

> **OBS.** O comando **_<$ git log --oneline>_** vai mostrar o(s) número(s) de commit(s).

4. **_<$ git commit -m "descrição explicativa">_** Esse comando vai associar o seu projeto do seu computador com o projeto que está no GitHub. Essa associação garante que você possa enviar dados de um projeto para o outro.

> **OBS.** A palavra “origin” é muito importante, pois é ela que garante o apelido do repositório do GitHub para que seja possível fazer essa conexão do projeto do repositório local (git) com o repositório remoto (GitHub). “Origin” é uma palavra padrão do GitHub. 

5. **_<$ git push>_** Esse comando vai enviar (comitar) para o GitHub os dados.

> **OBS.** Ou <$ git push -u origin main>

## PASSO-A-PASSO: Salvar uma nova versão de commit no git e github
```
$ git add .

$ git commit -m "descrição explicativa"

$ git push
```

## Criando branch
Branch é uma ramificação, ou seja, o comando git branch permite criar, listar, renomear e excluir ramificações. As ramificações do Git são um indicador efetivo de um instantâneo de suas mudanças. 

As ramificações são apenas indicadores, ou seja, quando você cria uma ramificação, tudo o que o Git precisa fazer é criar um novo indicador, ele não muda o repositório de nenhuma outra maneira, isto é, quando se cria uma branch, automaticamente, vai sair da main. 

Vale ressaltar que o HEAD sempre será o último commit.

<img src="https://github.com/Daniel-Penelva/aulagithub/blob/main/image/main-git.jpg" width="150px" height="150px">

Ele não permite alternar entre as ramificações ou reunir um histórico bifurcado de novo. Por esse motivo, o comando **_<$ git branch>_** é muito integrado com os comandos **_<$ git checkout>_** e **_<$ git merge>_**

**OBS.** Através do comando **_<$ git log --graph --all>_** ou **_<$ git log --oneline --graph --all>_** é possível ver um gráfico dos commits executados.

### PASSO A PASSO: criando branch

```
$ git checkout -b nome_branch_criada
OBS. Criar uma branch
OBS. O checkout vai fazer sair da branch “main” e vai para a branch criada.

$ git branch
OBS. Confere todas as suas branchs.

$ git add .

$ git commit -m "descrição explicativa"

$ git push origin nome_branch_criada

$ git checkout main
OBS. Altera do branch criado para o branch main. 
OBS. Vale ressaltar que para fazer o merge é preciso estar no branch main.

$ git merge nome_branch_criada
OBS. Faz a junção das branchs

$ git push
```

**Observações Adicionais:**
```
Para deletar um branch utiliza-se o comando:
$ git branch –d nome_do_branch

Para alterar o nome de uma branch utiliza-se o comando:
$ git branch –m nome_do_novo_branch
```
**Exemplificando**

Eu criei um branch teste e nele foi criado um arquivo chamado *teste.html* (através do comando touch). Farei três commits e depois vou carregar no github. 

<img src="https://github.com/Daniel-Penelva/aulagithub/blob/main/image/exemplo-branch.jpg" width="950px" height="950px">

:computer: Autor: Daniel Penelva de Andrade

