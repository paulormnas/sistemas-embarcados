---
layout: two-cols
transition: slide-up
---

# Teste de Unidade

<div class="mx-4">

O teste de unidade serve para verificar o comportamento de pequenas partes de código dentro de um sistema maior. Nesse caso, as pequenas partes que podemos testar são funções, classes e bibliotecas. Vamos voltar ao exemplo das figuras geométricas:

```dart
class Quadrado extends FigurasGeometricas{
  int _lado;
  
  Quadrado(this._lado);

  @override
  int calculaArea(){
    return _lado * _lado;
  }

  @override
  int calculaComprimento(){
    return 4 * _lado;
  }
}
```

</div>

::right::

<div v-click class="pt-12">

```dart
import 'package:test/test.dart';

void main() {
  test('calcula a area', () {
    var q = Quadrado(5);
    expect(q.calculaArea(), 25);
  });

  test('calcula comprimento', () {
    var q = Quadrado(5);
    expect(q.calculaComprimento(), 20);
  });
}


```

**Importante**: para executar os testes no Android Studio é importante adicionar o pacote de testes nas dependencias do projeto, dentro do arquivo `pubspec.yaml`.

```yaml
dev_dependencies:
  test: ^1.5.1
```

</div>
