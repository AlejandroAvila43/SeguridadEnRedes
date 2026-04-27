#### Descripción

Una empresa almacenó un mensaje secreto en un servidor que fue vulnerado porque el administrador usó contraseñas mal hashadas. ¿Se puede acceder al secreto almacenado en el servidor?

Habrá más detalles disponibles tras lanzar tu instancia de desafío.
### Solucion 
```
 nc verbal-sleep.picoctf.net 54851
Welcome!! Looking For the Secret?

We have identified a hash: 482c811da5d5b4bc6d497ffa98491e38
Enter the password for identified hash: password123
Correct! You've cracked the MD5 hash with no secret found!

Flag is yet to be revealed!! Crack this hash: b7a875fc1ea228b9061041b7cec4bd3c52ab3ce3
Enter the password for the identified hash: letmein
Correct! You've cracked the SHA-1 hash with no secret found!

Almost there!! Crack this hash: 916e8c4f79b25028c9e467f1eb8eee6d6bbdff965f9928310ad30a8d88697745
Enter the password for the identified hash: qwerty098
Correct! You've cracked the SHA-256 hash with a secret found.
The flag is: picoCTF{UseStr0nG_h@shEs_&PaSswDs!_5b836723}

```