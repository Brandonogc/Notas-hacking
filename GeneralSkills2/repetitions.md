**Reto:** repetitions

**Descripción:**
¿Puedes darle sentido a este archivo?Descargue el archivo [aquí](https://artifacts.picoctf.net/c/477/enc_flag) .

**Solución:**

brandonogc0107-picoctf@webshell:~$ cat enc_flag 
VmpGU1EyRXlUWGxTYmxKVVYwZFNWbGxyV21GV1JteDBUbFpPYWxKdFVsaFpWVlUxWVZaS1ZWWnVh
RmRXZWtab1dWWmtSMk5yTlZWWApiVVpUVm10d1VWZFdVa2RpYlZaWFZtNVdVZ3BpU0VKeldWUkNk
MlZXVlhoWGJYQk9VbFJXU0ZkcVRuTldaM0JZVWpGS2VWWkdaSGRXCk1sWnpWV3hhVm1KRk5XOVVW
VkpEVGxaYVdFMVhSbHBWV0VKVVZGWmFWMDVHV2tkYVNHUlZDazFyY0ZkVWJGWlhZVlpLU0dWRlZs
aGkKYlRrelZERldUMkpzUWxWTlJYTkxDZz09Cg==
brandonogc0107-picoctf@webshell:~$ base 64 -d enc_flag 
-bash: base: command not found
brandonogc0107-picoctf@webshell:~$ base64 -d enc_flag 
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlpVWEJUVFZaV05GWkdaSGRVCk1rcFdUbFZXYVZKSGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==
brandonogc0107-picoctf@webshell:~$ base64 -d enc_flag | base64 -d
V1RCa2MyRnRTWGRVYkZaVFltNVNjRmRXYUU5aVJUVnhWVzFhYVdGck5UWmFSVkpQWVRGbmVWVnVR
bHBsYTBweVUxWmpNRTVHWjNsVgpXR1JyVFdwV2VsUlZVbE5oTURCNVZXMWFZUXBTTVZWNFZGZHdU
MkpWTlVWaVJHeEVXbm93T1VOblBUMEsK
brandonogc0107-picoctf@webshell:~$ base64 -d enc_flag | base64 -d | base64 -d 
WTBkc2FtSXdUbFZTYm5ScFdWaE9iRTVxVW1aaWFrNTZaRVJPYTFneVVuQlpla0pyU1ZjME5GZ3lV
WGRrTWpWelRVUlNhMDB5VW1aYQpSMVV4VFdwT2JVNUViRGxEWnowOUNnPT0K
brandonogc0107-picoctf@webshell:~$ base64 -d enc_flag | base64 -d | base64 -d | base64 -d
Y0dsamIwTlVSbnRpWVhObE5qUmZiak56ZEROa1gyUnBZekJrSVc0NFgyUXdkMjVzTURSa00yUmZa
R1UxTWpObU5EbDlDZz09Cg==
brandonogc0107-picoctf@webshell:~$ base64 -d enc_flag | base64 -d | base64 -d | base64 -d | base64 -d
cGljb0NURntiYXNlNjRfbjNzdDNkX2RpYzBkIW44X2Qwd25sMDRkM2RfZGU1MjNmNDl9Cg==
brandonogc0107-picoctf@webshell:~$ base64 -d enc_flag | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d
==picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_de523f49}==

**Notas adicionales:**

- Intente decodificarlo con `base64 -d enc_flag`, pero el texto resultante seguía estando codificado.
- Continuae aplicando `base64 -d` repetidamente hasta que la cadena se convirtió en texto legible.
  ==picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_de523f49}==

**Referencias:** 
https://youtu.be/PI2-KwgAhXk?si=oNJDKXlqLZZh5tO-
