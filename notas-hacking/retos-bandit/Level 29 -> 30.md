# Level 29

## Objetivo
There is a git repository at `ssh://bandit30-git@localhost/home/bandit30-git/repo` via the port `2220`. The password for the user `bandit30-git` is the same as for the user `bandit30`.

Clone the repository and find the password for the next level.

## Datos de Acceso
bandit29
tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S

## Solución
Buscamos en las ramas del repo, nos movemos a dev y leemos el README.

```bash
bandit29@bandit:/tmp/albertovc$ git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo
Cloning into 'repo'...
The authenticity of host '[localhost]:2220 ([127.0.0.1]:2220)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit29/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit29/.ssh/known_hosts).
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

bandit29-git@localhost's password: 
remote: Enumerating objects: 16, done.
remote: Counting objects: 100% (16/16), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 16 (delta 2), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (16/16), done.
Resolving deltas: 100% (2/2), done.
bandit29@bandit:/tmp/albertovc$ cd repo/
bandit29@bandit:/tmp/albertovc/repo$ ls -la
total 16
drwxrwxr-x 3 bandit29 bandit29 4096 May 31 21:20 .
drwxrwxr-x 3 bandit29 bandit29 4096 May 31 21:19 ..
drwxrwxr-x 8 bandit29 bandit29 4096 May 31 21:20 .git
-rw-rw-r-- 1 bandit29 bandit29  131 May 31 21:20 README.md
bandit29@bandit:/tmp/albertovc/repo$ cat README.md 
# Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: <no passwords in production!>

bandit29@bandit:/tmp/albertovc/repo$ git log
commit 4bd5389f9f2b9e96ba517aa751ee58d051905761 (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Sun Apr 23 18:04:40 2023 +0000

    fix username

commit 1a57cf10158f133c4f40ff82251f605a7618631d
Author: Ben Dover <noone@overthewire.org>
Date:   Sun Apr 23 18:04:40 2023 +0000

    initial commit of README.md
bandit29@bandit:/tmp/albertovc/repo$ git branch
* master
bandit29@bandit:/tmp/albertovc/repo$ git branch -r
  origin/HEAD -> origin/master
  origin/dev
  origin/master
  origin/sploits-dev
bandit29@bandit:/tmp/albertovc/repo$ git branch ckeckout dev
fatal: Not a valid object name: 'dev'.
bandit29@bandit:/tmp/albertovc/repo$ git branch -r
  origin/HEAD -> origin/master
  origin/dev
  origin/master
  origin/sploits-dev

bandit29@bandit:/tmp/albertovc/repo$ git branch
* master
bandit29@bandit:/tmp/albertovc/repo$ git checkout dev
Branch 'dev' set up to track remote branch 'dev' from 'origin'.
Switched to a new branch 'dev'
bandit29@bandit:/tmp/albertovc/repo$ cat README.md 
# Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
