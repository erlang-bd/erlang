## Erlang Linux install

Erlang is a programming language used to build massively scalable soft real-time systems with requirements on high availability. Erlang runtime system has built-in support for concurrency, distribution and fault tolerance. This tutorial will help you to install erlang on Ubuntu 18.04 and 16.04 operating system.

Step 1 – Adding Repository
First, use the following commands to add erlang apt repository on your system. You can simply download erlang repository package from its official website and install on your system.

```sh
wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb
sudo dpkg -i erlang-solutions_1.0_all.deb
```

Step 2 – Install Erlang on Ubuntu
Now, you can install erlang package on your system using the following command. This will install all of its dependencies as well.

```sh
sudo apt-get update
sudo apt-get install erlang
```

Alternatively, you can do the complete erlang installation. It includes the Erlang/OTP platform and all of its applications.

```sh
sudo apt-get update
sudo apt-get install esl-erlang
```

Step 3 – Erlang Hello World Program
Let’s start with hello world program on erlang. First create file helloworld.erl with following content.

```sh
vi helloworld.erl
```

add the following contnet.

```sh
% hello world program
-module(helloworld).
-export([start/0]).

start() ->
io:fwrite("Hello World!\n").
```

Now compile the hello world program using below command.

```sh
erlc helloworld.erl
```

The above command will create a file helloworld.beam in the current directory. You can run your program now.

```sh
erl -noshell -s helloworld start -s init stop
```

Hello World!
