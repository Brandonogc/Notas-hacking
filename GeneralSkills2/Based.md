**Reto:** Based

**Descripción:**
Para obtener el verdadero 1337, debes comprender diferentes codificaciones de datos, como hexadecimal o binaria. ¿Puedes obtener la bandera de este programa para demostrar que estás en camino de obtener el 1337? Conéctate con `nc jupiter.challenges.picoctf.org 29221`.

**Solución:**
brandonogc0107-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 29221
Let us see how data is stored
sludge
Please give the 01110011 01101100 01110101 01100100 01100111 01100101 as a word.
...
you have 45 seconds.....

Input:
sludge
Please give me the  143 157 154 157 162 141 144 157 as a word.
Input:
colorado
Please give me the 636f6e7461696e6572 as a word.
Input:
container
You've beaten the challenge
Flag: ==picoCTF{learning_about_converting_values_00a975ff}==
**Notas adicionales:**

**Referencias:** 
https://gchq.github.io/CyberChef/#recipe=From_Binary('Space',8)&input=IDAxMTEwMDExIDAxMTAxMTAwIDAxMTEwMTAxIDAxMTAwMTAwIDAxMTAwMTExIDAxMTAwMTAx
https://gchq.github.io/CyberChef/#recipe=From_Octal('Space')&input=MTQzIDE1NyAxNTQgMTU3IDE2MiAxNDEgMTQ0IDE1Nw&oeol=CR
https://gchq.github.io/CyberChef/#recipe=From_Hex('Auto')&input=IDYzNmY2ZTc0NjE2OTZlNjU3Mg

