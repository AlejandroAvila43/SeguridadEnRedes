## Descripción

  

Have you heard of Rust? Fix the syntax errors in this Rust file to print the flag!Download the Rust code [here](https://challenge-files.picoctf.net/c_verbal_sleep/3f0e13f541928f420d9c8c96b06d4dbf7b2fa18b15adbd457108e8c80a1f5883/fixme1.tar.gz).

## Solución

```
 cargo run
   Compiling rust_proj v0.1.0 (/mnt/c/Users/aleja/forensic/examen/fixme1)
error: expected `;`, found keyword `let`
 --> src/main.rs:5:37
  |
5 |     let key = String::from("CSUCKS") // How do we end statements in R...
  |                                     ^ help: add `;` here
...
8 |     let hex_values = ["41", "30", "20", "63", "4a", "45", "54", "76",...
  |     --- unexpected token

error: argument never used
  --> src/main.rs:26:9
   |
25 |         ":?", // How do we print out a variable in the println funct...
   |         ---- formatting specifier missing
26 |         String::from_utf8_lossy(&decrypted_buffer)
   |         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ argument never used
   |
help: format specifiers use curly braces, consider adding a format specifier
   |
25 |         ":?{}", // How do we print out a variable in the println function?
   |            ++

error[E0425]: cannot find value `ret` in this scope
  --> src/main.rs:18:9
   |
18 |         ret; // How do we return in rust?
   |         ^^^ help: a local variable with a similar name exists: `res`

For more information about this error, try `rustc --explain E0425`.
error: could not compile `rust_proj` (bin "rust_proj") due to 3 previous errors

┌──(aleja㉿Laptop)-[/mnt/c/Users/aleja/forensic/examen/fixme1/src]
└─$ ─$ cargo run
   Compiling rust_proj v0.1.0 (/home/flavio/picoCTF/Examen1/fixme1)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.97s
     Running `target/debug/rust_proj`
"picoCTF{4r3_y0u_4_ru$t4c30n_
```