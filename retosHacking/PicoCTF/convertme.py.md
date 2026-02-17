### convertme.py
#### Descripción

Ejecuta el script en Python y convierte el número dado de decimal a binario a Coge la bandera.[Descargar script en Python](https://artifacts.picoctf.net/c/24/convertme.py)
## solucion 
```
Ale5623-picoctf@webshell:~$ python convertme.py 
If 12 is in decimal base, what is it in binary base?
Answer: ^CTraceback (most recent call last):
  File "/home/Ale5623-picoctf/convertme.py", line 23, in <module>
    ans = input('Answer: ')
KeyboardInterrupt

Ale5623-picoctf@webshell:~$ bin12
-bash: bin12: command not found
Ale5623-picoctf@webshell:~$ bin(12)
-bash: syntax error near unexpected token `12'
Ale5623-picoctf@webshell:~$ python convertme.py 
If 60 is in decimal base, what is it in binary base?
Answer: 111100
That is correct! Here's your flag: picoCTF{4ll_y0ur_b4535_722f6b39}
```
