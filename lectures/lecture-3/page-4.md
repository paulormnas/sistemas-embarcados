---
layout: default
transition: slide-up
---

# [Encapsulamento](https://www.alura.com.br/artigos/poo-programacao-orientada-a-objetos)

<div>

O encapsulamnto é uma maneira de proteger as propriedades de objeto de forma que não aconteçam efeitos colaterais imprevisíveis durante a execução do código. Por exemplo, considere a classe PIR apresentada anteriomente, nós sabemos que o intervalo entre medições foi definido para que o banco de dados não fique cheio de informações repetidas em um curto período de tempo. Desta forma, devemos proteger o acesso às propriedades `INTERVAL` e `LAST_READ_TIME`, e torná-las [privada](https://www.darttutorial.org/dart-tutorial/dart-private-fields/):

</div>

```dart
class PIR extends Sensor{
  int PIRPin = 9
  int _LAST_READ_TIME = 0
  int _INTERVAL = 5000 // intervalo entre medições em milisegundos

  void read() {
    dataToSend = []
    if (
        DateTime.now().millisecondsSinceEpoch - this._LAST_READ_TIME > this._INTERVAL
        and GPIO.input(this.PIN)
    ){
        dataToSend.add(this.formatData("MOVIMENTO", 1))
        self._LAST_READ_TIME = DateTime.now().millisecondsSinceEpoch
    }
    return dataToSend.length > 0 ? dataToSend : Null
  }
}
```
