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
Branch é uma ramificação, ou seja, o comando git branch permite criar, listar, renomear e excluir ramificações. 
Vale ressaltar que o HEAD sempre será o último commit.
