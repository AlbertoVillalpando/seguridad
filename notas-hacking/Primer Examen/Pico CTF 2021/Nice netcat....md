## Descripción

There is a nice program that you can talk to by using this command in a shell: `$ nc mercury.picoctf.net 21135`, but it doesn't speak English...

## Solución

Traducir del código ASCII a texto UTF-8.

picoCTF{g00d_k1tty!_n1c3_k1tty!_afd5fda4}

```bash
alberto@Nova:~$ netcat mercury.picoctf.net 21135 
112 
105 
99 
111 
67 
84 
70 
123 
103 
48 
48 
100 
95 
107 
49 
116 
116 
121 
33 
95 
110 
49 
99 
51 
95 
107 
49 
116 
116 
121 
33 
95 
97 
102 
100 
53 
102 
100 
97 
52 
125 
10 
^C
alberto@Nova:~$ 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()