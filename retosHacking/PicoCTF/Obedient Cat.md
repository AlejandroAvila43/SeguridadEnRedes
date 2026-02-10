#  Obedient Cat
### Descripcion
Este archivo tiene una bandera a la vista (también llamada "in-the-clear").[Bandera](https://challenge-files.picoctf.net/c_wily_courier/05592bf6e83870a5d06ac3cf744a0cbb841e24a4c14fa67a9766c60d88419fd2/flag)

### Solucion
```
Ale5623-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_wily_courier/05592bf6e83870a5d06ac3cf744a0cbb841e24a4c14fa67a9766c60d88419fd2/flag
--2026-02-09 14:31:39--  https://challenge-files.picoctf.net/c_wily_courier/05592bf6e83870a5d06ac3cf744a0cbb841e24a4c14fa67a9766c60d88419fd2/flag
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.160.5.40, 3.160.5.64, 3.160.5.95, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.160.5.40|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 34 [application/octet-stream]
Saving to: 'flag'

flag                  100%[=======================>]      34  --.-KB/s    in 0s      

2026-02-09 14:31:39 (11.7 MB/s) - 'flag' saved [34/34]

Ale5623-picoctf@webshell:~$ cat flag
picoCTF{s4n1ty_v3r1f13d_9b8fa0bc}
Ale5623-picoctf@webshell:~$ 
```
