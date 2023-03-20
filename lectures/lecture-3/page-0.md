---
layout: two-cols
transition: slide-up

---

# [Herança](https://www.alura.com.br/artigos/poo-programacao-orientada-a-objetos)

<div class="mx-4">

Herança é uma maneira de aproveitar o código descrito em outras classe e expandir suas funcionalidades. Por exemplo, pense que temos uma classe que representa o objeto Televisão. Esta classe já possui um método `turnOn()` com a funcionalidade de ligar a Televisão.

```dart
class Television {
  void turnOn() {
    _illuminateDisplay();
    _activateIrSensor();
  }
  // ···
}
```

</div>

::right::

<div v-click class="pt-9 mx-4">

Imagine agora que desejamos expandir estas funcionalidades para uma Smart TV, que possui as mesmas funcionalidades da TV normal, porém implementa mais alguns métodos para tratar a conectividade e atualizar os aplicativos instalados.

```dart
class SmartTelevision extends Television {
  void turnOn() {
    super.turnOn();
    _bootNetworkInterface();
    _initializeMemory();
    _upgradeApps();
  }
  // ···
}
```

</div>
