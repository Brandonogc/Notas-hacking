**Reto:** Búsqueda binaria  

**Descripción:** ¿Quieres jugar? A medida que uses más el shell, ¡quizás te interese saber cómo funcionan! La búsqueda binaria es un algoritmo clásico para encontrar rápidamente un elemento en una lista ordenada. ¿Puedes encontrar la bandera? Tendrás 1000 posibilidades y solo 10 intentos.La ciberseguridad suele requerir una gran cantidad de datos que analizar, desde registros y reportes de vulnerabilidad hasta análisis forense. Practicar los fundamentos manualmente podría ayudarte en el futuro cuando tengas que desarrollar tus propias herramientas.Puedes descargar los archivos del desafío aquí:

- [desafío.zip](https://artifacts.picoctf.net/c_atlas/20/challenge.zip)

`ssh -p 60836 ctf-player@atlas.picoctf.net`Usando la contraseña `6abf4a82`. Acepta la huella digital con `yes`y, `ls`una vez conectado, comienza. Recuerda: en un shell, las contraseñas están ocultas.

**Solución:** 
brandonogc0107-picoctf@webshell:~$ ssh -p 56314 ctf-player@atlas.picoctf.net
ctf-player@atlas.picoctf.net's password: `6abf4a82` 
Welcome to the Binary Search Game!
I'm thinking of a number between 1 and 1000.
Enter your guess: 500
Lower! Try again.
Enter your guess: 600
Lower! Try again.
Enter your guess: 350
Higher! Try again.
Enter your guess: 400
Lower! Try again.
Enter your guess: 353
Higher! Try again.
Enter your guess: 360
Higher! Try again.
Enter your guess: 365
Lower! Try again.
Enter your guess: 362
Lower! Try again.
Enter your guess: 361
Congratulations! You guessed the correct number: 361
Here's your flag: ==picoCTF{g00d_gu355_bee04a2a}==
Connection to atlas.picoctf.net closed.

**Notas adicionales:** 
comence de la mitad y fui buscando un numero que quedara en el rango hasta llegar al numero 360 que era el mas cercano y de ahi lo hice con prueba y error 

**Referencias:** 
https://play.picoctf.org/practice/challenge/442