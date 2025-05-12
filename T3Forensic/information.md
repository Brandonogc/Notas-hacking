Brandon Omar Cárdenas González
Luis Jesús Quintero Bañuelos  

**Reto:**  information

**Descripción:**
Files can always be changed in a secret way. Can you find the flag? [cat.jpg](https://mercury.picoctf.net/static/a614a27d4cb251d04c7d2f3f3f76a965/cat.jpg)
**Solución:**
descargamos el archivo con wget https://mercury.picoctf.net/static/e5825f58ef798fdd1af3f6013592a971/cat.jpg
y nos da una imagen 
vamos a darle un exiftool a la imagen a ver que nos aparece 
y con la informacion, vemos que en la parte de la license hay un codigo que nos interesa
License                         : cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9
vamos a cyberchef a ver que nos dice 
que es nuestra bandera

picoCTF{the_m3tadata_1s_modified}
**Notas adicionales:**

**Referencias:** 
https://www.youtube.com/watch?v=uG42AMp0XHU