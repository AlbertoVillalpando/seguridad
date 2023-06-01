## Descripción
In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/2604f8b51a5cc62d38a3736938f19cef/values)

## Solución
Desciframos el mensaje con el siguiente código:

picoCTF{sma11_N_n0_g0od_13686679}

```bash
from factordb.factordb import FactorDB

import gmpy2

c = 861270243527190895777142537838333832920579264010533029282104230006461420086153423
n = 1311097532562595991877980619849724606784164430105441327897358800116889057763413423
e = 65537
f = FactorDB(n)
f.connect()
p, q = f.get_factor_list()
ph = (p-1)*(q-1)
d = gmpy2.invert(e, ph)
plaintext = pow(c, d, n)
print("Flag: {}".format(bytearray.fromhex(format(plaintext, 'x')).decode()))

/usr/bin/python3.8 /home/alberto/Escritorio/pyth_xp/xpli.py 
Flag: picoCTF{sma11_N_n0_g0od_13686679}

Process finished with exit code 0
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
