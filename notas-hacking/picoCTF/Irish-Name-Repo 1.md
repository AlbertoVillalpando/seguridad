## Descripción
There is a website running at `https://jupiter.challenges.picoctf.org/problem/33850/` ([link](https://jupiter.challenges.picoctf.org/problem/33850/)) or http://jupiter.challenges.picoctf.org:33850. Do you think you can log us in? Try to see if you can login!

## Solución
Inspeccionamos la página, buscamos un campo oculto en el html, y lo revelamos, si colocamos un valor nos rediirigirá a una página dónde nos mostrará una sentencia SQL.

Basandonos en esa sentencia, realizamos una SQL injection en el campo nombre o contraseña. 'or 1=1

picoCTF{s0m3_SQL_f8adf3fb}

```bash
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- [SQL Injections](https://www.w3schools.com/sql/sql_injection.asp)
