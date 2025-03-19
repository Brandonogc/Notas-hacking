**Reto:** Static ain't always noise

**Descripción:**
¿Puedes ver los datos en este binario: [static](https://mercury.picoctf.net/static/e9dd71b5d11023873b8abe99cdb45551/static) ? ¡Este [script BASH](https://mercury.picoctf.net/static/e9dd71b5d11023873b8abe99cdb45551/ltdis.sh) podría ayudarte!

**Solución:**
brandonogc0107-picoctf@webshell:~$ ls
README.txt  challenge.zip  challenge.zip.1  challenge.zip.2  challenge.zip.3  challenge.zip.4  challenge.zip.5  drop-in  file  flag  flagout.txt  ltdis.sh  static  strings  warm
brandonogc0107-picoctf@webshell:~$ cat ltdis.sh 

brandonogc0107-picoctf@webshell:~$ cat static | grep picoCTF
grep: (standard input): binary file matches
brandonogc0107-picoctf@webshell:~$ strings static 
/lib64/ld-linux-x86-64.so.2
libc.so.6
puts
__cxa_finalize
__libc_start_main
GLIBC_2.2.5
_ITM_deregisterTMCloneTable
__gmon_start__
_ITM_registerTMCloneTable
AWAVI
AUATL
[]A\A]A^A_
Oh hai! Wait what? A flag? Yes, it's around here somewhere!
;*3$"
==picoCTF{d15a5m_t34s3r_ae0b3ef2}==
GCC: (Ubuntu 7.5.0-3ubuntu1~18.04) 7.5.0
crtstuff.c
deregister_tm_clones
__do_global_dtors_aux
completed.7698
__do_global_dtors_aux_fini_array_entry
frame_dummy
__frame_dummy_init_array_entry
static.c
__FRAME_END__
__init_array_end
_DYNAMIC
__init_array_start
__GNU_EH_FRAME_HDR
_GLOBAL_OFFSET_TABLE_
__libc_csu_fini
_ITM_deregisterTMCloneTable
puts@@GLIBC_2.2.5
_edata
__libc_start_main@@GLIBC_2.2.5
__data_start
__gmon_start__
__dso_handle
_IO_stdin_used
__libc_csu_init
__bss_start
main
__TMC_END__
_ITM_registerTMCloneTable
flag
__cxa_finalize@@GLIBC_2.2.5
.symtab
.strtab
.shstrtab
.interp
.note.ABI-tag
.note.gnu.build-id
.gnu.hash
.dynsym
.dynstr
.gnu.version
.gnu.version_r
.rela.dyn
.rela.plt
.init
.plt.got
.text
.fini
.rodata
.eh_frame_hdr
.eh_frame
.init_array
.fini_array
.dynamic
.data
.bss
.comment

==picoCTF{d15a5m_t34s3r_ae0b3ef2}==
**Notas adicionales:**

**Referencias:** 
https://youtu.be/kEembVtyaGk?si=Mb5KPQlFpQx0945v
