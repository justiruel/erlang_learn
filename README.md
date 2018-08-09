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
D:\> erl  --> jika tidak dapat di run, daftar kan "C:\Program Files\erl10.0.1\bin" ke PATH
...
cd("D:/").         --> lokasi dimana file helloworld.erl, hanya dibutuhkan jika current location di cmd saat ini tidak satu directory dengan helloworld.erl
c(helloworld).	   --> compile file helloworld.erl	
helloworld:start().   --> jalankan fungsi start
```





# CATATAN
jika mencoba import modul beda directory gagal, setting environtment variable ERL_LIBS dengan path dimana *.beam diletakkan<br/>
biasanya tanpa harus setting ERL_LIBS langsung dapat import module beda direktori seakan seperti dalam satu directory.
