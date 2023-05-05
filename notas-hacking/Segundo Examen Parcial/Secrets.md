## Descripción
We have several pages hidden. Can you find the one with the flag? The website is running [here](http://saturn.picoctf.net:52025/).

## Solución
Navegar a traves de las rutas encontradas en los atributos de los tags html. Crear la ruta donde se encuentra almacenada la bandera a partir de los valores encontrados.

Acceder a `/secret` encontrada en:
`<img src="secret/assets/DX1KYM.jpg" alt="https://www.alamy.com/security-safety-word-cloud-concept-image-image67649784.html" class="responsive">`

Inspeccionar la página y agregar `/hidden` a la ruta actual
`<link rel="stylesheet" href="hidden/file.css">`

Nos redireccionara a una página de login, el siguiente valor `/superhidden` se encontrara en un tag escondido.
`<input type="hidden" name="db" value="superhidden/xdfgwd.html">`

La ruta final sería: http://saturn.picoctf.net:52025/secret/hidden/superhidden/

La bandera se encuentra seleccionando el texto de la página para que resalte, ya que tiene el mismo color que el fondo, o inspeccionando el código fuente.

picoCTF{succ3ss_@h3n1c@10n_39849bcf}

```bash
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()

