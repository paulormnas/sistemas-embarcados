---
layout: default
transition: slide-up
---

# Operadores condicionais

- __Acesso condicional de propriedades (?.)__: é possível verificar se uma vriável é `null` antes de acessar suas propriedades. Por exemplo: `nome?.length`

- __Operador null-coalescing (??)__: usado para atribuir um valor diferente quando uma variável possuir o valor `null`.

```dart{0-6|10|all}
import "dart:io";

String? leNumero(){
  String? numero = stdin.readLineSync();
  return numero;
}

void main(){

  double dobro = double.parse(leNumero() ?? 0) * 2.0;
  print("O número em dobro é: $dobro");

}

```

[Exercício da conversão de moeda](https://replit.com/@paulormnas/conversor-de-moedas#main.dart)
