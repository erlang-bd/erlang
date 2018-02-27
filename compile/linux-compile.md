### Erlang Code Compile and Run

#### Erlang
* ` main.erl `

```erlang
%%%-------------------------------------------------------------------
%%% @author netcse
%%% @copyright (C) 2018, ssd-tech
%%% @doc
%%%
%%% @end
%%% Created : 24. Feb 2018 10:31 PM
%%%-------------------------------------------------------------------
-module(main).
-author("netcse").

-export([start/0]).

start() ->
  io:fwrite("Hello Erlang\n").
```

#### Compile and Run
```sh
erlc main.erl && erl -noshell -s main start -s init stop
```

#### Erlang Shell

```sh
erl
```

#### Compile and Run

```sh
c(main).
main:start().
```
