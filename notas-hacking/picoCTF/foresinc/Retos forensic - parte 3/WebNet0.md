## Descripción
We found this packet capture and key. Recover the flag.

Ya que los streams tcp están ecnriptados, necesitamos utilizar la key que nos proporcionan con la ip 0.0.0.0, puerto 443 y protocolo http.

## Solución
Ahora podemos ver la Transport Layer Security

Filtramos esta capa y seguimos el primer http stream y le realizamos un seguimiento mediante http. 

Aquí encontraremos la bandera.

picoCTF{nongshim.shrimp.crackers}

```bash
HTTP/1.1 200 OK
Date: Fri, 23 Aug 2019 15:56:36 GMT
Server: Apache/2.4.29 (Ubuntu)
Last-Modified: Mon, 12 Aug 2019 16:50:05 GMT
ETag: "5ff-58fee50dc3fb0-gzip"
Accept-Ranges: bytes
Vary: Accept-Encoding
Content-Encoding: gzip
Pico-Flag: picoCTF{nongshim.shrimp.crackers}
Content-Length: 821
Keep-Alive: timeout=5, max=100
Connection: Keep-Alive
Content-Type: text/html
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()

