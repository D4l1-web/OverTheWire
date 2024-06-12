Nos volvemos a encontrar de nuevo el "data.txt"

Aprenderemos el comando "strings" para ver cadenas de caracteres 
```
strings
```
Nos dice que para encontrar la passwords tiene cerca varios "===". Utilizaremos el comando
```
grep "==="
```
Tambien aprenderemos el comando "!$" para utilizar el último recursos que usamos.
```
!$
```
```
strings data.txt | grep "===" | tail -1
```
Pongo "tail -1" para que me salga solo la últinma línea.

Aprendemos también que con "echo $" creamos una variable
```
echo $
```

En bash las variables deben estar sin espacios.
