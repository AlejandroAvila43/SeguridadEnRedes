### Wave a flag
#### Descripción

¿Se pueden invocar flags de ayuda para una herramienta o un binario? Este programa tiene información extraordinariamente útil...[Cálido](https://challenge-files.picoctf.net/c_wily_courier/70013ed41d4cfe2bb48628471dac6fc12238b5dbe164301ae3b4e35277b1e80b/warm)

```
Ale5623-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_wily_courier/70013ed41d4cfe2bb48628471dac6fc12238b5dbe164301ae3b4e35277b1e80b/warm
--2026-02-11 14:16:49--  https://challenge-files.picoctf.net/c_wily_courier/70013ed41d4cfe2bb48628471dac6fc12238b5dbe164301ae3b4e35277b1e80b/warm
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.95, 3.160.5.18, 3.160.5.40, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.95|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 19312 (19K) [application/octet-stream]
Saving to: 'warm'

warm                                                       100%[======================================================================================================================================>]  18.86K  --.-KB/s    in 0.002s  

2026-02-11 14:16:49 (9.06 MB/s) - 'warm' saved [19312/19312]

Ale5623-picoctf@webshell:~$ file warm
warm: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=9e46ec8729d2f2aa8ffc4b1cdc058081bddcfe67, for GNU/Linux 3.2.0, with debug_info, not stripped
Ale5623-picoctf@webshell:~$ chmod warm
chmod: missing operand after 'warm'
Try 'chmod --help' for more information.
Ale5623-picoctf@webshell:~$ chmod +xwarm
chmod: missing operand after '+xwarm'
Try 'chmod --help' for more information.
Ale5623-picoctf@webshell:~$ chmod +x warm
Ale5623-picoctf@webshell:~$ ./warm
Hello user! Pass me a -h to learn what I can do!
Ale5623-picoctf@webshell:~$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_ac5832c}
```

./ y el nombre del ejecutable -h lo ejecuta y pide ayuda 
