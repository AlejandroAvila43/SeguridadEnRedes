#  plumbing
### Descripcion
A veces necesitas gestionar datos de procesos fuera de un archivo. ¿Puedes encontrar alguna forma de conservar la salida de este programa y buscar la bandera?Conéctate al fickle-tempest.picoctf.net 54767.

### Solucion 
```
Ale5623-picoctf@webshell:~$ nc fickle-tempest.picoctf.net 54767 | grep pico
picoCTF{digital_plumb3r_1eBfC512}

```
### NOTAS
- el > refirige la salida de comando
- el " | " 
