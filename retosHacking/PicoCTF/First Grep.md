#  First Grep
## Descripcion 
¿Puedes encontrar la bandera en el archivo? Sería realmente tedioso revisarlo manualmente, algo me dice que hay una forma mejor.

## 1-Solucion Linux

```
Ale5623-picoctf@webshell:~$ cat file | grep picoCTF
grep_is_good_to_find_things_beD770f5
```
## Notas 
- el comando cat es para leer un archivo
- el " | " es para haceer 2 cosas en un mismo comando 
- grep es para buscar una palabra en una linea de codigo 
- wget es para descargar un archivo mediante al url