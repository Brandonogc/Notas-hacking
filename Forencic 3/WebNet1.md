**Reto:** WebNet1

**Descripción:**
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/fbf98e695555a2a48fe42c9a245de376/picopico.key). Recover the flag.

**Solución:**
Descargamos los archivos, entramos al capture.pcap con wireshark y agragamos la llave, en edit preferences, protocolo tls y agegamos la llave encontramos la bandera en el paquete 91
picoCTF{honey.roasted.peanuts}

**Notas adicionales:**

**Referencias:** 
Clase