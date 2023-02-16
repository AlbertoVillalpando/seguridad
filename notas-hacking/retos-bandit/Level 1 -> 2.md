# Level 1

## Objetivo
The password for the next level is stored in a file called **-** located in the home directory

## Datos de Acceso
bandit1
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

## Solución
```bash
bandit0@bandit:/home/bandit1$ ls
-
bandit0@bandit:/home/bandit1$ cat -
^C
bandit0@bandit:/home/bandit1$ cat /home/bandit1/-
cat: /home/bandit1/-: Permission denied
bandit0@bandit:/home/bandit1$ 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- [Archivos con guión](https://stackoverflow.com/questions/42187323/how-to-open-a-dashed-filename-using-terminal)