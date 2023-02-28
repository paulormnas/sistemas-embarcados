---
layout: two-cols
transition: slide-up
---

<div class="mx-4">

<h1>

[Sets ou Conjuntos](https://api.dart.dev/stable/2.19.2/dart-core/Set-class.html)

</h1>

<br>

<span>
São parecidos com as listas, porém não aceitam elementos repetidos e não são ordenados. Sets funcionam como os conjuntos da matemática e permitem operações de interseção e união.
</span>

```dart
var halogens = {'fluorine', 'chlorine', 'bromine', 'iodine', 'astatine'};
var names = <String>{};
```
</div>

<div class="mx-4">

```dart
final characters1 = <String>{'A', 'B', 'C'};
final characters2 = <String>{'A', 'E', 'F'};
final intersectionSet = characters1.intersection(characters2);
print(intersectionSet); // {A}
```
</div>

::right::

<div v-click class="mx-4">

<h1>

[Maps](https://api.dart.dev/stable/2.19.2/dart-core/Map-class.html)

</h1>

<span>

É uma estrutura de dado baseado em chave-valor que não é ordenado e costuma ser mais rápido pra procurar um valor do que as listas

</span>

```dart
var gifts = {
  // Key:    Value
  'first': 'partridge',
  'second': 'turtledoves',
  'fifth': 'golden rings'
};

var nobleGases = {
  2: 'helium',
  10: 'neon',
  18: 'argon',
};

assert(gifts['second'] == 'turtledoves'); // true

```

</div>
