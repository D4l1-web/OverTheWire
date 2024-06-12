Nos encontramos de nuevo con el archivo "data.txt" y tenemos que encontrar la contraseña del nivel en todo el texto y es la unica linea que no se repite.

En este caso vamos a aprender el comando "uniq-u" y "sort" para ordenar y solo ver las no repeticiones

```
uniq-u
sort
```
```
cat data.txt | sort | uniq-u
```
