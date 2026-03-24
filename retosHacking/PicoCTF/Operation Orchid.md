### Operation Orchid
#### Descripción

Descarga esta imagen de disco y encuentra la bandera.Nota: si usas el webshell, descarga y extrae la imagen de disco que no sea tu directorio principal.`/tmp`

- [Descargar imagen de disco comprimida](https://artifacts.picoctf.net/c/212/disk.flag.img.gz)
```
mmls disk.flag.img
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000206847   0000204800   Linux (0x83)
003:  000:001   0000206848   0000411647   0000204800   Linux Swap / Solaris x86 (0x82)
004:  000:002   0000411648   0000819199   0000407552   Linux (0x83)

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ fl -o 0000411648 disk.flag.img
fl: command not found

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ fls -o 0000411648 disk.flag.img
d/d 460:        home
d/d 11: lost+found
d/d 12: boot
d/d 13: etc
d/d 81: proc
d/d 82: dev
d/d 83: tmp
d/d 84: lib
d/d 87: var
d/d 96: usr
d/d 106:        bin
d/d 120:        sbin
d/d 466:        media
d/d 470:        mnt
d/d 471:        opt
d/d 472:        root
d/d 473:        run
d/d 475:        srv
d/d 476:        sys
d/d 2041:       swap
V/V 51001:      $OrphanFiles

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ fls -o 0000411648 disk.flag.img 472
r/r 1875:       .ash_history
r/r * 1876(realloc):    flag.txt
r/r 1782:       flag.txt.enc

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ icat -o 0000411648 disk.flag.img 1876
           -0.881573            34.311733

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ icat -o 0000411648 disk.flag.img 1882

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ icat -o 0000411648 disk.flag.img 1782
Salted__0��!�-6V����0�U��l��&�:�pj_1�0�|�h
                                          �Ȥ7� ���؎$�'%
┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ icat -o 0000411648 disk.flag.img 1875
touch flag.txt
nano flag.txt
apk get nano
apk --help
apk add nano
nano flag.txt
openssl
openssl aes256 -salt -in flag.txt -out flag.txt.enc -k unbreakablepassword1234567
shred -u flag.txt
ls -al
halt

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ openssl aes256 -salt -in flag.txt -out flag.txt.enc -k unbreakablepassword1234567^C

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ icat -o 0000411648 disk.flag.img 1782 > flag.txt.enc

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ openssl aes256 -salt -d -in flag.txt.enc -out flag.txt -k unbreakablepassword1234567
*** WARNING : deprecated key derivation used.
Using -iter or -pbkdf2 would be better.
bad decrypt
40A7A4631E7D0000:error:1C800064:Provider routines:ossl_cipher_unpadblock:bad decrypt:../providers/implementations/ciphers/ciphercommon_block.c:107:

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/OperationOrchid]
└─$ cat flag.txt
picoCTF{h4un71ng_p457_0a710765}
```