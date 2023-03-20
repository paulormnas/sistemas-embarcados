---
layout: two-cols
transition: slide-up
---

# [Polimorfismo](https://www.alura.com.br/artigos/poo-programacao-orientada-a-objetos)

<div class="mx-4">

```dart
class DHT22 extends Sensor{
  int DHTSensor = 22
  int DHTPin = 9
  
  @override
  void read() {
    var humidityAndTemperature = []
    humidityAndTemperature = AdafruitDHT.readRetry(this.DHTSensor, this.DHTPin)
    if (humidity != None and temperature != None){
        return humidityAndTemperature
    } else {
        print("Falha ao receber os dados do sensor DHT22.")
    }
  }
}
```

</div>

::right::

<div class="pt-12 mx-4">

```dart
class PIR extends Sensor{
  int PIRPin = 9
  int LAST_READ_TIME = 0
  int INTERVAL = 5000 // intervalo entre medições em milisegundos

  @override
  void read() {
    dataToSend = []
    if (
        DateTime.now().millisecondsSinceEpoch - this.LAST_READ_TIME > this.INTERVAL
        and GPIO.input(this.PIN)
    ){
        dataToSend.add(this.formatData("MOVIMENTO", 1))
        self.LAST_READ_TIME = DateTime.now().millisecondsSinceEpoch
    }
    return dataToSend.length > 0 ? dataToSend : Null
  }
}
```

</div>