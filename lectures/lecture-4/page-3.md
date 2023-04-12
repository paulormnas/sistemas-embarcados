---
layout: two-cols
transition: slide-up
title: Operadores Null Safety
---

# [Mock](https://pub.dev/packages/mockito)

<div class="mx-4">

O mock é uma técnica usada para simular a chamada de uma função ou método de objeto sem de fato executar seu respectivo código. Com isso podemos simular a chamada de bancos de dados e APIs sem de fato consumir o serviço, tornando os testes mais ágeis. Para criar mocks nos testes em Dart devemos usar o pacote `mockito` ou usar as classes de teste disponíveis no pacotes adicionados ao projeto, como no caso do `http/testing`.

```dart {all} {maxHeight:'160px'}
Future<bool> getPokemonListFromAPI() async {
    bool apiCallStatus = false;
    try {
      var url = Uri.parse(
          "https://pokeapi.co/api/v2/pokemon/?offset=0&limit=1281");
      var response = await _client.get(url);
      _listaDePokemons = json.decode(response.body) as Map<String, dynamic>;
      apiCallStatus = response.statusCode == 200 ? true : false;
    } catch (e){
      print(e);
    }
    return apiCallStatus;
  }
```
</div>

::right::

<div class="pt-10">

Aqui temos um teste que realiza o mock do `Client` da biblioteca http. [Link pro Replit](https://replit.com/@paulormnas/pokemonAPI#projeto/test/pokemonAPI_test.dart)

```dart
 test("busca de catalogo de pokemons com mock", () async {
    final mockClient = MockClient(
            (request) async {
      return Response(jsonEncode(responseMap), 200);
    }
    );

    Catalog pokemonCatalog = Catalog(mockClient);
    await pokemonCatalog.getPokemonListFromAPI();
    const expectedPokeNames = [
      "bulbasaur",
      "ivysaur",
      "venusaur",
      "charmander",
      "charmeleon"
    ];

    expect(pokemonCatalog.listaDeNomes, expectedPokeNames);
  });
```

</div>