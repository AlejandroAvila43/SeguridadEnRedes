### Static ain't always noise
#### Descripción

¿Puedes mirar los datos en este binario? ¡El script de bash podría ayudar![estática](https://challenge-files.picoctf.net/c_wily_courier/b06384f5fdb3a6e3f0f254d1064d203e7df4bf7e9a5780a95622523367d82bc0/static), [ltdis.sh](https://challenge-files.picoctf.net/c_wily_courier/b06384f5fdb3a6e3f0f254d1064d203e7df4bf7e9a5780a95622523367d82bc0/ltdis.sh)

```
Ale5623-picoctf@webshell:~$ file *
README.txt: ASCII text, with escape sequences
file:       ASCII text, with very long lines (14545)
flag:       ASCII text
ltdis.sh:   Bourne-Again shell script, ASCII text executable
static:     ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=9a00d4dca6b92d22aa0cd1fceffa4ed7495b8534, for GNU/Linux 3.2.0, not stripped
strings:    ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=7e75296600ba106fbad1dd18137218feed44ecd9, for GNU/Linux 3.2.0, not stripped
warm:       ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=9e46ec8729d2f2aa8ffc4b1cdc058081bddcfe67, for GNU/Linux 3.2.0, with debug_info, not stripped
Ale5623-picoctf@webshell:~$ ./ltdis.sh
-bash: ./ltdis.sh: Permission denied
Ale5623-picoctf@webshell:~$ chm
chmem  chmod  
Ale5623-picoctf@webshell:~$ chmod +x ltdis.sh
Ale5623-picoctf@webshell:~$ ./ltdis.sh
Attempting disassembly of  ...
objdump: 'a.out': No such file
objdump: section '.text' mentioned in a -j option, but not found in any input file
Disassembly failed!
Usage: ltdis.sh <program-file>
Bye!
Ale5623-picoctf@webshell:~$ ./ltdis.sh static
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset
Ale5623-picoctf@webshell:~$ ls
README.txt  file  flag  ltdis.sh  static  static.ltdis.strings.txt  static.ltdis.x86_64.txt  strings  warm
Ale5623-picoctf@webshell:~$ cat static.ltdis.strings.txt |grep pico
   3020 picoCTF{d15a5m_t34s3r_20335e41}
```