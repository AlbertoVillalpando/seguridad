## Descripción
Connect to this PostgreSQL server and find the flag! `psql -h saturn.picoctf.net -p 64608 -U postgres pico` Password is `postgres`

## Solución
Para mostrar las tablas desde una terminal de postgres se utiliza el comando `\d`, una vez conocidas podemos ejecutar una consulta. 

select * from flags;

picoCTF{L3arN_S0m3_5qL_t0d4Y_21c94904}

```bash
alberto@Nova:~$ psql -h saturn.picoctf.net -p 64608 -U postgres pico
Contraseña para usuario postgres: 
psql (15.2 (Ubuntu 15.2-1.pgdg20.04+1))
Digite «help» para obtener ayuda.

pico=# \d
        Listado de relaciones
 Esquema | Nombre | Tipo  |  Dueño   
---------+--------+-------+----------
 public  | flags  | tabla | postgres
(1 fila)

pico=# select * from flags;
 id | firstname | lastname  |                address                 
----+-----------+-----------+----------------------------------------
  1 | Luke      | Skywalker | picoCTF{L3arN_S0m3_5qL_t0d4Y_21c94904}
  2 | Leia      | Organa    | Alderaan
  3 | Han       | Solo      | Corellia
(3 filas)
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()













