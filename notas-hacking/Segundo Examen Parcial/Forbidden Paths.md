## Descripción
Can you get the flag? Here's the [website](http://saturn.picoctf.net:52278/). We know that the website files live in `/usr/share/nginx/html/` and the flag is at `/flag.txt` but the website is filtering absolute file paths. Can you get past the filter to read the flag?

## Solución
Ya que el sitio no autoriza rutas absolutas, estamos en `/usr/share/nginx/html/` y la bandera está en `/flag.txt` hay que retroceder desde nuestra posición hasta el root.

`../../../../flag.txt`

picoCTF{7h3_p47h_70_5ucc355_6db46514}

```bash
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
