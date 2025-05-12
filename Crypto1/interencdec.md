
**Reto:**  interencdec

**Descripción:**
Can you get the real meaning from this file. Download the file [here](https://artifacts.picoctf.net/c_titan/108/enc_flag).

**Solución:**
entramos al archivo y encontramos esta decodificacion base 64 d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrX2g0N2o2azY5fQ==
despues la decodificamos con 
echo d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrX2g0N2o2azY5fQ== | base64 -d
wpjvJAM{jhlzhy_k3jy9wa3k_h47j6k69} 
pero también lo tenemos que rotar asi que nos vamos a cyberchef y lo rotamos 19 veces y nos da de resultado 
picoCTF{caesar_d3cr9pt3d_a47c6d69}


**Notas adicionales:**

**Referencias:** 
