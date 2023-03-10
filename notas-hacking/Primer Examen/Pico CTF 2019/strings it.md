## Descripción

Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/5bd86036f013ac3b9c958499adf3e2e2/strings) without running it?

## Solución

```bash
alberto@Nova:~/Descargas$ strings strings | grep picoCTF
picoCTF{5tRIng5_1T_827aee91}
alberto@Nova:~/Descargas$ 
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|strings|For each _file_ given, GNU **strings** prints the printable character sequences that are at least 4 characters long (or the number given with the options below) and are followed by an unprintable character. By default, it only prints the strings from the initialized and loaded sections of object files; for other types of files, it prints the strings from the whole file.|

## Referencias
- []()
