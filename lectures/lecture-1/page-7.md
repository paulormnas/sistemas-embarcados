---
layout: two-cols
transition: slide-up
---

# Estruturas de repetição

<div class="mx-4">

[Loop For](https://dart.dev/guides/language/language-tour#for-loops)

```dart {1-6|7-10|all}

var list = [];
for (var i = 0; i < 3; i++) {
  list.add(i++);
  print(`$list[i]`);
}

for (final v in list) { // list = [1, 2, 3]
  var temp = v++;
  print(`$temp`));
}

```

</div>

<div v-click class="mx-4">

<br>

<h4>

forEach()

</h4>

```dart

var collection = [1, 2, 3];
collection.forEach(print); // 1 2 3

```

</div>

::right::

<div v-click class="pt-5 mx-4">

<br>

<h4>

While

</h4>

```dart

while (!isDone()) {
  doSomething();
}


```

<br>

<h4>

Do - While

</h4>

```dart

do {
  printLine();
} while (!atEndOfPage());

```

</div>
