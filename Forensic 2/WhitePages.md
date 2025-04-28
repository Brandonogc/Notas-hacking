**Reto:**  WhitePages

**Descripción:**
I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://jupiter.challenges.picoctf.org/static/74274b96fe966126a1953c80762af80d/whitepages.txt) is all blank!

**Solución:**
descargamos y abrimos el archivo des pues usamos el comando 
sed 's/\xe2\x80\x83/0/g' whitepages.txt  | sed 's/ /1/g'
 
esto nos dara un codigo binario el cual meterempos al cyberchef para decodificarlo y encontraremos la bandera 
picoCTF{not_all_spaces_are_created_equal_c54f27cd05c2189f8147cc6f5deb2e56}

**Notas adicionales:**

**Referencias:** 