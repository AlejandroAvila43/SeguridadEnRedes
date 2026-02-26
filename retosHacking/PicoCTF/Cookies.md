### Cookies
#### Description

Who doesn't love cookies? Try to figure out the best one.http://wily-courier.picoctf.net:53488/

## Solucion 

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja]
└─$ for i in {1..30}; do curl -s http://wily-courier.picoctf.net:53488/check -H "Co
okie: name= $i"; done | grep pico
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{3v3ry1_l0v3s_c00k135_a4dadb49}


