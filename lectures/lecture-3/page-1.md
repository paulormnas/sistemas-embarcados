---
layout: default
transition: slide-up
---

# [Polimorfismo](https://www.alura.com.br/artigos/poo-programacao-orientada-a-objetos)

<div class="mx-4">

O polimorfismo é uma maneira de implementarmos um memso método em classes diferentes. Neste caso, os métodos teram funcionalidades diferentes, que depende do objeto que a classe representa. Vamos ver um exemplo:

```dart
abstract class Sensor{
  var value = 0;

  void read(){
    value += 1;
    print(value);
  }
}
```

</div>

