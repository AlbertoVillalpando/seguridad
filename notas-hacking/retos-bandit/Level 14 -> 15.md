# Level 14

## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30000 on localhost**.

## Datos de Acceso
bandit14
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

## Solución
```bash
bandit14@bandit:~$ nc -v localhost 30000
Connection to localhost (127.0.0.1) 30000 port [tcp/*] succeeded!
fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq
Correct!
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|nc|Sirve para conectarse a puertos de otros sistemas|

## Referencias
- []()
