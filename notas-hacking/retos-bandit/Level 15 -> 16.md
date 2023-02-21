# Level 15

## Objetivo
The password for the next level can be retrieved by submitting the password of the current level to **port 30001 on localhost** using SSL encryption.

**Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…**

## Datos de Acceso
bandit15
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt

## Solución
```bash
bandit15@bandit:~$ openssl s_client -connect localhost:30001
CONNECTED(00000003)
Can't use SSL_get_servername
depth=0 CN = localhost
verify error:num=18:self-signed certificate
verify return:1
depth=0 CN = localhost
verify error:num=10:certificate has expired
notAfter=Feb 21 06:20:29 2023 GMT
verify return:1
depth=0 CN = localhost
notAfter=Feb 21 06:20:29 2023 GMT
verify return:1
---
Certificate chain
 0 s:CN = localhost
   i:CN = localhost
   a:PKEY: rsaEncryption, 2048 (bit); sigalg: RSA-SHA1
   v:NotBefore: Feb 21 06:19:29 2023 GMT; NotAfter: Feb 21 06:20:29 2023 GMT
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIDCzCCAfOgAwIBAgIEA7qUdzANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls
b2NhbGhvc3QwHhcNMjMwMjIxMDYxOTI5WhcNMjMwMjIxMDYyMDI5WjAUMRIwEAYD
VQQDDAlsb2NhbGhvc3QwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDL
vM0gZzAHdXTeD5t4ruUJo/kRs4UAodA9XcqDhNtW464W0c55RqKLp921syy3Lvjr
8Q9WkqvCFX+efShMd8XnzbT/dyRrD+cZQnSiPJ3bwDdpwqfkl9h3mb609Kb5HI6R
JgogEyuRLJI+HKtr/wXHwo1vBZ0+yaPMX6sdkd6Hu5Ra0L5Q5+E5+3F/8QgvCeVE
hDRIOrh2a7jxykb8G6+xVC6jIZY0YfrZz6LrESyQau256pqyaQPqQoUWTlitxIql
Ym2Baw7vYDxmFZrvj0FkumC6NokX6K2G9bZ0DaKR/DspPdAC4oT81SawJvsBibdN
51VI6dxBn412ZS8bS155AgMBAAGjZTBjMBQGA1UdEQQNMAuCCWxvY2FsaG9zdDBL
BglghkgBhvhCAQ0EPhY8QXV0b21hdGljYWxseSBnZW5lcmF0ZWQgYnkgTmNhdC4g
U2VlIGh0dHBzOi8vbm1hcC5vcmcvbmNhdC8uMA0GCSqGSIb3DQEBBQUAA4IBAQA9
skxWNwZbedjaVTa5yMPUZQ4Nf5/LAAMtS5Q7mzGH5tdQsTGR0Z4n4eA4hzrmzHBF
MVRL5mR9n+sM5pIrKDa6f4zIc5ObxDyN19ie+3SFASCPz9tihK8Js2V8qsR6LHV1
pfD8DSG0hZPtUuK3Mfi+nWqQUFiiTGj30mb9vlS1sSWv5PGznou1gQ3ZfrDs7B4K
ZKZrllPIVV1CrlDw2Bv8Dc432LQuZAmKAjBd6FG0OAboU/WJMTwAfVjlKMtvC8tg
DZ3djSTprq6PrXlI0utw/MsMIh69b61BRXUuDvRxhU11SNmSI8aegjVL8KuK+Euh
sSLPTocV29SY1YXOwEQi
-----END CERTIFICATE-----
subject=CN = localhost
issuer=CN = localhost
---
No client certificate CA names sent
Peer signing digest: SHA256
Peer signature type: RSA-PSS
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 1339 bytes and written 373 bytes
Verification error: certificate has expired
---
New, TLSv1.3, Cipher is TLS_AES_256_GCM_SHA384
Server public key is 2048 bit
Secure Renegotiation IS NOT supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
Early data was not sent
Verify return code: 10 (certificate has expired)
---
---
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: 3E0A3E59DA27969BBDEA29450F7C7BCDE713EC9AABC33DA522D4FA13E3E686D5
    Session-ID-ctx: 
    Resumption PSK: 4EAE7DAE86E8C61422E773F9B968AB904102AA0615228FA7CA91F6035DD7C24147B711569184A6762E909355BA8B5EF0
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - ee ae 09 e4 56 06 6c 9e-c9 80 86 77 50 83 15 59   ....V.l....wP..Y
    0010 - d4 d5 94 20 f3 ea 0f 3c-f0 16 47 7e 39 7e 3e 06   ... ...<..G~9~>.
    0020 - d2 12 80 e1 36 ff b1 65-31 ba f3 90 0f 63 29 4e   ....6..e1....c)N
    0030 - 3d a8 64 ae 6d 00 2b b7-ec e7 64 96 c3 fc 5c be   =.d.m.+...d...\.
    0040 - 71 89 20 59 3b af 63 36-32 88 1b 39 87 56 47 e0   q. Y;.c62..9.VG.
    0050 - 2e 20 6f ca b7 5a a5 4a-68 a9 9b 00 02 2e db 70   . o..Z.Jh......p
    0060 - 95 11 31 11 6e 65 44 d0-ed 42 1c c1 05 e2 1f 0f   ..1.neD..B......
    0070 - 94 74 50 a7 7f 6d 34 57-4b b8 99 f5 f0 a9 61 36   .tP..m4WK.....a6
    0080 - fc c7 8c 6d 0a eb 61 9b-92 72 66 62 58 8e bd b8   ...m..a..rfbX...
    0090 - 69 e3 e7 c1 dd bb 95 f9-0c b1 93 d9 63 55 4c e2   i...........cUL.
    00a0 - a5 53 38 75 f1 15 52 00-0f de 5a c7 27 9c 40 f9   .S8u..R...Z.'.@.
    00b0 - 83 fb b3 93 ec c6 cf 0c-5d d0 d7 16 fc 82 6b 5d   ........].....k]
    00c0 - b7 f9 75 19 26 3c fa 15-eb 50 a9 20 f0 6e cd e5   ..u.&<...P. .n..

    Start Time: 1677007693
    Timeout   : 7200 (sec)
    Verify return code: 10 (certificate has expired)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
---
Post-Handshake New Session Ticket arrived:
SSL-Session:
    Protocol  : TLSv1.3
    Cipher    : TLS_AES_256_GCM_SHA384
    Session-ID: 621E6DBF8C51DF7A59DD1BEA064066296DBCC18C5BF6457962860044298CE79C
    Session-ID-ctx: 
    Resumption PSK: DE6096BA40AC395861A6B676338DE4EFC82DCC1C3075188C8CAF75C12E277C1165E9FEC600194EF5E7C673DBFBB2E627
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - ee ae 09 e4 56 06 6c 9e-c9 80 86 77 50 83 15 59   ....V.l....wP..Y
    0010 - 76 c9 c4 fd 0d 97 13 5a-a5 38 b3 0f 4e 4d 51 11   v......Z.8..NMQ.
    0020 - 51 f2 70 ae b4 82 02 46-da 0a fc 63 6a 81 0a 25   Q.p....F...cj..%
    0030 - 2e d2 c1 0d de 74 f0 ca-b0 e5 37 bd 35 0b b5 58   .....t....7.5..X
    0040 - eb 6b 69 a1 ee 77 de 89-6f f6 03 c8 53 3d 50 63   .ki..w..o...S=Pc
    0050 - 52 1b da 01 3d 85 01 4c-6c fe d2 b3 78 40 5c 33   R...=..Ll...x@\3
    0060 - a6 db da be 58 e9 d3 0d-2b 6f b7 10 29 ac 8e ab   ....X...+o..)...
    0070 - 0a 3c 5b 26 ac 3f 46 a1-39 d8 9d cf ee 13 ed 65   .<[&.?F.9......e
    0080 - e7 67 70 63 04 10 7f 9c-22 0a 16 3e ea 14 2e 12   .gpc...."..>....
    0090 - 5d ca ea e3 50 d6 5d 97-1a c8 7e 6d 48 9d 2e 53   ]...P.]...~mH..S
    00a0 - 76 5d 80 23 f4 5f f3 53-d4 03 ba 65 02 66 55 31   v].#._.S...e.fU1
    00b0 - 43 8b 3d 6b b4 0d 58 0e-d3 08 84 51 f0 0e 96 82   C.=k..X....Q....
    00c0 - 91 4a 84 70 34 51 f4 ef-b7 61 1e 29 85 ba 17 b8   .J.p4Q...a.)....

    Start Time: 1677007693
    Timeout   : 7200 (sec)
    Verify return code: 10 (certificate has expired)
    Extended master secret: no
    Max Early Data: 0
---
read R BLOCK
jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
Correct!
JQttfApK4SeyHwDlI9SXGR50qclOAil1

closed

```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
