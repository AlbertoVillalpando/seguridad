## Descripción

Our flag printing service has started glitching! `$ nc saturn.picoctf.net 53933`

## Solución


```bash
alberto@Nova:~/Descargas$ nc saturn.picoctf.net 53933
'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'
^C
alberto@Nova:~/Descargas$ touch glitch_flag.py
alberto@Nova:~/Descargas$ nano glitch_flag.py 
alberto@Nova:~/Descargas$ cat glitch_flag.py 
print('picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'
)
alberto@Nova:~/Descargas$ python3 glitch_flag.py 
picoCTF{gl17ch_m3_n07_a4392d2e}
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
