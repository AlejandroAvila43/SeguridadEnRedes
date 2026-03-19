- Webnet1
- #### Description

We found this [packet capture](https://challenge-files.picoctf.net/c_fickle_tempest/d1e9add4e31989553f239ebf71ba5972f9bed7bd4932f931e14bfba80d75f815/capture.pcap) and [key](https://challenge-files.picoctf.net/c_fickle_tempest/d1e9add4e31989553f239ebf71ba5972f9bed7bd4932f931e14bfba80d75f815/picopico.key). Recover the flag.

```
(aleja㉿Laptop)-[/mnt/c/Users/aleja/WebNet1]
└─$ strings vulture.jpg | gerp pico
Command 'gerp' not found, did you mean:
  command 'grep' from deb grep
Try: sudo apt install <deb name>

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/WebNet1]
└─$ strings vulture.jpg | grep pico
picoCTF{honey.roasted.peanuts}

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/WebNet1]
└─$
```