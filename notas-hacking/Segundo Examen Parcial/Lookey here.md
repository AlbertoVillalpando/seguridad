## Descripción
Attackers have hidden information in a very large mass of data in the past, maybe they are still doing it. Download the data [here](https://artifacts.picoctf.net/c/124/anthem.flag.txt).

## Solución
Buscar la bandera con el comando grep y guardarlo en un archivo.

```bash
alberto@Nova:~/Descargas$ grep -oE 'picoCTF{.*?}' anthem.flag.txt > flag.txt
alberto@Nova:~/Descargas$ cat flag.txt
picoCTF{gr3p_15_@w3s0m3_4c479940}
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
