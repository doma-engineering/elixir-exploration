# Elixir

## Rules of Elixir in Doma

 - The code SHOULD be [deeply functional](https://github.com/witchcrafters/witchcraft).
 - Library functions MUST be defined using [quark's defpartial](https://github.com/witchcrafters/quark#partial).
 - Binary data MUST be tagged, perhaps using witchcraft's [`defdata binary()`](https://github.com/witchcrafters/algae#single-field-shorthand).
 - Typespecs MUST be written as tightly as possible
 - Computations SHOULD be declared and executed independently (monad / runner pattern)
 - Functions that configure execution handling (routers, request
   handlers, etc) SHOULD be composable.
