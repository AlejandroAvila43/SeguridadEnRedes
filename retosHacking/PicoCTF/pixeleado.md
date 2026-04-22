#### Descripción

Tengo estas dos imágenes, ¿puedes hacer una bandera con ellas?[scrambled1.png](https://challenge-files.picoctf.net/c_wily_courier/3dced65f7a857f7a28f538da0f98fdceca989646f69d4651133b5c04590b0b0d/scrambled1.png) [scrambled2.png](https://challenge-files.picoctf.net/c_wily_courier/3dced65f7a857f7a28f538da0f98fdceca989646f69d4651133b5c04590b0b0d/scrambled2.png)
## solucion
```
 wget https://challenge-files.picoctf.net/c_wily_courier/3dced65f7a857f7a28f538da0f98fdceca989646f69d4651133b5c04590b0b0d/scrambled2.png
--2026-04-22 08:02:11--  https://challenge-files.picoctf.net/c_wily_courier/3dced65f7a857f7a28f538da0f98fdceca989646f69d4651133b5c04590b0b0d/scrambled2.png
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 18.238.132.49, 18.238.132.26, 18.238.132.88, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|18.238.132.49|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 197173 (193K) [application/octet-stream]
Saving to: ‘scrambled2.png’

scrambled2.png                100%[=================================================>] 192.55K   742KB/s    in 0.3s

2026-04-22 08:02:12 (742 KB/s) - ‘scrambled2.png’ saved [197173/197173]


┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/Pixelado]
└─$ sudo chmod +x stegsolve.jar
[sudo] password for aleja:
sudo: a password is required

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/Pixelado]
└─$ java -jar /opt/stegsolve.jar

picoCTF{8cdf93c3}
```