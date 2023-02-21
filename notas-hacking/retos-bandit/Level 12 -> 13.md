# Level 12

## Objetivo
The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Datos de Acceso
bandit12
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

## Solución
```bash
bandit12@bandit:~$ ls
data.txt
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO| bzcat | tar xO | zcat | file -
/dev/stdin: ASCII text
bandit12@bandit:~$ cat data.txt | xxd -r | zcat | bzcat | zcat | tar xO | tar xO| bzcat | tar xO | zcat 
The password is wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|zcat, bzcat, tar x0|Comandos para descomprimir un archivo en sus respectivos formatos|
|xxd -r|Realiza un vaciado exadecimal, sirve para examinar byte por byte un archivo|

## Referencias
- [Hex dump](https://en.wikipedia.org/wiki/Hex_dump)