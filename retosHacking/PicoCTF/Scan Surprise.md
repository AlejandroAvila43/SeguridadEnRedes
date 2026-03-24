### Scan Surprise

#### Description

I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead?You can download the challenge files here:

- [challenge.zip](https://artifacts.picoctf.net/c_atlas/14/challenge.zip)

The same files are accessible via SSH here:`ssh -p 60511 ctf-player@atlas.picoctf.net`Using the password `84b12bae`. Accept the fingerprint with `yes`, and `ls` once connected to begin. Remember, in a shell, passwords are hidden!

### solcuion 
wget https://artifacts.picoctf.net/c_atlas/14/challenge.zip
--2026-03-23 22:21:56--  https://artifacts.picoctf.net/c_atlas/14/challenge.zip
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.161.55.64, 3.161.55.100, 3.161.55.26, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.161.55.64|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 742 [application/octet-stream]
Saving to: ‘challenge.zip’

challenge.zip             100%[===================================>]     742  --.-KB/s    in 0.002s

2026-03-23 22:21:57 (327 KB/s) - ‘challenge.zip’ saved [742/742]


┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/Redaction]
└─$ ssh -p 60511 ctf-player@atlas.picoctf.net
The authenticity of host '[atlas.picoctf.net]:60511 ([18.217.83.136]:60511)' can't be established.
ED25519 key fingerprint is: SHA256:hVmbk/OaNT4902bBr7h26wfhmBuJWi4tub8AJqoAJCM
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[atlas.picoctf.net]:60511' (ED25519) to the list of known hosts.
** WARNING: connection is not using a post-quantum key exchange algorithm.
** This session may be vulnerable to "store now, decrypt later" attacks.
** The server may need to be upgraded. See https://openssh.com/pq.html
ctf-player@atlas.picoctf.net's password:

































