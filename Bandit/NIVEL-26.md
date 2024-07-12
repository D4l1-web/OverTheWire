Aquí nos toca spawnear una shell y seguir para la 27

Hacemos lo mismo que en el anterior y envede leer el archivo spawneamos una shell

```
:set shell=/bin/bash
```
Posteriormente hacemos lo mismo ":"
```
shell
```
Nos encontramos un binario y un "text.txt"

Si lo hacemos nos dice que ejecuta un comando con otro usuario y te da un ejemplo "./bandit27-do id", nosotros spawneamos una shell.

```
./bandit27 -do bash-p
```
O un cat a la passwd
