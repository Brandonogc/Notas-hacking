**Reto:** Special

**Descripción:**

¿Los usuarios avanzados ya no se cansan de cometer errores ortográficos en la shell? ¡Ya no! Presentamos Special, la interfaz con corrección ortográfica para Linux. Ahora, cada palabra se escribe y escribe correctamente en mayúsculas... ¡automáticamente y en segundo plano! Sé el primero en probar Special en su versión beta y cuéntanos cómo Special optimiza cada proceso de desarrollo que enfrentas. Cuando tus compañeros vean tu increíble interfaz de shell, simplemente diles: ¡Eso es Special!Inicie su instancia para ver los detalles de la conexión.`ssh -p 54952 ctf-player@saturn.picoctf.net`La contraseña es`483e80d4`
**Solución:**
Special$ ls
Is 
sh: 1: Is: not found
Special$ clear
Clear 
sh: 1: Clear: not found
Special$ clear & cat./ blargh/flag.txt
Clear & catch blargh/flag.txt 
sh: 1: Clear: not found
sh: 1: catch: not found
Special$ clear & find
Clear & find 
sh: 1: Clear: not found
.
./blargh
./blargh/flag.txt
./.cache
./.cache/motd.legal-displayed
Special$ clear & cat ./blargh/flag.txt
Clear & cat ./blargh/flag.txt 
sh: 1: Clear: not found
==picoCTF{5p311ch3ck_15_7h3_w0r57_b741d1b1}==


**Notas adicionales:**

**Referencias:** 
https://youtu.be/6lEd1yVsxpw?si=xvYDDUUjdfnu8qIu