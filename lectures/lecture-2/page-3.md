---
layout: default
transition: slide-up
title: Operadores Null Safety
---

# Operadores Null Safety

- __Nullable type (?)__: utilizado para indicar que uma variável pode receber `null`. O operador deve ser inserido logo após o tipo da variável, por exemplo: `String?`;

- __Null assertion operator (!)__: em alguns momentos o sistema de tipagem pode inferir que uma operaçõa não poderã ser realizada porque umas das variáveis pode receber null. Porém, se você tem certeza que aquela variável nunca receberá `null` pode-se usar o operador ! para reforçar pro sistema de tipagem que um valor não é `null` antes de realizar outra operação.

<div>

  ```dart
  void main() {
    int? a;
    a = null;
    print('a is $a.');
  }
  ```

</div>


<div v-click>

  ```dart
  void main() {
    int a;
    a = 42;
    print('a is $a.');
  }
  ```
  
</div>

[Exercícios de operadores Null Safety](https://dart.dev/codelabs/null-safety)

