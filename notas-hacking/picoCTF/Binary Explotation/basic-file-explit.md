## Descripción
The program provided allows you to write to a file and read what you wrote from it. Try playing around with it and see if you can break it! Connect to the program with netcat: $ nc saturn.picoctf.net 50959 The program's source code with the flag redacted can be downloaded here.

## Solución
Introducir una cadena de texto.

Leer la cadena introducida.

En el paso de lectura, agregar un tipo de dato no esperado por el programa.

```bash
alberto@Nova:~$ nc saturn.picoctf.net 50959
Hi, welcome to my echo chamber!
Type '1' to enter a phrase into our database
Type '2' to echo a phrase in our database
Type '3' to exit the program
1
1
Please enter your data:
hola
hola
Please enter the length of your data:
4
4
Your entry number is: 1
Write successful, would you like to do anything else?
2
2
Please enter the entry number of your data:
no
no

picoCTF{M4K3_5UR3_70_CH3CK_Y0UR_1NPU75_E0394EC0}
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
