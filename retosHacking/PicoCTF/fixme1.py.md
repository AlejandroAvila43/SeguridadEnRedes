### fixme1.py

#### Descripción

Correge el error de sintaxis en este script de Python para imprimir la bandera.[Descargar script en Python](https://artifacts.picoctf.net/c/27/fixme1.py)[[]]


### solucion 
```
Ale5623-picoctf@webshell:~$ wget -q https://artifacts.picoctf.net/c/27/fixme1.py
Ale5623-picoctf@webshell:~$ python fixme1.py 
  File "/home/Ale5623-picoctf/fixme1.py", line 20
    print('That is correct! Here\'s your flag: ' + flag)
IndentationError: unexpected indent
Ale5623-picoctf@webshell:~$ nano fixme1.py 
Ale5623-picoctf@webshell:~$ python fixme1.py 
That is correct! Here's your flag: picoCTF{1nd3nt1ty_cr1515_182342f7}
Ale5623-picoctf@webshell:~$ 
```

## NOTA 
cuando las pistas nos dicen que corrigamos el error hay que ejecutarlo y ver que error nos dice el smd y corregir el error 
