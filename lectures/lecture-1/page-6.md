---
layout: two-cols
transition: slide-up
---

# Estruturas de decisão

<div class="mx-4">

[If e Else](https://dart.dev/guides/language/language-tour#if-and-else)



```dart

if (isRaining()) {
  you.bringRainCoat();
} else if (isSnowing()) {
  you.wearJacket();
} else {
  car.putTopDown();
}

```
</div>

::right::

<div v-click class="pt-5 mx-4">

<br>

[Switch e Case](https://dart.dev/guides/language/language-tour#switch-and-case)


```dart

var command = 'OPEN';
switch (command) {
  case 'CLOSED':
    executeClosed();
    break;
  case 'PENDING':
    executePending();
    break;
  case 'APPROVED':
    executeApproved();
    break;
  case 'DENIED':
    executeDenied();
    break;
  case 'OPEN':
    executeOpen();
    break;
  default:
    executeUnknown();
}

```

</div>
