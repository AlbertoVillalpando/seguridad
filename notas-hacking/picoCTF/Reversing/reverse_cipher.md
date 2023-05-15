## Descripción
We have recovered a [binary](https://jupiter.challenges.picoctf.org/static/31c9b832d036a10daeef52d8b4290ef0/rev) and a [text file](https://jupiter.challenges.picoctf.org/static/31c9b832d036a10daeef52d8b4290ef0/rev_this). Can you reverse the flag.

## Solución
Descargar ghidra, agregar el archivo descargado, checar el método que genera la llave, realizar una ejecución inversa al método del archivo.

```bash
rev = open('rev_this').read()

for j in range(8,len(rev)-1):
    if j & 1 == 0:
        print(chr(ord(rev[j])-5), end = '')
    else:
        print(chr(ord(rev[j])+2), end = '')

picoCTF{r3v3rs37ee84d27}
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
