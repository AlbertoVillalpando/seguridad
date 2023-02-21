# Level 11

## Objetivo
The password for the next level is stored in the file **data.txt**, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Datos de Acceso
bandit11
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

## Solución
```bash
bandit11@bandit:~$ ls
data.txt
bandit11@bandit:~$ cat data.txt | tr [a-zA-Z] [n-za-mN-ZA-M]
The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|tr|Indicamos a una cadena de texto que rote su texto una cantidad de caracteres indicada. Ej, tr [a-zA-Z] [n-za-mN-ZA-M], de a a z y A a Z rota los caracteres n hasta z y a hasta n. 


## Referencias
- [ROT13](https://es.wikipedia.org/wiki/ROT13)