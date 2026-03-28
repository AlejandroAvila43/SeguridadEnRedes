## Descripción

  

Connect to this PostgreSQL server and find the flag! `psql -h saturn.picoctf.net -p 55452 -U postgres pico` Password is `postgres`

## Solución
```
┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/bookshelf/bookshelf]
└─$ psql -h saturn.picoctf.net -p 61547 -U postgres pico
Password for user postgres:
psql (18.3 (Debian 18.3-1+b1), server 15.2 (Debian 15.2-1.pgdg110+1))
Type "help" for help.

pico=# SELECT * FROM flags;
 id | firstname | lastname  |                address
----+-----------+-----------+----------------------------------------
  1 | Luke      | Skywalker | picoCTF{L3arN_S0m3_5qL_t0d4Y_21c94904}
  2 | Leia      | Organa    | Alderaan
  3 | Han       | Solo      | Corellia
(3 rows)

pico=#
```