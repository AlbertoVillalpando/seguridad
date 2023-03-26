## Descripción
This is a really weird text file [TXT](https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt)? Can you find the flag?

## Solución
Cambiar la extensión del archivo a .png.

```bash
┌──(alberto㉿Nova)-[/media/sf_notas-hacking/picoCTF/foresinc/extensions]
└─$ xxd -l 32 flag.txt 
00000000: 8950 4e47 0d0a 1a0a 0000 000d 4948 4452  .PNG........IHDR
00000010: 0000 06a1 0000 0260 0802 0000 0085 ad5e  .......`.......^
                                                                                                                                                                                                                                     
┌──(alberto㉿Nova)-[/media/sf_notas-hacking/picoCTF/foresinc/extensions]
└─$ hexeditor flag.txt 
                                                                                                                                                                                                                                     
┌──(alberto㉿Nova)-[/media/sf_notas-hacking/picoCTF/foresinc/extensions]
└─$ mv flag.txt flag.png
                                                                                                                                                                                                                                     
┌──(alberto㉿Nova)-[/media/sf_notas-hacking/picoCTF/foresinc/extensions]
└─$ open flag.png 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
