##  strings it
#### Descripción

¿Puedes encontrar la bandera en [el archivo](https://challenge-files.picoctf.net/c_fickle_tempest/094a1db42d5ae681cd9e513dcbea2d997495dd3763d50c643b939923ca86e29b/strings) sin ejecutarla?

### solucion 
```
Ale5623-picoctf@webshell:~$ chmod +x strings
Ale5623-picoctf@webshell:~$ ./strings 
Maybe try the 'strings' function? Take a look at the man page
Ale5623-picoctf@webshell:~$ strings strings | grep pico
picoCTF{5tRIng5_1T_47948C73}
Ale5623-picoctf@webshell:~$ 
```
chmod +x  es para otorgar permisos de un archivo
