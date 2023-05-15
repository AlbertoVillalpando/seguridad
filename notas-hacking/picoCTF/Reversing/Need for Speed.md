## Descripción


## Solución
Dar permisos de ejecución al archivo

Utilizar gdb.

Ver las funciones que contiene con 'info functions'

Ver el código del método main con 'disassemble main'

Agregar un break en el método main con 'break main'

ejecutar con 'run'

Llamar a la función get_key con 'call (int) get_key()'

Después llamar a la función que nos da la bandera 'call (int) print_flag()'

```bash
(gdb) info functions
All defined functions:

Non-debugging symbols:
0x00000000000005d8  _init
0x0000000000000600  putchar@plt
0x0000000000000610  puts@plt
0x0000000000000620  alarm@plt
0x0000000000000630  __sysv_signal@plt
0x0000000000000640  exit@plt
0x0000000000000650  __cxa_finalize@plt
0x0000000000000660  _start
0x0000000000000690  deregister_tm_clones
0x00000000000006d0  register_tm_clones
0x0000000000000720  __do_global_dtors_aux
0x0000000000000760  frame_dummy
0x000000000000076a  decrypt_flag
0x00000000000007f1  calculate_key
0x000000000000080e  alarm_handler
0x000000000000082f  set_timer
0x000000000000087d  get_key
0x00000000000008ac  print_flag
0x00000000000008d8  header
0x000000000000091a  main
0x0000000000000960  __libc_csu_init
0x00000000000009d0  __libc_csu_fini
0x00000000000009d4  _fini
(gdb) disassemble main
Dump of assembler code for function main:
   0x000000000000091a <+0>:	push   %rbp
   0x000000000000091b <+1>:	mov    %rsp,%rbp
   0x000000000000091e <+4>:	sub    $0x10,%rsp
   0x0000000000000922 <+8>:	mov    %edi,-0x4(%rbp)
   0x0000000000000925 <+11>:	mov    %rsi,-0x10(%rbp)
   0x0000000000000929 <+15>:	mov    $0x0,%eax
   0x000000000000092e <+20>:	callq  0x8d8 <header>
   0x0000000000000933 <+25>:	mov    $0x0,%eax
   0x0000000000000938 <+30>:	callq  0x82f <set_timer>
   0x000000000000093d <+35>:	mov    $0x0,%eax
   0x0000000000000942 <+40>:	callq  0x87d <get_key>
   0x0000000000000947 <+45>:	mov    $0x0,%eax
   0x000000000000094c <+50>:	callq  0x8ac <print_flag>
   0x0000000000000951 <+55>:	mov    $0x0,%eax
   0x0000000000000956 <+60>:	leaveq 
   0x0000000000000957 <+61>:	retq   
End of assembler dump.
(gdb) break main
Punto de interrupción 1 at 0x91e
(gdb) call (int) get_key()
No puede hacer esto sin un proceso de depuración.
(gdb) run
Starting program: /home/alberto/Descargas/need-for-speed 

Breakpoint 1, 0x000055555555491e in main ()
(gdb) call (int) get_key()
Creating key...
^[[AFinished
$1 = 9
(gdb) call (int) print_flag()
Printing flag:
PICOCTF{Good job keeping bus #24c43740 speeding along!}
$2 = 56

```

## Notas Adicionales
|comando|descripcion|
|---|---|
|xx|xx|

## Referencias
- []()
