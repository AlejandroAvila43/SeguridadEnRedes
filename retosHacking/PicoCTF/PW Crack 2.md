### PW Crack 2
#### Descripción

¿Puedes descifrar la contraseña para conseguir la bandera?Download the password checker [here](https://artifacts.picoctf.net/c/13/level2.py) and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/13/level2.flag.txt.enc) in the same directory too.
```
Ale5623-picoctf@webshell:~$ python level2.py 
Traceback (most recent call last):
  File "/home/Ale5623-picoctf/level2.py", line 28, in <module>
    level_2_pw_check()
  File "/home/Ale5623-picoctf/level2.py", line 17, in level_2_pw_check
    print(user_pw == chr(0x64) + chr(0x65) + chr(0x37) + chr(0x36))
UnboundLocalError: local variable 'user_pw' referenced before assignment
Ale5623-picoctf@webshell:~$ nano level2.py
Ale5623-picoctf@webshell:~$ python level2.py 
Please enter correct password for flag: de76
Welcome back... your flag, user:
picoCTF{tr45h_51ng1ng_489dea9a}
Ale5623-picoctf@webshell:~$ ^C
Ale5623-picoctf@webshell:~$ 
Webshell session has ended.

```