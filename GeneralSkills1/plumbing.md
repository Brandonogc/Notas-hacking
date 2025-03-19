**Reto:** plumbing

**Descripción:** 
A veces necesitas gestionar datos de procesos fuera de un archivo. ¿Puedes encontrar una manera de conservar la salida de este programa y buscar la bandera? Conéctate a `jupiter.challenges.picoctf.org 14291`.

**Solución:**
brandonogc0107-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 14291 >> flagout.txt

brandonogc0107-picoctf@webshell:~$ ls
README.txt  challenge.zip  challenge.zip.1  challenge.zip.2  challenge.zip.3  challenge.zip.4  challenge.zip.5  drop-in  file  flag  flagout.txt
brandonogc0107-picoctf@webshell:~$ cat flagout.txt | grep picoCTF
==picoCTF{digital_plumb3r_ea8bfec7}==


**Notas adicionales:**

**Referencias:** 