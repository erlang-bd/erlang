### Erlang Code Compile and Run

#### Erlang
* ` main.erl `

```erlang
%%%-------------------------------------------------------------------
%%% @author smwin
%%% @copyright (C) 2018, ssd-tech
%%% @doc
%%%
%%% @end
%%% Created : 24. Jan 2018 4:06 PM
%%%-------------------------------------------------------------------
-module(main).
-author("smwin").

-export([start/0]).

start() ->
  io:fwrite("Hello Erlang\n").
```

#### Compile and Run
```sh
erlc main.erl ; erl -noshell -s main start -s init stop
```
