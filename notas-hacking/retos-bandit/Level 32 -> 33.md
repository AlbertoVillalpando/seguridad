# Level 32

## Objetivo
After all this `git` stuff its time for another escape. Good luck!

## Datos de Acceso
bandit32
rmCBvG56y58BXzv98yZGdO7ATVL5dW8y

## Solución
Ya que todo input lo convierte a mayúsculas a partir de cierta posición en la línea de comandos, debemos posicionarnos en un índice dónde esto no ocurra con $0, entonces deberemos exportar el valor de entorno SHELL para poder acceder al shell propio del reto y poder leer la llave. 

```bash
alberto@Nova:~/bandit$ ssh bandit32@bandit.labs.overthewire.org -p 2220
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

bandit32@bandit.labs.overthewire.org's password: 
WELCOME TO THE UPPERCASE SHELL
>> 
>> $0
$ export SHELL=/bin/bash    
$ echo $SHELL
/bin/bash
$ $SHELL
bandit33@bandit:~$ cat /etc/bandit_pass/bandit33
odHo63fHiFqcWWJG9rLiLDtPm45KzUKy
bandit33@bandit:~$ 

```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()