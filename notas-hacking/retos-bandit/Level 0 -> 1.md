# Level 0

## Objetivo
The password for the next level is stored in a file called **readme** located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Datos de Acceso
bandit0
bandit0
ssh bandit0@bandit.labs.overthewire.org -p 2220

## Solución
```bash
bandit0@bandit:~$ ls
readme
bandit0@bandit:~$ cat 
.bash_logout  .bashrc       .profile      readme        
bandit0@bandit:~$ cat readme 
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|cat|muestra el contenido de un archivo|

## Referencias
[# Bandit Level 0 → Level 1](https://overthewire.org/wargames/bandit/bandit1.html)
