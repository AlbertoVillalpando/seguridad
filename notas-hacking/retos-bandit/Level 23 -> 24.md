# Level 23

## Objetivo
A program is running automatically at regular intervals from **cron**, the time-based job scheduler. Look in **/etc/cron.d/** for the configuration and see what command is being executed.

**NOTE:** This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

**NOTE 2:** Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…

## Datos de Acceso
bandot23
QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G

## Solución
```bash
bandit23@bandit:~$ 
bandit23@bandit:~$ mkdir /tmp/avc99
bandit23@bandit:~$ cd /tmp/avc99
bandit23@bandit:/tmp/avc99$ nano avcscript.sh
Unable to create directory /home/bandit23/.local/share/nano/: No such file or directory
It is required for saving/loading search history or cursor positions.

bandit23@bandit:/tmp/avc99$ cat avcscript.sh 
cat /etc/bandit_pass/bandit24 > /tmp/avc99/password
bandit23@bandit:/tmp/avc99$ chmod 777 avcscript.sh 
bandit23@bandit:/tmp/avc99$ touch password
bandit23@bandit:/tmp/avc99$ chmod 666 password 
bandit23@bandit:/tmp/avc99$ ls -la
total 112
drwxrwxr-x    2 bandit23 bandit23   4096 Feb 28 18:33 .
drwxrwx-wt 3010 root     root     106496 Feb 28 18:33 ..
-rwxrwxrwx    1 bandit23 bandit23     53 Feb 28 18:31 avcscript.sh
-rw-rw-rw-    1 bandit23 bandit23      0 Feb 28 18:33 password
bandit23@bandit:/tmp/avc99$ cp avcscript.sh /var/spool/bandit24/foo
bandit23@bandit:/tmp/avc99$ ls -la
bandit23@bandit:/tmp/avc99$ cp avcscript.sh /var/spool/bandit24/foo
bandit23@bandit:/tmp/avc99$ cat password 
VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
