#### Descripción

¿Qué tal un poco de escondite, jeje?Mira esta [imagen aquí](https://artifacts.picoctf.net/c/241/atbash.jpg).

```
(aleja㉿Laptop)-[/mnt/c/Users/aleja/Pixelado]
└─$ steghide info atbash.jpg
"atbash.jpg":
  format: jpeg
  capacity: 2.4 KB
Try to get information about embedded data ? (y/n) y
Enter passphrase:
steghide: could not extract any data with that passphrase!

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/Pixelado]
└─$ steghide info atbash.jpg
"atbash.jpg":
  format: jpeg
  capacity: 2.4 KB
Try to get information about embedded data ? (y/n) y
Enter passphrase:
  embedded file "encrypted.txt":
    size: 31.0 Byte
    encrypted: rijndael-128, cbc
    compressed: yes
picoCTF{atbash_crack_7142fde9}


```