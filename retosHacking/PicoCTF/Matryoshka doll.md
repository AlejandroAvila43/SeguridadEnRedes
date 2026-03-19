- Matryoshka doll
#### Descripción

Las muñecas matrioska son un conjunto de muñecas de madera de tamaño decreciente colocadas unas dentro de otras. ¿Cuál es el último?Imagen: [dolls.jpg](https://challenge-files.picoctf.net/c_wily_courier/b236ead0cb75e5a4b8b8d5aa15c6cc80369b3ea778f1a116911f23d774a92bf4/dolls.jpg)

## Solucion 
```
unzip  base_images/3_c.jpg
Archive:  base_images/3_c.jpg
warning [base_images/3_c.jpg]:  123606 extra bytes at beginning or within zipfile
  (attempting to process anyway)
  inflating: base_images/4_c.jpg

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/Matryoshka]
└─$ unzip  base_images/4_c.jpg
Archive:  base_images/4_c.jpg
warning [base_images/4_c.jpg]:  79578 extra bytes at beginning or within zipfile
  (attempting to process anyway)
 extracting: flag.txt

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/Matryoshka]
└─$ cat flag.txt | grep pico
picoCTF{LL9lb1dR4QbGe4l4iWCvGq9pdtwt7392}
```