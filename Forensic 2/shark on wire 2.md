
**Reto:** shark on wire 2

**Descripción:**
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/b506393b6f9d53b94011df000c534759/capture.pcap). Recover the flag that was pilfered from the network.

**Solución:**
Entramos al wireshark y hacemos seguimiento de los paquetes, filtramos los paquetes udp cuyo puerto de destino sea el 22 extraemos los que sean mayor a 5000 y decodificamos los paquetes y cada paquete es una letra de la bandera 
picoCTF{p1LLf3r3d_data_v1a_st3g0}

**Notas adicionales:**

**Referencias:** 