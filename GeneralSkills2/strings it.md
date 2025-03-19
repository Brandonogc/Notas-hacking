**Reto:** strings it

**Descripción:**
¿Puedes encontrar la bandera en [el archivo](https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings) sin ejecutarlo?

**Solución:**
brandonogc0107-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings
brandonogc0107-picoctf@webshell:~$ ls
README.txt  challenge.zip  challenge.zip.1  challenge.zip.2  challenge.zip.3  challenge.zip.4  challenge.zip.5  drop-in  file  flag  flagout.txt  strings
brandonogc0107-picoctf@webshell:~$ strings strings


brandonogc0107-picoctf@webshell:~$ strings n-10 strings | grep pico*
strings: 'n-10': No such file
==picoCTF{5tRIng5_1T_d66c7bb7}==

**Notas adicionales:**
**`strings n-10 strings`**: El comando `strings` se utiliza para mostrar las cadenas de texto legibles dentro de un archivo binario o un archivo no textual.

**Referencias:** 
https://linux.die.net/man/1/strings
