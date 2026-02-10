# Bases
## Descripcion
¿Qué significa este bDNhcm5fdGgzX3IwcDM1? Creo que tiene que ver con las bases.
## Solucion 1- consola


```
Ale5623-picoctf@webshell:~$ echo 'bDNhcm5fdGgzX3IwcDM1' | base64 -d
l3arn_th3_r0p35Ale5623-picoctf@webshell:~$ ^C
Ale5623-picoctf@webshell:~$ 
```
## Solucion 2- Python
```
Python 3.10.12 (main, Feb  4 2025, 14:57:36) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import base64
>>> base64.b64decode('bDNhcm5fdGgzX3IwcDM1')
b'l3arn_th3_r0p35'
>>> 
```
## Referencias

## Notas
	-base64 es un sistema de codificacion que utiliza ascii imprimibles 
	