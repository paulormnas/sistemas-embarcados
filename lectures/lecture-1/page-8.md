---
layout: default
transition: slide-up
---

# Entrada de dados

<div>

Para ler dados do terminal digitado pelo usuário precisamos importar a biblioteca **dart:io** e usar a a função `stdin.readLineSync()`

</div>

```dart
import 'dart:io';

void main() {
  print("Qual a sua idade?");
  String? input = stdin.readLineSync();
  if (input != null) {
    int idade = int.parse(input);
    print("Ano que vem sua idade será ${idade + 1} anos.");
  } else {
    print("Não foi possível calcular o valor da idade");
  }
}

```
