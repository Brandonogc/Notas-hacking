**Reto:** time machine 

**Descripción:** 
What was I last working on? I remember writing a note to help me remember...You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_titan/161/challenge.zip)

**Solución:**
wget https://artifacts.picoctf.net/c_titan/161/challenge.zip
--2025-03-19 03:50:27--  https://artifacts.picoctf.net/c_titan/161/challenge.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.16, 3.160.22.128, 3.160.22.43, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.16|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 17739 (17K) [application/octet-stream]
Saving to: 'challenge.zip.5'

challenge.zip.5                                                                100%[====================================================================================================================================================================================================>]  17.32K  --.-KB/s    in 0.001s  

2025-03-19 03:50:27 (20.8 MB/s) - 'challenge.zip.5' saved [17739/17739]

brandonogc0107-picoctf@webshell:~$ unzip challenge.zip.5
Archive:  challenge.zip.5
replace drop-in/message.txt? [y]es, [n]o, [A]ll, [N]one, [r]ename: A
  inflating: drop-in/message.txt     
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
 extracting: drop-in/.git/objects/43/246218ab4fc7b30e9a9dff073e012316851469  
 extracting: drop-in/.git/objects/25/16effb8d70e33bdd0023629b164a77225e1ec2  
 extracting: drop-in/.git/objects/10/228f3d6437701ef5aaac04213757031f30ebec  
  inflating: drop-in/.git/index      
 extracting: drop-in/.git/COMMIT_EDITMSG  
  inflating: drop-in/.git/logs/HEAD  
  inflating: drop-in/.git/logs/refs/heads/master  
brandonogc0107-picoctf@webshell:~$ cd drop-in/
brandonogc0107-picoctf@webshell:~/drop-in$ ls -la
total 44
drwxr-xr-x 4 brandonogc0107-picoctf brandonogc0107-picoctf   115 Mar 19 03:50 .
drwxr-xr-x 4 brandonogc0107-picoctf brandonogc0107-picoctf  4096 Mar 19 03:50 ..
drwxr-xr-x 8 brandonogc0107-picoctf brandonogc0107-picoctf  4096 Mar 19 03:50 .git
-rw-rw-r-- 1 brandonogc0107-picoctf brandonogc0107-picoctf 24646 Mar 12  2024 challenge.zip
drwxr-xr-x 3 brandonogc0107-picoctf brandonogc0107-picoctf    33 Mar 17 22:56 drop-in
-rw-r--r-- 1 brandonogc0107-picoctf brandonogc0107-picoctf    22 Mar  9  2024 message.py
-rw-r--r-- 1 brandonogc0107-picoctf brandonogc0107-picoctf    87 Mar 12  2024 message.txt
brandonogc0107-picoctf@webshell:~/drop-in$ cat message.txt
This is what I was working on, but I'd need to look at my commit history to know why...

brandonogc0107-picoctf@webshell:~/drop-in$ git reflog
10228f3 (HEAD -> master) HEAD@{0}: commit (initial): ==picoCTF{t1m3m@ch1n3_8defe16a}==
**Notas adicionales:**

**Referencias:** 
https://youtu.be/Mmm9RXWKwhA?si=BqmIbrrY2l52q6Dl 