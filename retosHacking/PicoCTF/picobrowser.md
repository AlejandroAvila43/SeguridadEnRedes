### picobrowser
#### Description

This website can be rendered only by picobrowser, go and catch the flag!http://fickle-tempest.picoctf.net:56733

```
Ale5623-picoctf@webshell:~$ curl http://fickle-tempest.picoctf.net:56733/flag -H 'User-Agent: picobrowser' | grep pico
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  2115  100  2115    0     0  30245      0 --:--:-- --:--:-- --:--:-- 30652
         <!-- <strong>Title</strong> --> picobrowser!
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{p1c0_s3cr3t_ag3nt_fba5c48f}</code></p>
Ale5623-picoctf@webshell:~$ 
```