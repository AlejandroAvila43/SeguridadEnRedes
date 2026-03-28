## Descripción

  

Reception of Special has been cool to say the least. That's why we made an exclusive version of Special, called Secure Comprehensive Interface for Affecting Linux Empirically Rad, or just 'Specialer'. With Specialer, we really tried to remove the distractions from using a shell. Yes, we took out spell checker because of everybody's complaining. But we think you will be excited about our new, reduced feature set for keeping you focused on what needs it the most. Please start an instance to test your very own copy of Specialer. `ssh -p 55505 ctf-player@saturn.picoctf.net`. The password is `3f39b042`

## Solución

```
ssh -p 65205 ctf-player@saturn.picoctf.net
The authenticity of host '[saturn.picoctf.net]:65205 ([13.59.203.175]:65205)' can't be established.
ED25519 key fingerprint is: SHA256:lMXKIC17ONzyUJx7ZYBY5VSwoxCz20uq5/Nm+IhXKew
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[saturn.picoctf.net]:65205' (ED25519) to the list of known hosts.
** WARNING: connection is not using a post-quantum key exchange algorithm.
** This session may be vulnerable to "store now, decrypt later" attacks.
** The server may need to be upgraded. See https://openssh.com/pq.html
ctf-player@saturn.picoctf.net's password:
Specialer$  echo "$(<ala/kazam.txt)"
return 0 picoCTF{y0u_d0n7_4ppr3c1473_wh47_w3r3_d01ng_h3r3_811ae7e9}
Specialer$
```
