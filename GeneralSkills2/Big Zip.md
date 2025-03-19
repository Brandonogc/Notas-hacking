**Reto:** Big Zip 

**Descripción:**
Descomprime este archivo y busca la bandera.

- [Descargar archivo zip](https://artifacts.picoctf.net/c/503/big-zip-files.zip)

**Solución:**
brandonogc0107-picoctf@webshell:~$ unzip big-zip-files.zip 
brandonogc0107-picoctf@webshell:~$ grep -rl "pico"
README.txt
.bash_history
drop-in/.git/logs/refs/heads/master
drop-in/.git/logs/HEAD
drop-in/.git/COMMIT_EDITMSG
drop-in/drop-in/.git/logs/HEAD
drop-in/drop-in/.git/logs/refs/heads/main
drop-in/drop-in/.git/logs/refs/heads/feature/part-1
drop-in/drop-in/.git/logs/refs/heads/feature/part-2
drop-in/drop-in/.git/logs/refs/heads/feature/part-3
drop-in/drop-in/flag.py
challenge.zip.5
file
.wget-hsts
flag
flagout.txt
strings
warm
static
Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku/fang-of-haynekhtnamet
big-zip-files/folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt
brandonogc0107-picoctf@webshell:~$ cat big-zip-files/folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt
information on the record will last a billion years. Genes and brains and books encode ==picoCTF{gr3p_15_m4g1c_ef8790dc}==

**Notas adicionales:**
 **`grep`**: Busca texto dentro de archivos.
 **`-r`**: Busca de manera recursiva en todos los subdirectorios.
**`-l`**: Muestra solo los nombres de los archivos que contienen la palabra buscada (no muestra las líneas donde aparece).

**Referencias:**
https://youtu.be/YFJ9dXlUaZY?si=vcBOLTTFaiqS0van