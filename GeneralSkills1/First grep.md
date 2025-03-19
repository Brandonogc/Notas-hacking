**Reto:** First Grep

**Descripción:**
¿Puedes encontrar la bandera en [el archivo](https://jupiter.challenges.picoctf.org/static/495d43ee4a2b9f345a4307d053b4d88d/file) ? Sería muy tedioso revisarlo manualmente, pero algo me dice que hay una mejor manera.

**Solución:**
brandonogc0107-picoctf@webshell:~$ wget https://jupiter.challenges.picoctf.org/static/495d43ee4a2b9f345a4307d053b4d88d/file
brandonogc0107-picoctf@webshell:~$ ls
README.txt  challenge.zip  challenge.zip.1  challenge.zip.2  challenge.zip.3  challenge.zip.4  challenge.zip.5  drop-in  file
brandonogc0107-picoctf@webshell:~$ file file
file: ASCII text, with very long lines (4200)
brandonogc0107-picoctf@webshell:~$ cat file | grep "picoCTF"
==picoCTF{grep_is_good_to_find_things_dba08a45}==

**Notas adicionales:**

**Referencias:** 
https://youtu.be/CLm4SDekpUs?si=Qdtf8rmBPBEOaBbD