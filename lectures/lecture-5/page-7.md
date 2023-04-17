---
layout: default
transition: slide-up
---

# Comandos Importantes

<div>

Uma Branch (Ramificação) nada mais é que abrir um novo fluxo de trabalho para continuar o desenvolvimento sem bagunçar o código que se encontra funcional no momento.

</div>

<div>

```shell
$ git init # inicia um novo repositório local
$ git status # verifica as modificações do repositório local
$ git log # mostra histórico de alterações gravadas no banco de dados local
$ git add [nome-do-arquivo] # marca o arquivo para gravar no próximo commit
$ git commit # efetua a gravção das modificações no banco de dados local
$ git push [nome-do-remote] [nome-da-branch] # envia alterações para o repositório remoto
$ git pull [nome-do-remote]  [nome-da-branch] # baixa alterações do repositório remoto para o repositório local
$ git branch [nome-da-branch] # cria uma nova branch no repositório local
$ git checkout [nome-da-branch] # troca de branch para fazer novas alterações
$ git remote # configura informações do repositório remoto
$ git fetch # busca informações no repositório remoto mas não sobreescreve o banco de dados local
$ git stash # salva modificações em uma memória temporária e não registra no banco de dados
$ git merge [nome-da-branch] # Faz o merge da branch atual com a branch indicada no comando
```

</div>
