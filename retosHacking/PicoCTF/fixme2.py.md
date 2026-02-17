### fixme2.py
#### Descripción

Corrige el error de sintaxis en el script de Python para imprimir la bandera.[Descargar script en Python](https://artifacts.picoctf.net/c/4/fixme2.py)
### solución  
```
Ale5623-picoctf@webshell:~$ python fixme2.py 
  File "/home/Ale5623-picoctf/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?
Ale5623-picoctf@webshell:~$ nano fixme
fixme1.py  fixme2.py  
Ale5623-picoctf@webshell:~$ nano fixme2.py 
Ale5623-picoctf@webshell:~$ python fixme2.py 
That is correct! Here's your flag: picoCTF{3qu4l1ty_n0t_4551gnm3nt_e8814d03}
Ale5623-picoctf@webshell:~$ 
```