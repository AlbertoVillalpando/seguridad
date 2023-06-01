## Descripción
How about some hide and seek heh? Look at this image [here](https://artifacts.picoctf.net/c/235/atbash.jpg).

## Solución
Al jpg le extraemos la información que pueda contener con el comando steghide.

Al texto proporcionado le aplicamos el algoritmo Atbash Cipher:

picoCTF{atbash_crack_92533667}

```bash
alberto@Nova:~/Descargas$ steghide extract -sf atbash.jpg 
Anotar salvoconducto: 
anot� los datos extra�dos e/"encrypted.txt".
alberto@Nova:~/Descargas$ cat encrypted.txt 
krxlXGU{zgyzhs_xizxp_92533667}
alberto@Nova:~/Descargas$ 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()