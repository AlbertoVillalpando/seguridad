# Level 20

## Objetivo
There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

**NOTE:** Try connecting to your own network daemon to see if it works as you think

## Datos de Acceso
bandit20
VxCazJaVykI6W36BkBU0mJTCM8rR95XT

## Solución
```bash
bandit20@bandit:~$ ls -la
total 36
drwxr-xr-x  2 root     root      4096 Feb 21 22:03 .
drwxr-xr-x 70 root     root      4096 Feb 21 22:04 ..
-rw-r--r--  1 root     root       220 Jan  6  2022 .bash_logout
-rw-r--r--  1 root     root      3771 Jan  6  2022 .bashrc
-rw-r--r--  1 root     root       807 Jan  6  2022 .profile
-rwsr-x---  1 bandit21 bandit20 15600 Feb 21 22:03 suconnect

bandit20@bandit:~$ nc -nlvp 8383 <<< VxCazJaVykI6W36BkBU0mJTCM8rR95XT &
[1] 3122002
bandit20@bandit:~$ Listening on 0.0.0.0 8383

bandit20@bandit:~$ ./suconnect 8383
Connection received on 127.0.0.1 46566
Read: VxCazJaVykI6W36BkBU0mJTCM8rR95XT
Password matches, sending next password
NvEJF7oVjkddltPSrdKEFOllh9V1IBcq

```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
