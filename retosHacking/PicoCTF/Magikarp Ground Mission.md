### Magikarp Ground Mission
#### Descripción

¿Sabes cómo moverte entre directorios y leer archivos en la carcasa? Arranca el contenedor, a él y, una vez conectado, empieza a empezar.`ssh``ls`Inicia sesión con la contraseña, en el host y en el puerto.`ssh``ctf-player``8c606eb1``wily-courier.picoctf.net``53840`

## Solucion
```

ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ cat^C
ctf-player@pico-chall$ cat 1of3.flag.txt
picoCTF{xxsh_
ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ ls
2of3.flag.txt  challenge  home                      lib64  opt   run   sys  var
bin            dev        instructions-to-3of3.txt  media  proc  sbin  tmp
boot           etc        lib                       mnt    root  srv   usr
ctf-player@pico-chall$ cat 2of3.flag.txt
0ut_0f_//4t3r_
ctf-player@pico-chall$ cat ~
cat: /home/ctf-player: Is a directory
ctf-player@pico-chall$ ls
2of3.flag.txt  challenge  home                      lib64  opt   run   sys  var
bin            dev        instructions-to-3of3.txt  media  proc  sbin  tmp
boot           etc        lib                       mnt    root  srv   usr
ctf-player@pico-chall$ cat 2of3.flag.txt 
0ut_0f_//4t3r_
ctf-player@pico-chall$ cat instructions-to-3of3.txt
Lastly, ctf-player, go home... more succinctly `~`
ctf-player@pico-chall$ cat ~
cat: /home/ctf-player: Is a directory
ctf-player@pico-chall$ cd ~
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cat 3of3.flag.txt 
0b24fc4f}ctf-player@pico-chall$ 
```
