---
layout: default
transition: slide-up
---

# Exemplo

<div class="mx-4">

```dart
// Without null safety:
bool isEmpty(String texto) => texto.length == 0;

main() {
  isEmpty(null);
}
```

</div>

<div v-click class="pt-5 mx-4">

```dart
// Using null safety:
makeCoffee(String coffee, [String? dairy]) {
  if (dairy != null) {
    print('$coffee with $dairy');
  } else {
    print('Black $coffee');
  }
}
```

</div>
