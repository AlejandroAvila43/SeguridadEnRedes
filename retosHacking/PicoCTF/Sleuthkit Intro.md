- Sleuthkit Intro
- #### Descripción

Descarga la imagen de disco y úsala para encontrar el tamaño del Linux Partición. Conéctate con el servicio de verificación remota para comprobar tu respuesta y obtener La bandera.`mmls`Nota: si usas el webshell, descarga y extrae la imagen de disco que no sea tu directorio principal.`/tmp`[Descargar imagen de disco](https://artifacts.picoctf.net/c/164/disk.img.gz)

Habrá más detalles disponibles tras lanzar tu instancia de desafío.
```
mmls disk.img
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000204799   0000202752   Linux (0x83)

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/SleuthkirIntro]
└─$ nc saturn.picoctf.net 64222
What is the size of the Linux partition in the given disk image?
Length in sectors: 202752
202752
Great work!
picoCTF{mm15_f7w!}
```