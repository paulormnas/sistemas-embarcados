---
layout: two-cols
transition: slide-up
---

# Listas

<div class="mx-4">
São semelhantes aos vetores/arrays da linguagem C, porém com uma sintaxe um pouco diferente e algumas funções built-in já implementadas

```dart
var list = [
  'Car',
  'Boat',
  'Plane',
];
```
</div>

<div v-click class="mx-4">

```dart
var list = [1, 2, 3];
assert(list.length == 3);
assert(list[1] == 2);

list[1] = 1;
assert(list[1] == 1);
```
</div>

<div v-click class="mx-4">
<br><br>

[Métodos da Lista](https://api.dart.dev/stable/2.19.2/dart-core/List-class.html)

</div>

::right::

<div v-click class="mx-4">
<br><br><br>

Strings também são consideradas vetores de caracteres (ou runes) em Dart. Além disso, Dart suporta o **spread operator**.

```dart
var list = [1, 2, 3];
var list2 = [0, ...list];
assert(list2.length == 4); // true
```

</div>

<div v-click class="mx-4">

Outra mágica do Dart são as **collection if** e **collection for**

```dart
var nav = ['Home', 'Furniture', 'Plants', if (promoActive) 'Outlet'];

```

</div>

<div v-click class="mx-4">

```dart
var listOfInts = [1, 2, 3];
var listOfStrings = ['#0', for (var i in listOfInts) '#$i'];
assert(listOfStrings[1] == '#1'); // true
```

</div>


