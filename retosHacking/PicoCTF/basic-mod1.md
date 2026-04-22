#### Description

We found this weird message being passed around on the servers, we think we have a working decryption scheme.Download the message [here](https://artifacts.picoctf.net/c/129/message.txt).Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore.Wrap your decrypted message in the picoCTF flag format (i.e. `picoCTF{decrypted_message}`)

### solucion
```
python arch1.py
['350', '63', '353', '198', '114', '369', '346', '184', '202', '322', '94', '235', '114', '110', '185', '188', '225', '212', '366', '374', '261', '213']
350   - 17    - R
63    - 26    - 0
353   - 20    - U
198   - 13    - N
114   - 3     - D
369   - 36    - _
346   - 13    - N
184   - 36    - _
202   - 17    - R
322   - 26    - 0
94    - 20    - U
235   - 13    - N
114   - 3     - D
110   - 36    - _
185   - 0     - A
188   - 3     - D
225   - 3     - D
212   - 27    - 1
366   - 33    - 7
374   - 4     - E
261   - 2     - C
213   - 28    - 2

R0UND_N_R0UND_ADD17EC2

```