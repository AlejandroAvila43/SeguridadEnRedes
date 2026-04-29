#### Description

In the last challenge, you mastered octal (base 8), decimal (base 10), and hexadecimal (base 16) numbers, but this vault door uses a different change of base as well as URL encoding!The source code for this vault is here: [VaultDoor5.java](https://challenge-files.picoctf.net/c_fickle_tempest/676c61b70bd76ad210af911bd9cc981a14c6dd2c81ad6f8c79e7de9688b6564b/VaultDoor5.java)
### Solucion 
## Qué hace el programa

Tu password pasa por:

`password → URL encode → Base64 → comparar con "expected"`

Entonces tú debes hacer lo contrario:

`expected → Base64 decode → URL decode → password real`

---

## 🧠 Paso 1: Base64 decode

El `expected` es:

`JTYzJTMwJTZlJTc2JTMzJTcyJTc0JTMxJTZlJTY3JTVmJTY2JTcyJTMwJTZkJTVmJTYyJTYxJTM1JTY1JTVmJTM2JTM0JTVmJTY0JTMxJTM5JTM0JTM4JTY0JTM0JTY1`

Al decodificar Base64 obtienes algo así:

`%63%30%6e%76%33%72%74%31%6e%67%5f%66%72%30%6d%5f%62%61%35%65%5f%36%34%5f%64%31%39%34%38%64%34%65`

---

## 🧠 Paso 2: URL decode

Cada cosa tipo `%63` es hexadecimal ASCII:

Ejemplo:

`%63 → c %30 → 0 %6e → n`

Al decodificar todo:

`c0nv3rt1ng_fr0m_ba5e_64_d1948d4e`

---

## ✅ PASSWORD FINAL

`c0nv3rt1ng_fr0m_ba5e_64_d1948d4e`

---

## 🏁 FLAG

`picoCTF{c0nv3rt1ng_fr0m_ba5e_64_d1948d4e}`