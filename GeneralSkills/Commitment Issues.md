**Reto:** Commitment Issues

**Descripción:**
Anoté la bandera sin querer. ¡Menos mal que la borré!Puedes descargar los archivos del desafío aquí:

- [desafío.zip](https://artifacts.picoctf.net/c_titan/77/challenge.zip)
**Solución:**
brandonogc0107-picoctf@webshell:~$ unzip challenge.zip.4 
Archive:  challenge.zip.4
replace drop-in/.git/description? [y]es, [n]o, [A]ll, [N]one, [r]ename: A
  inflating: drop-in/.git/description  
  inflating: drop-in/.git/hooks/applypatch-msg.sample  
  inflating: drop-in/.git/hooks/commit-msg.sample  
  inflating: drop-in/.git/hooks/fsmonitor-watchman.sample  
  inflating: drop-in/.git/hooks/post-update.sample  
  inflating: drop-in/.git/hooks/pre-applypatch.sample  
  inflating: drop-in/.git/hooks/pre-commit.sample  
  inflating: drop-in/.git/hooks/pre-merge-commit.sample  
  inflating: drop-in/.git/hooks/pre-push.sample  
  inflating: drop-in/.git/hooks/pre-rebase.sample  
  inflating: drop-in/.git/hooks/pre-receive.sample  
  inflating: drop-in/.git/hooks/prepare-commit-msg.sample  
  inflating: drop-in/.git/hooks/update.sample  
  inflating: drop-in/.git/info/exclude  
 extracting: drop-in/.git/refs/heads/master  
 extracting: drop-in/.git/HEAD       
  inflating: drop-in/.git/config     
 extracting: drop-in/.git/objects/96/f7309de67d785ec0b93b8766ff2882bef5c3ef  
 extracting: drop-in/.git/objects/8c/1d254e2da6713e33acd6d622fc1dae357ec3c6  
 extracting: drop-in/.git/objects/3d/5ec8a26ee7b092a1760fea18f384c35e435139  
 extracting: drop-in/.git/objects/d5/52d1ecd2d83fa2e65b6724d1ff73b45a7d59b7  
 extracting: drop-in/.git/objects/0c/1ab266b7a3a1cd099bb509f82b7a2d03aecd03  
 extracting: drop-in/.git/objects/e1/237df82d2e69f62dd53279abc1c8aeb66f6d64  
  inflating: drop-in/.git/index      
 extracting: drop-in/.git/COMMIT_EDITMSG  
  inflating: drop-in/.git/logs/HEAD  
  inflating: drop-in/.git/logs/refs/heads/master  
 extracting: drop-in/message.txt     
brandonogc0107-picoctf@webshell:~$ ls
README.txt  challenge.zip  challenge.zip.1  challenge.zip.2  challenge.zip.3  challenge.zip.4  drop-in
brandonogc0107-picoctf@webshell:~$ cd drop-in/
brandonogc0107-picoctf@webshell:~/drop-in$ ls -la
total 44
drwxr-xr-x 4 brandonogc0107-picoctf brandonogc0107-picoctf   115 Mar 18 03:38 .
drwxr-xr-x 4 brandonogc0107-picoctf brandonogc0107-picoctf  4096 Mar 18 03:35 ..
drwxr-xr-x 8 brandonogc0107-picoctf brandonogc0107-picoctf  4096 Mar 18 03:38 .git
-rw-rw-r-- 1 brandonogc0107-picoctf brandonogc0107-picoctf 24646 Mar 12  2024 challenge.zip
drwxr-xr-x 3 brandonogc0107-picoctf brandonogc0107-picoctf    33 Mar 17 22:56 drop-in
-rw-r--r-- 1 brandonogc0107-picoctf brandonogc0107-picoctf    22 Mar  9  2024 message.py
-rw-r--r-- 1 brandonogc0107-picoctf brandonogc0107-picoctf    11 Mar  9  2024 message.txt
brandonogc0107-picoctf@webshell:~/drop-in$ cat massage.txt
cat: massage.txt: No such file or directory
brandonogc0107-picoctf@webshell:~/drop-in$ ca             
cachepic           caller             capinfos           capsh              captoinfo          captype            cargo              cargo-clippy       cargo-fmt          cas_help           case               cat                catman             cautious-launcher  
brandonogc0107-picoctf@webshell:~/drop-in$ cat message.txt
TOP SECRET
brandonogc0107-picoctf@webshell:~/drop-in$ git reflog

[1]+  Stopped                 git reflog
brandonogc0107-picoctf@webshell:~/drop-in$ git checkout 3d5ec8a
Note: switching to '3d5ec8a'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 3d5ec8a create flag
brandonogc0107-picoctf@webshell:~/drop-in$ cat message.txt
==picoCTF{s@n1t1z3_30e86d36}==



**Notas adicionales:**

Se utiliza el comando `unzip challenge.zip.4`, que descomprime un archivo ZIP fragmentado llamado `challenge.zip.4`. Al descomprimir, se extraen varios archivos dentro de una carpeta llamada `drop-in`. Esto incluye archivos relacionados con Git, como configuraciones y objetos.

Se ejecuta el comando `git reflog`, que muestra los registros de las acciones realizadas en el repositorio Git. El comando se detiene, probablemente debido a que el proceso está suspendido.

Luego, se usa `git checkout 3d5ec8a`, que cambia el estado del repositorio a un commit específico identificado por el hash `3d5ec8a`. Esto pone el repositorio en un estado conocido como "detached HEAD", lo que significa que no estás en ninguna rama, sino que has ido a un punto específico en la historia del repositorio.

**Referencias:**  
Wehling, L., & McNamara, M. (2016). _Hacking: The Art of Exploitation_. No Starch Press.
Git Documentation. (2023). _Git Documentation: git-reflog_. Retrieved from [https://git-scm.com/docs/git-reflog](https://git-scm.com/docs/git-reflog)
