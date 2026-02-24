#### Description

Can you break into this super secure portal?

Additional details will be available after launching your challenge instance.

---


### solucion 
```
### Condiciones que debe cumplir el password

1. `substring(0, 8) == "picoCTF{"`
    
2. `substring(3, 6) == "oCT"`
    
3. `substring(6, 11) == "F{not"`
    
4. `substring(7, 9) == "{n"`
    
5. `substring(8, 16) == "not_this"`
    
6. `substring(16, 24) == "_again_4"`
    
7. `substring(12, 16) == "this"`
    
8. La parte final contiene `"daf93}"`
   picoCTF{not_this_again_4daf93}
```