## Descripción

  

The Multiverse is within your grasp! Unfortunately, the server that contains the secrets of the multiverse is in a universe where keyboards only have numbers and (most) symbols. `ssh -p 55092 ctf-player@mimas.picoctf.net` Use password: `1db87a14`

## Solución
```
(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/examen]
└─$ echo cmV0dXJuIDAgcGljb0NURns3aDE1X211MTcxdjNyNTNfMTVfbTRkbjM1NV80OTQ1NjMwYX0= | base64 -d
return 0 picoCTF{7h15_mu171v3r53_15_m4dn355_4945630a}
```