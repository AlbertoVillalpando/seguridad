## Descripción
We found this packet capture and key. Recover the flag.

## Solución
Para poder ver la información encriptada agregamos un protocolo tls con la key proporcionada con ip 0.0.0.0, puerto 443 y protocolo http.

Exportamos los objetos http

Exploramos el .jpg con srtings

```bash
┌──(alberto㉿Nova)-[~/Descargas]
└─$ strings vulture.jpg | grep pico
picoCTF{honey.roasted.peanuts}
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()