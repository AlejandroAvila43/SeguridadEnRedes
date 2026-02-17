### runme.py
Ejecuta el script para obtener la bandera. Descarga el guion con tu Navegador o con el webshell.`runme.py``wget`[Descargar runme.py script en Python](https://artifacts.picoctf.net/c/34/runme.py)

#### Descripción

Ejecuta el script para obtener la bandera. Descarga el guion con tu Navegador o con el webshell.`runme.py``wget`[Descargar runme.py script en Python](https://artifacts.picoctf.net/c/34/runme.py)

## solucion 
```
Ale5623-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/34/runme.py
--2026-02-16 13:58:51--  https://artifacts.picoctf.net/c/34/runme.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.128, 3.160.22.43, 3.160.22.16, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.128|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 270 [application/octet-stream]
Saving to: 'runme.py'

runme.py                     100%[============================================>]     270  --.-KB/s    in 0s      

2026-02-16 13:58:52 (11.3 MB/s) - 'runme.py' saved [270/270]

Ale5623-picoctf@webshell:~$ ls  
Addadshashanammu      README.txt     big-zip-files.zip  files      runme.py
Addadshashanammu.zip  big-zip-files  enc_flag           files.zip
Ale5623-picoctf@webshell:~$ file 
.bash_history         .ltdis.x86_64.txt     Addadshashanammu/     big-zip-files/        files/
.bash_logout          .profile              Addadshashanammu.zip  big-zip-files.zip     files.zip
.bashrc               .ssh/                 README.txt            enc_flag              runme.py
Ale5623-picoctf@webshell:~$ file runme.py 
runme.py: Python script, ASCII text executable
Ale5623-picoctf@webshell:~$ python runme.py 
picoCTF{run_s4n1ty_run}
```


## Nota
 se usa el comando python y el nombre del archivo para ejecutarlo 
 file es para ver que tipo de archivo es si es ejecutable o no.