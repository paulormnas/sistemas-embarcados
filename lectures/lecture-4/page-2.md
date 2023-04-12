---
layout: default
transition: slide-up
---

# [Cobertura de código](https://pub.dev/packages/test#collecting-code-coverage)

<div class="mx-4">

A cobertura de código é uma maneira de identificar o quanto seus teste estão efetivamente executando trechos do código fonte da sua aplicação. Quanto maior a cobertura, mais o software está sendo testado. Porém, alcançar 100% de cobertura de código pode não ser viável. 

A seguir estão alguns comandos para verificar a cobertura de código em um projeto com Dart/Flutter

```shell
## Executa os testes Dart e coloca os resultados no diretório `./coverage`:
dart run test --coverage=./coverage

## Ativa o pacote `coverage` (se necessário):
dart pub global activate coverage

## Formata os resultados de cobertura para LCOV (apenas arquivos no diretório "lib")
dart pub global run coverage:format_coverage --packages=.dart_tool/package_config.json --report-on=lib --lcov -o ./coverage/lcov.info -i ./coverage

## Gera o relatório LCOV:
genhtml -o ./coverage/report ./coverage/lcov.info

## Abre o HTML  com o relatório de cobertura:
open ./coverage/report/index.html
```

</div>