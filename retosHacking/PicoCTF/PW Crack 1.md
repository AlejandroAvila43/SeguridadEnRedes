### PW Crack 1
#### Descripción

¿Puedes descifrar la contraseña para conseguir la bandera?Descarga el comprobador [de contraseñas aquí](https://artifacts.picoctf.net/c/12/level1.py) y podrás Necesito la [bandera](https://artifacts.picoctf.net/c/12/level1.flag.txt.enc) cifrada en la misma también directorio
## Solucion 

```
def level_1_pw_check():
    user_pw = input("Please enter correct password for flag: ")
    if( user_pw == "8713"):
        print("Welcome back... your flag, user:")
        decryption = str_xor(flag_enc.decode(), user_pw)
        print(decryption)
        return
    print("That password is incorrect")



level_1_pw_check()
Ale5623-picoctf@webshell:~$ cat level1.flag.txt.enc 
[gE]__TgS^S

           JAle5623-picoctf@webshell:~$ python level1.py 
Please enter correct password for flag: [gE]__TgS^S
That password is incorrect
Ale5623-picoctf@webshell:~$ nano level1.
Ale5623-picoctf@webshell:~$ nano level1.py
Ale5623-picoctf@webshell:~$ python level1.py 
Please enter correct password for flag: 8713
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_1b2fd683}
Ale5623-picoctf@webshell:~$ 
```