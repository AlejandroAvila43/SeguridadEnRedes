
#### Description

What happens if you have a small exponent? There is a twist though, we padded the plaintext so that (M ** e) is just barely larger than N. Let's decrypt this:[values](https://challenge-files.picoctf.net/c_wily_courier/7ba940d8ab348a0caa291609a28d488c0b1f6839e7f55ae6bf5bf77aefb1bda1/values)
### Solucion 
```
(aleja㉿Laptop)-[/mnt/c/Users/aleja]
└─$ python3 minirsa.py
calculando raiz cubica

¡Raíz cúbica perfecta encontrada!
Mensaje (entero): 1787330808968142828287809319332701517353332911736848279839502759158602467824780424488141955644417387373185756944952906538004355347478978500948630620749868180414755933760446136287315896825929319145984883756667607031853695069891380871892213007874933651015534862552820965037339951640771420661677346655540782589819314418453997020813427309834
FLAG:                                                                                                        picoCTF{e_sh0u1d_b3_lArg3r_92f4d5a5}
```