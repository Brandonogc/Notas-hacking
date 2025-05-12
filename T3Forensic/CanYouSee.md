Brandon Omar Cárdenas González
Luis Jesús Quintero Bañuelos  

**Reto:** CanYouSee

**Descripción:**
How about some hide and seek?
Download this file here.

**Solución:**
vamos a descargar el archivo con Wget https://artifacts.picoctf.net/c_titan/5/unknown.zip
Y le vamos a dar unzip 
despues le vamos dar exiftool a nuestro archivo y nos mostrara varia unformacion, copiamos una que es
brandon@DESKTOP-VC9BR11:~/Ciber/retos/Canyousee$ exiftool ukn_reality.jpg
ExifTool Version Number         : 12.40
File Name                       : ukn_reality.jpg
Directory                       : .
File Size                       : 2.2 MiB
File Modification Date/Time     : 2024:03:11 18:05:57-06:00
File Access Date/Time           : 2024:03:11 18:05:57-06:00
File Inode Change Date/Time     : 2025:05:11 22:01:53-06:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
Resolution Unit                 : inches
X Resolution                    : 72
Y Resolution                    : 72
XMP Toolkit                     : Image::ExifTool 11.88
Attribution URL                 : cGljb0NURntNRTc0RDQ3QV9ISUREM05fZDhjMzgxZmR9Cg==
Image Width                     : 4308
Image Height                    : 2875
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 4308x2875
Megapixels                      : 12.4
y una ves copiado nos vamos a cyberchef y nos pone BASE64 lo cual es nuestra bandera

BANDERA
picoCTF{ME74D47A_HIDD3N_d8c381fd}

**Notas adicionales:**


**Referencias:** 
https://www.youtube.com/watch?v=VTx9DSfEcmM&pp=ygUTY2FueW91c2VlbWUgcGljb2N0Zg%3D%3D