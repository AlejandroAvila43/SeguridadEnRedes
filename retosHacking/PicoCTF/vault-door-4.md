#### Description

This vault uses ASCII encoding for the password.The source code for this vault is here: [VaultDoor4.java](https://challenge-files.picoctf.net/c_fickle_tempest/f587295139ec9c3d23e1299b831596c3243b0e042bec63dd21168e996c0f7c8c/VaultDoor4.java)

### solucion 
## Paso 1: Entender el arreglo

`myBytes` mezcla:

- Decimal → `106`
- → hexadecimal `0x55`
- Octal → `0142`
- Caracteres → `'9'`

Todo eso al final **son bytes ASCII**.

---

## 🧠 Paso 2: Convertir TODO a ASCII

### 🔢 Bloque de cebador (decimal)

`106 → j 85  → U 53  → 5 116 → t 95  → _ 52  → 4 95  → _ 98  → b`

👉 `jU5t_4_b`

---

### 🔢 Segundo bloque (hexágono)

`0x55 → U 0x6e → n 0x43 → C 0x68 → h 0x5f → _ 0x30 → 0 0x66 → f 0x5f → _`

👉 `UnCh_0f_`

---

### 🔢 Tercer bloque (octal)

`0142 → b 0131 → Y 0164 → t 063  → 3 0163 → s 0137 → _ 067  → 7 065  → 5`

👉 `bYt3s_75`

---

### 🔢 Cuarto bloque (chars)

`'9' '6' '0' '0' 'a' 'b' 'c' '3'`

👉 `9600abc3`

---

## ✅ Paso 3: Unir todo

`jU5t_4_b + UnCh_0f_ + bYt3s_75 + 9600abc3`

---

## 🔐 FINAL CONTRASEÑA

`jU5t_4_bUnCh_0f_bYt3s_759600abc3`