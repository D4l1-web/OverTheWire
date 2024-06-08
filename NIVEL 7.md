# INICIO 

Nos encontramos un archivo "data.txt" con una infinidad de palabras.

Aprenderemos el comando "grep"

Permite filtrar y eliminar la información inútil que se produce tras ejecutar un comando

```
grep
```
Nos comentan que cerca de la palabra "millionth" tenemos la contraseña del siguiente nivel.

Esto es bastante simple, debemos obviamente leer el archivo y filtrar seguun dicha palabra

```
cat data.txt | grep "millionth"
```
Otra forma podria ser sin utilizar el "cat"
```
grep "millionth" data.txt
```

