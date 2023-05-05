## Descripción
Can you find the flag? [shark1.pcapng](https://mercury.picoctf.net/static/81c7862241faf4a48bd64a858392c92b/shark1.pcapng).

## Solución
Abrir el archivo, seguir el protocolo TCP, buscar en la frecuencia 5, a la cadena encontrada aplicarle rot13.

cvpbPGS{c33xno00_1_f33_h_qrnqorrs} -> picoCTF{p33kab00_1_s33_u_deadbeef}

```bash
┌──(alberto㉿Nova)-[~]
└─$ echo cvpbPGS{c33xno00_1_f33_h_qrnqorrs} | rot13
picoCTF{p33kab00_1_s33_u_deadbeef}

┌──(alberto㉿Nova)-[~]
└─$ 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()

