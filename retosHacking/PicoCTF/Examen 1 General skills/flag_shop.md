## Descripción

  

There's a flag shop selling stuff, can you buy a flag? [Source](https://challenge-files.picoctf.net/c_fickle_tempest/a688b629e6044019fb08e6323c70c4604d60853d771e5ae1137f90b0f1039056/store.c).

Connect with nc fickle-tempest.picoctf.net 65297.

## Solución
```

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/examen]
└─$ nc fickle-tempest.picoctf.net 54851.
Welcome to the flag exchange
We sell flags

1. Check Account Balance

2. Buy Flags

3. Exit

 Enter a menu selection
1



 Balance: 1100


Welcome to the flag exchange
We sell flags

1. Check Account Balance

2. Buy Flags

3. Exit

 Enter a menu selection
2
Currently for sale
1. Defintely not the flag Flag
2. 1337 Flag
40000000
Welcome to the flag exchange
We sell flags

3. Check Account Balance

4. Buy Flags

5. Exit

 Enter a menu selection
2
Currently for sale
1. Defintely not the flag Flag
2. 1337 Flag
1
These knockoff Flags cost 900 each, enter desired quantity
4000000

The final cost is: -694967296

Your current balance after transaction: 694968396

Welcome to the flag exchange
We sell flags

1. Check Account Balance

2. Buy Flags

3. Exit

 Enter a menu selection
2
Currently for sale
1. Defintely not the flag Flag
2. 1337 Flag
2
1337 flags cost 100000 dollars, and we only have 1 in stock
Enter 1 to buy one
1
YOUR FLAG IS: picoCTF{m0n3y_bag5_39AF2bE1}

Welcome to the flag exchange
We sell flags

```