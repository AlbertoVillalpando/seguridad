# Level 4

## Objetivo
The password for the next level is stored in the only human-readable file in the **inhere** directory. Tip: if your terminal is messed up, try the “reset” command.

## Datos de Acceso
bandit4
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

## Solución
```bash
bandit4@bandit:~$ cd inhere/
bandit4@bandit:~/inhere$ ls -la
total 48
drwxr-xr-x 2 root    root    4096 Jan 11 19:19 .
drwxr-xr-x 3 root    root    4096 Jan 11 19:19 ..
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file00
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file01
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file02
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file03
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file04
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file05
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file06
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file07
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file08
-rw-r----- 1 bandit5 bandit4   33 Jan 11 19:19 -file09
bandit4@bandit:~/inhere$ file ./*
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
bandit4@bandit:~/inhere$ cat ./-file07
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

```

## Notas Adicionales
|comando|descripcion|
|---|---|
|file|Indica el tipo de archivo|

## Referencias
- []()