### Sleuthkit Apprentice
#### Descripción

Descarga esta imagen de disco y encuentra la bandera.Nota: si usas el webshell, descarga y extrae la imagen de disco que no sea tu directorio principal.`/tmp`

- [Descargar imagen de disco comprimida](https://artifacts.picoctf.net/c/136/disk.flag.img.gz)
## solucion 
```
 icat -o 0000360448 disk.flag.img 2371
picoCTF{by73_5urf3r_3497ae6b}

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/SleuthkirApprentice]
└─$ fls -o 0000360448 disk.flag.img -r
```