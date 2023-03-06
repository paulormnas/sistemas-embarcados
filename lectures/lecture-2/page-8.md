---
layout: two-cols
transition: slide-up
---

# Codando uma classe 

<div class="mx-4">

### Classe

```dart
class Carro {
  Double velocidade;
  String modelo;

  Carro(String modelo) {
      this.modelo = modelo;
      this.velocidade = 0;
  }

  void acelerar() {
      /* código do carro para acelerar */
  }

  void frear() {
      /* código do carro para frear */
  }

  void acenderFarol() {
      /* código do carro para acender o farol */
  }

```

</div>

::right::

<div class="pt-14 mx-4">

### Objeto

```dart
import "Carro";

void main(){

var carro = Carro("Onix");


}
```

</div>

