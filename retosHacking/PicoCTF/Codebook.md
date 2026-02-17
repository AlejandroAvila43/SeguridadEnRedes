### Codebook
#### Descripción

Ejecuta el script de Python en el mismo directorio que .`code.py``codebook.txt`

- [Descargar code.py](https://artifacts.picoctf.net/c/1/code.py)
- [Descargar codebook.txt](https://artifacts.picoctf.net/c/1/codebook.txt)
### solucion 
```
Ale5623-picoctf@webshell:~$ wget -q  https://artifacts.picoctf.net/c/1/codebook.txt
Ale5623-picoctf@webshell:~$ ls
Addadshashanammu  README.txt  big-zip-files  code.py  codebook.txt  files
Ale5623-picoctf@webshell:~$ file *
Addadshashanammu: directory
README.txt:       ASCII text, with escape sequences
big-zip-files:    directory
code.py:          Python script, ASCII text executable, with very long lines (404)
codebook.txt:     ASCII text
files:            directory
Ale5623-picoctf@webshell:~$ cat code
code.py       codebook.txt  
Ale5623-picoctf@webshell:~$ cat codebook.txt
azbycxdwevfugthsirjqkplomn
Ale5623-picoctf@webshell:~$ nano codebook.txt 
Ale5623-picoctf@webshell:~$ nano code.py      
Ale5623-picoctf@webshell:~$ python code.py 
picoCTF{c0d3b00k_455157_d9aa2df2}
```
