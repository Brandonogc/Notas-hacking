**Reto:** Glitch Cat

**Descripción:**
¡Nuestro servicio de impresión de banderas ha comenzado a fallar!`$ nc saturn.picoctf.net 56068`

**Solución:**
brandonogc0107-picoctf@webshell:~$ nc saturn.picoctf.net 56068
'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'
brandonogc0107-picoctf@webshell:~$ python
Python 3.10.12 (main, Feb  4 2025, 14:57:36) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
 print(chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65))
a4392d2e

picoCTF{gl17ch_m3_n07_a4392d2e}
**Notas adicionales:**
la terminal de los retos tambien tiene python, El código en Python usa la función `chr()` para convertir valores en hexadecimal a sus caracteres ASCII correspondientes y luego los concatena con `+`
**Referencias:** 
https://play.picoctf.org/practice/challenge/242?category=5&originalEvent=69&page=1

