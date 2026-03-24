- Operation Oni
-Nota: debes iniciar una instancia de desafío para poder ver el enlace de descarga de tu imagen de disco.

#### Fecha límite en: **15 horas y 6 minutos**

##### Asignación: Forense 4 ([EJ26 - IS - Seguridad en Redes y Sistemas de Software](https://play.picoctf.org/classrooms))

#### Descripción

Descarga esta imagen de disco, encuentra la clave y inicia sesión en la máquina remota.Nota: si usas el webshell, descarga y extrae la imagen de disco que no sea tu directorio principal.`/tmp`

Habrá más detalles disponibles tras lanzar tu instancia de desafío.
### solucion 
```
─$ ssh -i id_rsa -p 51406 ctf-player@saturn.picoctf.net
** WARNING: connection is not using a post-quantum key exchange algorithm.
** This session may be vulnerable to "store now, decrypt later" attacks.
** The server may need to be upgraded. See https://openssh.com/pq.html
Welcome to Ubuntu 20.04.5 LTS (GNU/Linux 6.8.0-1047-aws x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

This system has been minimized by removing packages and content that are
not required on a system that users do not log into.

To restore this content, you can run the 'unminimize' command.

The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

ctf-player@challenge:~$ ls
flag.txt
ctf-player@challenge:~$ cat flag.txt
picoCTF{k3y_5l3u7h_339601ed}ctf-player@challenge:~$
```