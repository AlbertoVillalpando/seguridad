## Descripción

Can you crack the password to get the flag? Download the password checker [here](https://artifacts.picoctf.net/c/17/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/17/level2.flag.txt.enc) in the same directory too.

## Solución

```bash
alberto@Nova:~/Descargas$ nano level2.py 

alberto@Nova:~/Descargas$ touch decoder.py
alberto@Nova:~/Descargas$ nano decoder.py 
alberto@Nova:~/Descargas$ cat decoder.py 
print(chr(0x34) + chr(0x65) + chr(0x63) + chr(0x39))
alberto@Nova:~/Descargas$ python3 decoder.py 
4ec9

alberto@Nova:~/Descargas$ python3 level2.py 
Please enter correct password for flag: 4ec9
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_9701e681}
alberto@Nova:~/Descargas$ 

```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
