
### Super SSH
#### Descripción

Usar un Secure Shell (SSH) va a ser bastante importante.¿Puedes ir al puerto para conseguir la bandera?`ssh``ctf-player``titan.picoctf.net``54500`También necesitarás la contraseña. Si se le pide, acepta la huella con .`84b12bae``yes`Si tu dispositivo no tiene carcasa, puedes usar: [https://webshell.picoctf.org](https://webshell.picoctf.org/)Si no tienes claro qué es una carcasa, echa un vistazo a nuestro primer de manual: [https://primer.picoctf.com/#_the_shell](https://primer.picoctf.com/#_the_shell)

### solucion

```
Ale5623-picoctf@webshell:~$ ssh ctf-player@titan.picoctf.net -p63216 
The authenticity of host '[titan.picoctf.net]:63216 ([3.139.174.234]:63216)' can't be established.
ED25519 key fingerprint is SHA256:4S9EbTSSRZm32I+cdM5TyzthpQryv5kudRP9PIKT7XQ.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[titan.picoctf.net]:63216' (ED25519) to the list of known hosts.
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_07a987ac}
Connection to titan.picoctf.net closed.
Ale5623-picoctf@webshell:~$ 
```