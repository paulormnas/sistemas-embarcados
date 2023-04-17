---
layout: default
transition: slide-up
---

# [GitFlow](https://datasift.github.io/gitflow/IntroducingGitFlow.html)

<div>

O GitFlow é uma recomendação de organização de branchs e commits quando se está trabalhando em equipe. Isso ajuda a manter um estado funcional do código, recuperar versões anteriores e ajuda a manter o controle de qual versão será lançada para o usuário final. 

</div>

<div class="ml-30">

```mermaid
gitGraph
      commit id:"1" tag:"v1.0.0"
      branch hotfix order: 1
      branch develop order: 2
      checkout develop
      commit id:"2"
      branch feature1 order: 3
      checkout feature1
      commit id:"3"
      commit id:"4"
      checkout hotfix
      commit id:"5"
      checkout main
      merge hotfix tag:"v1.0.1"
      checkout feature1
      commit id:"6"
      checkout develop
      merge feature1
      commit id:"7"
      checkout main
      merge develop tag:"v1.2.0"

```

</div>
