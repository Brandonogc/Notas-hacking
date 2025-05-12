Brandon Omar Cárdenas González
Luis Jesús Quintero Bañuelos  

**Reto:** hideme

**Descripción:**
Every file gets a flag. The SOC analyst saw one image been sent back and forth between two people. They decided to investigate and found out that there was more than what meets the eye [here](https://artifacts.picoctf.net/c/262/flag.png).

**Solución:**
primero descargamos el archivo con wget https://artifacts.picoctf.net/c/259/flag.png
 y le hacemos un string y vemos una palabra clave que es 
secret/flag.png
le hacemos un binwalk para ver que tiene
luego le damos un binwalk -e flag.png
 binwalk -e flag.png

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             PNG image, 512 x 504, 8-bit/color RGBA, non-interlaced
41            0x29            Zlib compressed data, compressed
39739         0x9B3B          Zip archive data, at least v1.0 to extract, name: secret/
39804         0x9B7C          Zip archive data, at least v2.0 to extract, compressed size: 2869, uncompressed size: 3024, name: secret/flag.png
42908         0xA79C          End of Zip archive, footer length: 22

$ ls
y nos da unos archivos de flag asi que entramos con cd 
luego le damos un sz a flag.png y nos da una imagen, donde se encuentra la bandera

$ binwalk -e flag.png 

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             PNG image, 512 x 504, 8-bit/color RGBA, non-interlaced
41            0x29            Zlib compressed data, compressed
39739         0x9B3B          Zip archive data, at least v1.0 to extract, name: secret/
39804         0x9B7C          Zip archive data, at least v2.0 to extract, compressed size: 2869, uncompressed size: 3024, name: secret/flag.png
42908         0xA79C          End of Zip archive, footer length: 22

-picoctf@webshell:~/enc$ ls
_flag.png.extracted  flag.png
-picoctf@webshell:~/enc$ 

 ls
_flag.png.extracted  flag.png
-picoctf@webshell:~/enc$ ^C
-picoctf@webshell:~/enc$ cd _flag.png.extracted/
-picoctf@webshell:~/enc/_flag.png.extracted$ ls
29  29.zlib  9B3B.zip  secret
-picoctf@webshell:~/enc/_flag.png.extracted$ cd secret/
-picoctf@webshell:~/enc/_flag.png.extracted/secret$ ls
flag.png
-picoctf@webshell:~/enc/_flag.png.extracted/secret$ sz flag.png 
PNGg.png 100.00% 2.95 KB/2.95 KB


BANDERA
picoCTF{Hiddinng_An_imag3_within_@n_ima9e_82101824}

**Notas adicionales:**

**Referencias:** 
