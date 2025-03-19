**Reto:** Wave a flag

**Descripción:**
¿Se pueden invocar indicadores de ayuda para una herramienta o un binario? [Este programa](https://mercury.picoctf.net/static/a14be2648c73e3cda5fc8490a2f476af/warm) contiene información muy útil...

**Solución:**
brandonogc0107-picoctf@webshell:~$ wget https://mercury.picoctf.net/static/a14be2648c73e3cda5fc8490a2f476af/warm

brandonogc0107-picoctf@webshell:~$ ./warm
-bash: ./warm: Permission denied
brandonogc0107-picoctf@webshell:~$ chmod +x warm
brandonogc0107-picoctf@webshell:~$ ls
README.txt  challenge.zip  challenge.zip.1  challenge.zip.2  challenge.zip.3  challenge.zip.4  challenge.zip.5  drop-in  file  flag  flagout.txt  strings  warm
brandonogc0107-picoctf@webshell:~$ ./warm
Hello user! Pass me a -h to learn what I can do!
brandonogc0107-picoctf@webshell:~$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: ==picoCTF{b1scu1ts_4nd_gr4vy_755f3544}==


**Notas adicionales:**
**`chmod +x warm`**: Luego, cambias los permisos del archivo para hacerlo ejecutable utilizando el comando `chmod +x warm`. Esto le da al archivo el permiso necesario para que pueda ejecutarse como un programa.
**Referencias:** 
https://play.picoctf.org/practice/challenge/170?category=5&originalEvent=34&page=1
https://youtu.be/hj_0TUD-ss4?si=lBlcT2n3LFQ-S_GE
