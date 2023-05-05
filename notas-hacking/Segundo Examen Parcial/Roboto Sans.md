## Descripción
The flag is somewhere on this web application not necessarily on the website. Find it. Check [this](http://saturn.picoctf.net:64271/) out.

## Solución
Acceder a la ruta /robots.txt, aplicar base64 al texto `"anMvbXlmaWxlLnR4dA==`, nos regresará una ruta `js/myfile.txt`, agregamos esta ruta en el navegador y encontraremos la bandera.

picoCTF{Who_D03sN7_L1k5_90B0T5_032f1c2b}

```bash
alberto@Nova:~$ echo anMvbXlmaWxlLnR4dA== | base64 -d
js/myfile.txt
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
