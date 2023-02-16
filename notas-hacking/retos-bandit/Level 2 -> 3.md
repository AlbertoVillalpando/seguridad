# Level 2

## Objetivo
The password for the next level is stored in a file called **spaces in this filename** located in the home directory

## Datos de Acceso
bandit2
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi


## Solución
```bash
bandit2@bandit:~$ cat 
.bash_logout             .profile                 
.bashrc                  spaces in this filename  
bandit2@bandit:~$ cat spaces\ in\ this\ filename 
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
```

## Notas Adicionales
- Cando hay espacios en el nombre, hay que delimitarlo.

## Referencias