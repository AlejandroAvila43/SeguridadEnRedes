## Based 
#### Descripción

Para obtener verdaderamente 1337, debes entender diferentes codificaciones de datos, como hexadecimal o binaria. ¿Puedes conseguir la bandera de este programa para demostrar que vas camino de convertirte en 1337?

Habrá más detalles disponibles tras lanzar tu instancia de desafío.
Contacta con NC fickle-tempest.picoctf.net 51209.
### Solucion

```
Ale5623-picoctf@webshell:~$ nc fickle-tempest.picoctf.net 51209
Let us see how data is stored
submarine
Please give the 01110011 01110101 01100010 01101101 01100001 01110010 01101001 01101110 01100101 as a word.
...
you have 45 seconds.....

Input:
submanine
WRONG!

Ale5623-picoctf@webshell:~$ nc fickle-tempest.picoctf.net 51209
Let us see how data is stored
sludge
Please give the 01110011 01101100 01110101 01100100 01100111 01100101 as a word.
...
you have 45 seconds.....

Input:
sludge
Please give me the  o154 o141 o155 o160 as a word.
Input:
lamp
Please give me the 636f6d7075746572 as a word.
Input:
computer
You've beaten the challenge
Flag: picoCTF{learning_about_converting_values_aeBEA593}

```

## NOTA
pasamos de binario a ascii , luego a octal y por ultimo a hexadecimal.
