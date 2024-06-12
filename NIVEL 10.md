En este nivel nos encontraremos de nuevo con un "data.txt" pero en este caso cifrado en "base64"

```
cata data.txt | base 64 -d
```
Utilizaremos el parametro "-d" para descifrar.

También aprendemos el comando "tr"
```
tr
```
```
cata data.txt | base64 -d | tr " " '\n'
```
Gracias a esto cambiamos los espacion por saltos
