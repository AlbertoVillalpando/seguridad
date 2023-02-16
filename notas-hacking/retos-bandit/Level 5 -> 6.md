# Level 5

## Objetivo
The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:
-   human-readable
-   1033 bytes in size
-   not executable

## Datos de Acceso
bandit5
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

## Solución
```bash
bandit5@bandit:~$ find -readable -size 1033c -type f
./inhere/maybehere07/.file2
bandit5@bandit:~$ cat ./inhere/maybehere07/.file2
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|find|Busca un archivo en específico|
|-readable|Busca archivos legibles (ASCII) para un humano|
|-size|Especifica el tamaño|
|-type|Especifica el tipo|

## Referencias
- []()