# erlang_learn

Tutorial :
- https://www.youtube.com/watch?v=eB0Y2mYLHO4&list=PLJr0bQpUAsMjwKxwHQXEunWQaZ9q5ttuH
- https://www.tutorialspoint.com/erlang/erlang_data_types.htm

contoh :

Buat file <b>helloworld.erl</b> (nama file harus sesuai nama modul)
```
% hello world program
-module(helloworld).    -> seperti namespace 
-export([start/0]). 

start() -> 
   io:fwrite("Hello, world!\n").
```

ketik perintah
```
D:\> erl
...
cd("D:/").         --> lokasi dimana file helloworld.erl
c(helloworld).	   --> compile file helloworld.erl	
```

