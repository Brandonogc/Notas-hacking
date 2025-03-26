**Reto:** Client-side-again

**Descripción:**
¿Puedes entrar en este portal súper seguro? `https://jupiter.challenges.picoctf.org/problem/60786/`( [enlace](https://jupiter.challenges.picoctf.org/problem/60786/) ) o http://jupiter.challenges.picoctf.org:60786
**Solución:**
inspeccionamos la pagina `https://jupiter.challenges.picoctf.org/problem/60786/` 
despues tomamos la linea 10 y la desofucamos y despues en un javascript reorganizamos la bandera


var f = ['f49bf}', '_again_e', 'this', 'Password\x20Verified', 'Incorrect\x20password', 'getElementById', 'value', 'substring', 'picoCTF{', 'not_this'];

f[8]+f[9]+f[1]+f[0]

==picoCTF{not_this_again_ef49bf}==
**Notas adicionales:**
La ofuscación informática es un proceso que hace más difícil entender y aplicar ingeniería inversa al código de un programa.
**Referencias:** 
https://beautifier.io/
https://www.mycompiler.io/es/new/java