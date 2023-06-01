## Descripción
We found this [file](https://mercury.picoctf.net/static/7b2d7c26630e977197022d0af09e3aeb/tunn3l_v1s10n). Recover the flag.

## Solución
Abrimos el archivo con un hex editor, notamos que el archivo es tipo bmp por la primera línea que contiene BM.

Cambiado el formato, abrimos el archivo con ImageMagick.

A la imagen le falta resolución, corriendo el comando exitfool notamos que la resolución de anchura y tamaño son 1134x306, respectivamente.

Tenemos que cambiar estos valores en el editor hex, para esto hay que ubicar sus valores correspondientes en hexadecimal.

1134>0x46e
306>0x132

Sus valores correspondientes serían 6E 04 y 32 01. Y cambiado a su altura correspondiente sería:

850>0x352

picoCTF{qu1t3_a_v13w_2020}

```bash
ubucar
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()