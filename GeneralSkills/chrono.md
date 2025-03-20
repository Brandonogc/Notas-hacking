**Reto:** chrono

**Descripción:**
¿Cómo automatizar tareas para que se ejecuten a intervalos en servidores Linux?Utilice ssh para conectarse a este servidor:

```
Server: saturn.picoctf.net
Port: 50516
Username: picoplayer 
Password: kZx-HVJKu8
```

**Solución:**
picoplayer@challenge:~$ crontab -e
no crontab for picoplayer - using an empty one
update-alternatives: error: no alternatives for editor
/usr/bin/sensible-editor: 25: editor: not found
/usr/bin/sensible-editor: 28: nano: not found
/usr/bin/sensible-editor: 31: nano-tiny: not found
/usr/bin/sensible-editor: 34: vi: not found
Couldn't find an editor!
Set the $EDITOR environment variable to your desired editor.
crontab: "/usr/bin/sensible-editor" exited with status 1
picoplayer@challenge:~$ cat /etc/crontab
==picoCTF{Sch3DUL7NG_T45K3_L1NUX_5b7059d0}==


**Notas adicionales:**

**Referencias:** 
https://youtu.be/PHNa4Wtsa44?si=XZm5PXuOZUAVirKu