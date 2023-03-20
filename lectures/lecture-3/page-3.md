---
layout: default
transition: slide-up
title: Operadores Null Safety
---

# [Polimorfismo](https://www.alura.com.br/artigos/poo-programacao-orientada-a-objetos)

<div>

Como é implementado o polimorfismo em Dart?

</div>

```dart
void main(){
  DHT22 dht = DHT22();
  PIR pir = PIR();
  var sensors = [dht, pir];

  for (final sensor in sensors){
    print( sensor.read() );
  } 
}
```