# Level 17

## Objetivo
The credentials for the next level can be retrieved by submitting the password of the current level to **a port on localhost in the range 31000 to 32000**. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

## Datos de Acceso
bandit17
VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e
llave privada

## Solución
```bash
bandit17@bandit:~$ ls -ls
total 8
4 -rw-r----- 1 bandit18 bandit17 3300 Feb 21 22:02 passwords.new
4 -rw-r----- 1 bandit18 bandit17 3300 Feb 21 22:02 passwords.old
bandit17@bandit:~$ diff passwords.old passwords.new --color
42c42
< f9wS9ZUDvZoo3PooHgYuuWdawDFvGld2
---
> hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|diff|Muestra las diferencias entre un texto y otro|

## Referencias
- []()
