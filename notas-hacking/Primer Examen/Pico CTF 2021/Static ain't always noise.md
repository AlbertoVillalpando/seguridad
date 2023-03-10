## Descripción

Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/0f6ea599582dcce7b4f1ba94e3617baf/static)? This [BASH script](https://mercury.picoctf.net/static/0f6ea599582dcce7b4f1ba94e3617baf/ltdis.sh) might help!

## Solución

```bash
alberto@Nova:~/Descargas$ sh ltdis.sh static 
Attempting disassembly of static ...
Disassembly successful! Available at: static.ltdis.x86_64.txt
Ripping strings from binary with file offsets...
Any strings found in static have been written to static.ltdis.strings.txt with file offset
alberto@Nova:~/Descargas$ ls
ltdis.sh                                                                                         static                                                                                                              static.ltdis.strings.txt
 file                                                                                                                             static.ltdis.x86_64.txt                 
alberto@Nova:~/Descargas$ cat static.ltdis.strings.txt | grep picoCTF
   1020 picoCTF{d15a5m_t34s3r_6f8c8200}
alberto@Nova:~/Descargas$ 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
