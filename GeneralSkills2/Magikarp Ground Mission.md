**Reto:** Magikarp Ground Mission

**Descripción:**
¿Sabes cómo navegar entre directorios y leer archivos en el shell? Inicia el contenedor, accede a él por ssh y, una vez conectado, por ssh. Inicia sesión por ssh como ctf-player y usa la contraseña a13b7f9d.

**Solución:**
brandonogc0107-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ ssh ctf-player@venus.picoctf.net -p 57176


ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ cat 1of3.flag.txt 
picoCTF{xxsh_
ctf-player@pico-chall$ cat instructions-to-2of3.txt 
Next, go to the root of all things, more succinctly `/`
ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ ls
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
ctf-player@pico-chall$ cat 2of3.flag.txt 
0ut_0f_\/\/4t3r_
ctf-player@pico-chall$ cat instructions-to-3of3.txt 
Lastly, ctf-player, go home... more succinctly `~`
ctf-player@pico-chall$ cd home/
ctf-player@pico-chall$ ls
ctf-player
ctf-player@pico-chall$ cd ctf-player/
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cat 3of3.flag.txt 
71be5264}

picoCTF{xxsh_0ut_0f_\/\/4t3r_71be5264}
**Notas adicionales:**

**Referencias:** 
https://youtu.be/duEwM4xC-dw?si=XKuwYzT9VqlaVo_v

