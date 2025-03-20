**Reto:**  Collaborative Development  

**Descripción:**
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/177/challenge.zip)
**Solución:**
brandonogc0107-picoctf@webshell:~/drop-in$ wget https://artifacts.picoctf.net/c_titan/177/challenge.zip
--2025-03-17 22:39:56--  https://artifacts.picoctf.net/c_titan/177/challenge.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.92, 3.160.22.128, 3.160.22.43, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.92|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 24646 (24K) [application/octet-stream]
Saving to: 'challenge.zip'

challenge.zip                                                                  100%[====================================================================================================================================================================================================>]  24.07K  --.-KB/s    in 0.008s  

2025-03-17 22:39:56 (2.79 MB/s) - 'challenge.zip' saved [24646/24646]

brandonogc0107-picoctf@webshell:~/drop-in$ unzip challenge.zip 

brandonogc0107-picoctf@webshell:~/drop-in$ cd drop-in/
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ ls -la
total 4
drwxr-xr-x 3 brandonogc0107-picoctf brandonogc0107-picoctf  33 Mar 12  2024 .
drwxr-xr-x 4 brandonogc0107-picoctf brandonogc0107-picoctf  92 Mar 17 22:40 ..
drwxr-xr-x 8 brandonogc0107-picoctf brandonogc0107-picoctf 166 Mar 12  2024 .git
-rw-r--r-- 1 brandonogc0107-picoctf brandonogc0107-picoctf  30 Mar 12  2024 flag.py

brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ cat flag.py 
print("Printing the flag...")
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ 

brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git reflog
d7d0954 (HEAD -> main) HEAD@{0}: checkout: moving from feature/part-3 to main
8fccfcd (feature/part-3) HEAD@{1}: commit: add part 3
d7d0954 (HEAD -> main) HEAD@{2}: checkout: moving from main to feature/part-3
d7d0954 (HEAD -> main) HEAD@{3}: checkout: moving from feature/part-2 to main
e1629c7 (feature/part-2) HEAD@{4}: commit: add part 2
d7d0954 (HEAD -> main) HEAD@{5}: checkout: moving from main to feature/part-2
d7d0954 (HEAD -> main) HEAD@{6}: checkout: moving from feature/part-1 to main
b2e0542 (feature/part-1) HEAD@{7}: commit: add part 1
d7d0954 (HEAD -> main) HEAD@{8}: checkout: moving from main to feature/part-1
d7d0954 (HEAD -> main) HEAD@{9}: commit (initial): init flag printer

brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git merge feature/part-1
Updating d7d0954..b2e0542
Fast-forward
 flag.py | 1 +
 1 file changed, 1 insertion(+)
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ cat flag.py 
print("Printing the flag...")
print("picoCTF{t3@mw0rk_", end='')brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ 
print("picoCTF{t3@mw0rk_", end='')brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git merge feature/part-2
Committer identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'brandonogc0107-picoctf@webshell.(none)')
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git config --global user.name random
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git config --global user.email random@gmail.com
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git merge feature/part-2
Auto-merging flag.py
CONFLICT (content): Merge conflict in flag.py
Automatic merge failed; fix conflicts and then commit the result.
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ cat flag.py 
print("Printing the flag...")
 HEAD
print("picoCTF{t3@mw0rk_", end='')

print("m@k3s_th3_dr3@m_", end='')
feature/part-2

brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git add flag.py 
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git commit -m megeg
[main 8f3ad03] megeg
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ cat flag.py 
print("Printing the flag...")
<<<<<<< HEAD
print("picoCTF{t3@mw0rk_", end='')

print("m@k3s_th3_dr3@m_", end='')
>>>>>>> feature/part-2
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git merge feature/part-3
Auto-merging flag.py
CONFLICT (content): Merge conflict in flag.py
Automatic merge failed; fix conflicts and then commit the result.
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git add flag.py 
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ git commit -m metged
[main 21bc2a6] metged
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ cat flag.py 
print("Printing the flag...")
<<<<<<< HEAD
<<<<<<< HEAD
print("picoCTF{t3@mw0rk_", end='')
=======

print("m@k3s_th3_dr3@m_", end='')
>>>>>>> feature/part-2
=======

print("w0rk_7ae8dd33}")
>>>>>>> feature/part-3
brandonogc0107-picoctf@webshell:~/drop-in/drop-in$ 


**Notas adicionales:**
El comando `git merge` en Git se utiliza para combinar los cambios de dos ramas diferentes. Específicamente, se utiliza para integrar los cambios de una rama (por lo general, una rama de desarrollo) a otra (usualmente la rama principal, como `main` o `master`).
**Referencias:** 