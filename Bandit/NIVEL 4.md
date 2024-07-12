#NIVEL 4 D4l1

En este caso nos encontramos con un directrio con muchos ficheros y que solo necesitamos ver los que tengan un lenguaje humano "readable"

Gracias a esto deberemos aprender y entender el comando "File" y los "magic numbers"

File determina el tipo y formato del fichero

```
file fichero
```
Los magic numbers, son los primero bits que tienen los ficheros para poder identificar que tipo de fichero es (Esto lo veremos mejor más adelante).

Entendido lo anteriormente explicado proseguimos con el procedimiento.

#PROCEDIMIENTO

Lo primero que deberemos hacer es identificar todos los ficheros, gracias a esto aprenderemos el argumento "*"

Con esto seleccionaremos todo, dentro de la ruta especificada.

```
File directorio/ *
```
Otra forma que podriamos utilizar ya mas enrevesada es:
```
Find . -name File * | xargs file
```
Aprendiendo el comando "File" con el argumento "."
Buscando todos los ficheros que contengan dicho nombre dentro de la ruta especificada.

El comando "xargs" hace que posteriormente al comando utilizado nos devuelva el resultado.
