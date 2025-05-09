**Reto:**  Sleuthkit Intro

**Descripción:**
#### Description

Download the disk image and use `mmls` on it to find the size of the Linux partition. Connect to the remote checker service to check your answer and get the flag. Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory. [Download disk image](https://artifacts.picoctf.net/c/164/disk.img.gz)

Additional details will be available after launching your challenge instance.

**Solución:**
gzip -d disk.img.gz
lsbrandon@DESKTOP-VC9BR11:~/Ciber/retos/Sleuthkit_Intro$ ls-la
ls-la: command not found
brandon@DESKTOP-VC9BR11:~/Ciber/retos/Sleuthkit_Intro$ ls -la
total 102408
drwxr-xr-x  2 brandon brandon      4096 May  8 20:18 .
drwxr-xr-x 26 brandon brandon      4096 May  8 20:07 ..
-rw-r--r--  1 brandon brandon 104857600 Aug  4  2023 disk.img
brandon@DESKTOP-VC9BR11:~/Ciber/retos/Sleuthkit_Intro$ mmls disk.img
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000204799   0000202752   Linux (0x83)
brandon@DESKTOP-VC9BR11:~/Ciber/retos/Sleuthkit_Intro$ nc saturn.picoctf.net 57712
What is the size of the Linux partition in the given disk image?
Length in sectors: 202752
202752
Great work!
picoCTF{mm15_f7w!}

**Notas adicionales:**

**Referencias:** 
