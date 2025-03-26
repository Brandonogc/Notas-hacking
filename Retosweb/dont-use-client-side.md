
**Reto:** dont-use-client-side

**Descripción:**
¿Puedes entrar en este portal súper seguro? `https://jupiter.challenges.picoctf.org/problem/37821/`( [enlace](https://jupiter.challenges.picoctf.org/problem/37821/) ) o http://jupiter.challenges.picoctf.org:37821

**Solución:**
split=4 

|if (checkpass.substring(0, split) == 'pico') {|
||if (checkpass.substring(split*6, split*7) == 'a3c8') {|
||if (checkpass.substring(split, split*2) == 'CTF{') {|
||if (checkpass.substring(split*4, split*5) == 'ts_p') {|
||if (checkpass.substring(split*3, split*4) == 'lien') {|
||if (checkpass.substring(split*5, split*6) == 'lz_1') {|
||if (checkpass.substring(split*2, split*3) == 'no_c') {|
||if (checkpass.substring(split*7, split*8) == '9}') {|

==picoCTF{no_clients_plz_1a3c89}==

**Notas adicionales:**

**Referencias:** 