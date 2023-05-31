# Level 31

## Objetivo
There is a git repository at `ssh://bandit31-git@localhost/home/bandit31-git/repo` via the port `2220`. The password for the user `bandit31-git` is the same as for the user `bandit31`.

Clone the repository and find the password for the next level.

## Datos de Acceso
bandit30
OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt

## Solución
Eliminamos el .gitignore ya que no nos permitirá enviar .txt, después creamos y enviamos el archivo con el contenido indicado.  

```bash
bandit31@bandit:~$ mkdir /tmp/alberto_vc
bandit31@bandit:~$ cd /tmp/alberto_vc
bandit31@bandit:/tmp/alberto_vc$ git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo
Cloning into 'repo'...
The authenticity of host '[localhost]:2220 ([127.0.0.1]:2220)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit31/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit31/.ssh/known_hosts).
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

bandit31-git@localhost's password: 
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (4/4), 381 bytes | 381.00 KiB/s, done.
bandit31@bandit:/tmp/alberto_vc$ pass=OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt
bandit31@bandit:/tmp/alberto_vc$ pass=OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt
bandit31@bandit:/tmp/alberto_vc$ pass=OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt
bandit31@bandit:/tmp/alberto_vc$ cd repo/
bandit31@bandit:/tmp/alberto_vc/repo$ ls -la
total 20
drwxrwxr-x 3 bandit31 bandit31 4096 May 31 21:39 .
drwxrwxr-x 3 bandit31 bandit31 4096 May 31 21:39 ..
drwxrwxr-x 8 bandit31 bandit31 4096 May 31 21:39 .git
-rw-rw-r-- 1 bandit31 bandit31    6 May 31 21:39 .gitignore
-rw-rw-r-- 1 bandit31 bandit31  147 May 31 21:39 README.md
bandit31@bandit:/tmp/alberto_vc/repo$ cat .git
cat: .git: Is a directory
bandit31@bandit:/tmp/alberto_vc/repo$ cat .git
.git/       .gitignore  
bandit31@bandit:/tmp/alberto_vc/repo$ cat .gitignore 
*.txt
bandit31@bandit:/tmp/alberto_vc/repo$ rm .gitignore 
bandit31@bandit:/tmp/alberto_vc/repo$ cat README.md 
This time your task is to push a file to the remote repository.

Details:
    File name: key.txt
    Content: 'May I come in?'
    Branch: master

bandit31@bandit:/tmp/alberto_vc/repo$ git branch
* master
bandit31@bandit:/tmp/alberto_vc/repo$ echo "May I come in?" > key.txt
bandit31@bandit:/tmp/alberto_vc/repo$ ls
key.txt  README.md
bandit31@bandit:/tmp/alberto_vc/repo$ cat key.txt 
May I come in?
bandit31@bandit:/tmp/alberto_vc/repo$ git add .
bandit31@bandit:/tmp/alberto_vc/repo$ git commit -am "File added"
[master da2292c] File added
 2 files changed, 1 insertion(+), 1 deletion(-)
 delete mode 100644 .gitignore
 create mode 100644 key.txt
bandit31@bandit:/tmp/alberto_vc/repo$ git push origin master
The authenticity of host '[localhost]:2220 ([127.0.0.1]:2220)' can't be established.
ED25519 key fingerprint is SHA256:C2ihUBV7ihnV1wUXRb4RrEcLfXC5CXlhmAAM/urerLY.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Could not create directory '/home/bandit31/.ssh' (Permission denied).
Failed to add the host to the list of known hosts (/home/bandit31/.ssh/known_hosts).
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

bandit31-git@localhost's password: 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 287 bytes | 287.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: ### Attempting to validate files... ####
remote: 
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote: 
remote: Well done! Here is the password for the next level:
remote: rmCBvG56y58BXzv98yZGdO7ATVL5dW8y 
remote: 
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote: 
To ssh://localhost:2220/home/bandit31-git/repo

```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
