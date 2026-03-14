- m00nwalk
- #### Descripción

Descifra este [mensaje](https://challenge-files.picoctf.net/c_fickle_tempest/816c75fc4b45dfc4ab4c4caad4ac738a3e0cfb3825fedda2a753eb5360c477bb/message.wav) de la luna.

## Solucion 
`picoCTF{beep_boop_im_in_space}`

```
 sstv -d message.wav -o result.png
[sstv] Searching for calibration header... Found!
[sstv] Detected SSTV mode Scottie 1
^[[C[sstv] Decoding image...   [##############################################............] [sstv] Decoding image...   [##########################################################] 100%
[sstv] Drawing image data...
[sstv] ...Done!

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/m00nwalk]
└─$ ls
message.wav  result.png

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/m00nwalk]
└─$  open result.png
Command 'open' not found, did you mean:
  command 'openk' from deb offpunk
  command 'wopen' from deb gworkspace.app
  command 'pen' from deb pen
  command 'gopen' from deb gnustep-gui-runtime
Try: sudo apt install <deb name>
```