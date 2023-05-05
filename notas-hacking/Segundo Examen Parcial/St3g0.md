## Descripción
Download this image and find the flag.

-   [Download image](https://artifacts.picoctf.net/c/215/pico.flag.png)

## Solución
En este reto se aplica la estenografía, que es básicamente una manera de esconder un mensaje dentro de otro.

Con la herramienta zsteg podemos encontrar la bandera que esconde.

```bash
┌──(alberto㉿Nova)-[~/Descargas]
└─$ zsteg --lsb pico.flag.png | grep -oE "picoCTF{.*?}"
picoCTF{7h3r3_15_n0_5p00n_96ae0ac1}
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- [Steganography](https://en.wikipedia.org/wiki/Steganography)
