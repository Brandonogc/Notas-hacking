Brandon Omar Cárdenas González
Luis Jesús Quintero Bañuelos  

**Reto:** St3g0

**Descripción:**
Download this image and find the flag.

- [Download image](https://artifacts.picoctf.net/c/216/pico.flag.png)

**Solución:**
bueno descargamos la imagen para intentar resolverla y de pura tonteria hacemos un zsteg ypues para ver que tenia la imagen
entonces al hacerlo pues ahi venia la bandera
asi que viendo un video para ayudarnos vemos que efectivamente era hacer eso mismo, asi que encontramos la bandera
zsteg pico.flag.png
b1,rgb,lsb,xy       .. text: "picoCTF{7h3r3_15_n0_5p00n_a1062667}$t3g0"
b1,abgr,lsb,xy      .. text: "E2A5q4E%uSA"
b2,b,lsb,xy         .. text: "AAPAAQTAAA"
b2,b,msb,xy         .. text: "HWUUUUUU"
b3,r,lsb,xy         .. file: gfxboot compiled html help file
b4,r,lsb,xy         .. file: Targa image data (16-273) 65536 x 4097 x 1 +4352 +4369 - 1-bit alpha - right "\021\020\001\001\021\021\001\001\021\021\001"
b4,g,lsb,xy         .. file: 0420 Alliant virtual executable not stripped
b4,b,lsb,xy         .. file: Targa image data - Map 272 x 17 x 16 +257 +272 - 1-bit alpha "\020\001\021\001\021\020\020\001\020\001\020\001"
b4,bgr,lsb,xy       .. file: Targa image data - Map 273 x 272 x 16 +1 +4113 - 1-bit alpha "\020\001\001\001"
b4,rgba,msb,xy      .. file: Applesoft BASIC program data, first line number 8


**Notas adicionales:**


**Referencias:** 
https://www.youtube.com/watch?v=_IAjE_jUEOM

