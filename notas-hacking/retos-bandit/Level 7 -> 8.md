# Level 7

## Objetivo
The password for the next level is stored in the file **data.txt** next to the word **millionth**

## Datos de Acceso
bandit7
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

## Solución
```bash
bandit7@bandit:~$ ls -la
total 4108
drwxr-xr-x  2 root    root       4096 Jan 11 19:19 .
drwxr-xr-x 70 root    root       4096 Jan 11 19:19 ..
-rw-r--r--  1 root    root        220 Jan  6  2022 .bash_logout
-rw-r--r--  1 root    root       3771 Jan  6  2022 .bashrc
-rw-r-----  1 bandit8 bandit7 4184396 Jan 11 19:19 data.txt
-rw-r--r--  1 root    root        807 Jan  6  2022 .profile
bandit7@bandit:~$ wc data.txt 
  98567  197133 4184396 data.txt
bandit7@bandit:~$ grep millionth data.txt 
millionth	TESKZC0XvTetK0S9xNwm25STk5iWrBvP
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|grep|Filtra las lineas de texto en un archivo|

## Referencias
- []()