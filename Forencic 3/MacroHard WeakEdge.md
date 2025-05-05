
**Reto:** MacroHard WeakEdge

**Descripción:**
I've hidden a flag in this file. Can you find it? [Forensics is fun.pptm](https://mercury.picoctf.net/static/c0da20f29337e87ffb58ea987d8c596e/Forensics is fun.pptm)

**Solución:**
descargamos y abrimos el archivo y depues entramos a /Ciber/retos/macro/macro/ppt/slideMasters despues usamos cat para el archivo hidden y encontamos esta cadena: Z m x h Z z o g c G l j b 0 N U R n t E M W R f d V 9 r b j B 3 X 3 B w d H N f c l 9 6 M X A 1 f Q y para encontrar la bandera usamos el siguiente comando : 
cat hidden | sed 's/ //g' | base64 -d
flag: picoCTF{D1d_u_kn0w_ppts_r_z1p5}




**Notas adicionales:**

**Referencias:** 
https://youtu.be/c5mphZsRvKQ?si=oEl_E_7CIViuc_lI