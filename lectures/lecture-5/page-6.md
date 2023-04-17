---
layout: default
transition: slide-up
---

# [Git Braching](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)

<div>

Uma Branch (Ramificação) nada mais é que abrir um novo fluxo de trabalho para continuar o desenvolvimento sem bagunçar o código que se encontra funcional no momento.

</div>

<div class="ml-50">

<br><br><br>

```mermaid
---
title: Exemplo de um diagrama de Git
---
gitGraph
   commit
   commit
   branch develop
   checkout develop
   commit
   commit
   checkout main
   merge develop
   commit
   commit
```

</div>
