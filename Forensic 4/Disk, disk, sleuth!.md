**Reto:** Disk, disk, sleuth!

**Descripción:**
Use `srch_strings` from the sleuthkit and some terminal-fu to find a flag in this disk image: [dds1-alpine.flag.img.gz](https://mercury.picoctf.net/static/2f998eee12730cf5766624681212a441/dds1-alpine.flag.img.gz)


**Solución:**
Descargue el archivo use gzip -d dds1-alpine.flag.img.gzpara descomprimirlo y para encontrar la bandera 
srch_strings dds1-alpine.flag.img | grep pico
ffffffff81399ccf t pirq_pico_get
ffffffff81399cee t pirq_pico_set
ffffffff820adb46 t pico_router_probe
  SAY picoCTF{f0r3ns1c4t0r_n30phyt3_267e38f6}

**Notas adicionales:**

**Referencias:** 