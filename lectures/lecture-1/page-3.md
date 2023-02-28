---
layout: default
transition: slide-up
title: Outras brincadeiras com funções
---

# Outras brincadeiras com funções

<div>

  First Class Object

  ```dart {1|3-4|all}
  String upperMessage(String msg) => '!!! ${msg.toUpperCase()} !!!'

  var loudify = upperMessage;
  assert(loudify('hello') == '!!! HELLO !!!'); // true
  ```
</div>


<div v-click>

  Função Anônima 

  ```dart {monaco}

  const list = ['apples', 'bananas', 'oranges'];
  const mappedList = list.map((item) {
    return item.toUpperCase();
  }) // ['APPLES', 'BANANAS', 'ORANGES']
  
  mappedList.forEach((item) {
    print('$item: ${item.length}');
  });

  ```
</div>

