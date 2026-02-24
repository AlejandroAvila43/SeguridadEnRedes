#### Descripción

¿Cómo automatizar tareas para ejecutarse a intervalos en servidores Linux?Usa ssh para conectarte a este servidor:

```
Server: saturn.picoctf.net
Port: 59832
Username: picoplayer 
Password: kZx-HVJKu8
```


## Solucion 
```
Ale5623-picoctf@webshell:~$ ssh -p 59832 picoplayer@saturn.picoctf.net
The authenticity of host '[saturn.picoctf.net]:59832 ([13.59.203.175]:59832)' can't be established.
ED25519 key fingerprint is SHA256:dMTscRrUiURy7uMu5eGWwEKdd2FzqLzx6LfWhssWnNQ.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[saturn.picoctf.net]:59832' (ED25519) to the list of known hosts.
picoplayer@saturn.picoctf.net's password: 
Welcome to Ubuntu 20.04.5 LTS (GNU/Linux 6.8.0-1044-aws x86_64)

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

picoplayer@challenge:~$ crontab -l
no crontab for picoplayer
picoplayer@challenge:~$ cat /etc/crontab
# picoCTF{Sch3DUL7NG_T45K3_L1NUX_5b7059d0}
```

### Notas 
# Ver usuario actual

`whoami`

# Ver cron del usuario

`crontab -l`
Sirve para:  
Mostrar las tareas programadas del usuario actual.
# Ver cron del sistema

`cat /etc/crontab`
Mostrar las tareas programadas a nivel sistema (muchas veces ejecutadas por root).
# Ver directorios de cron

`ls -la /etc/cron.d`
Sirve para:  
Listar scripts que se ejecutan automaticamente cada cierto tiempo.