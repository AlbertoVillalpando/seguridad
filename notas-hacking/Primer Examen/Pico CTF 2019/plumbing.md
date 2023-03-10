## Descripción

Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 7480`.

alberto@Nova:~$ 

## Solución

```bash
alberto@Nova:~$ netcat jupiter.challenges.picoctf.org 7480 | grep picoCTF
picoCTF{digital_plumb3r_06e9d954}
^C
alberto@Nova:~$ 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
