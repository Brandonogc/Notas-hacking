**Reto:** WebNet0

**Descripción:**
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.

**Solución:**
Descargamos los archivos, entramos al capture.pcap con wireshark y agragamos la llave, en edit preferences, protocolo tls y agegamos la llave encontramos la bandera en el paquete 35 
picoCTF{nongshim.shrimp.crackers}

**Notas adicionales:**

**Referencias:** 
Clase