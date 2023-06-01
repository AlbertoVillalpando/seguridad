## Descripción
We found this weird message being passed around on the servers, we think we have a working decryption scheme. Download the message [here](https://artifacts.picoctf.net/c/127/message.txt). Take each number mod 37 and map it to the following character set: 0-25 is the alphabet (uppercase), 26-35 are the decimal digits, and 36 is an underscore. Wrap your decrypted message in the picoCTF flag format (i.e. `picoCTF{decrypted_message}`)

## Solución
Desencriptamos el mensaje con el siguiente código

picoCTF{R0UND_N_R0UND_79C18FB3}


```bash
message = "128 322 353 235 336 73 198 332 202 285 57 87 262 221 218 405 335 101 256 227 112 140".split()  
  
dictionary = [i for i in range(0, 37)]  
  
char_list = list("ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_")  
  
d = {dictionary[i]: char_list[i] for i in range(len(dictionary))}  
  
for i in range(len(message)):  
	print(d[int(message[i]) % 37], end='')

/usr/bin/python3.8 /home/alberto/Escritorio/pyth_xp/xpli.py 
R0UND_N_R0UND_79C18FB3
Process finished with exit code 0
```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
