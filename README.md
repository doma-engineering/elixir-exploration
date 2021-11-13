# Elixir

## Rules of Elixir in Doma

 - The code SHOULD be [deeply functional](https://github.com/witchcrafters/witchcraft).
 - Library functions SHOULD be defined using [quark's defpartial](https://github.com/witchcrafters/quark#partial).
 - Binary data MUST be tagged, perhaps using witchcraft's [`defdata binary()`](https://github.com/witchcrafters/algae#single-field-shorthand).
 - Typespecs MUST be written as tightly as possible.
 - Computations SHOULD be declared and executed independently (monad / runner pattern).
 - Functions that configure execution handling (routers, request handlers, etc) SHOULD be composable.
 - Bloatware frameworks such as Phoenix SHOULD NOT be used.
 - ORMs such as Ecto SHOULD NOT be used (I know that it's not supposed to be an ORM, but it's even worse).
 - If a database is used in the system, perpared statements SHOULD be used and encapsulated into a standalone module.
 - If a database is used, it SHOULD be used in append-only mode.

## Installation

### Ubuntu packages

```
sudo apt install libncurses5 libwxbase3.0-dev libwxgtk3.0-gtk3-dev libsctp1
```

### ESL Erlang (or asdf Erlang)

```
wget https://packages.erlang-solutions.com/erlang/debian/pool/esl-erlang_24.0.5-1~ubuntu~focal_amd64.deb -O /tmp/erl.deb
sudo dpkg -i /tmp/erl.deb
rm /tmp/erl.deb
```

If you want an easier time maintaining several versions of Erlang for some reason, please use `asdf` to install it.

### ESL Elixir (or asdf Elixir)

```
wget https://packages.erlang-solutions.com/erlang/debian/pool/elixir_1.12.2-1~ubuntu~focal_all.deb -O /tmp/ex.deb
sudo dpkg -i /tmp/ex.deb
rm /tmp/ex.deb
```

Don't forget to update your `hex` utility like so:

```
mix local.hex
```

If you want an easier time maintaining several versions of Elixir for some reason, please use `asdf` to install it.
