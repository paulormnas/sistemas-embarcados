---
layout: default
transition: slide-up
---

# Princípios do Null Safety

- __Non-nullable by default__: A não ser que você diga ao Dart que uma variável pode receber null, ele considera sempre que todas as variáveis são  `non-nullable`;

- __Incrementally adoptable__: Você escolhe o que migrar para _null safety_ e quando. Você pode migrar incrementalmente, misturando código _null safety_ com código _non null safety_ no mesmo projeto;

- __Fully Sound__: O _null safety_ é bastante robusto e auxilia durante o desenvolvimento de código. Se o sistema de tipagem identificar que uma variável não pode ser ser _null_, ela nunca será. Isto contribui não apenas para menos bugs, mas também para binários menores e execução mais rápida.