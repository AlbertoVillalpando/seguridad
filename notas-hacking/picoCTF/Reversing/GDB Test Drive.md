## Descripción
Can you get the flag? Download this [binary](https://artifacts.picoctf.net/c/87/gdbme). Here's the test drive instructions:

-   `$ chmod +x gdbme`
-   `$ gdb gdbme`
-   `(gdb) layout asm`
-   `(gdb) break *(main+99)`
-   `(gdb) run`
-   `(gdb) jump *(main+104)`

## Solución
Ejecutar los comandos proporcionados en la descripción.

```bash
(gdb) break *(main+99)
Punto de interrupción 1 at 0x132a
(gdb) run
Starting program: /home/alberto/Descargas/gdbme

Breakpoint 1, 0x000055555555532a in main ()
(gdb) jump *(main+104)
Continuando a 0x55555555532f.
picoCTF{d3bugg3r_dr1v3_7776d758}
(gdb) ior 1 (process 44156) exited normally]
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
