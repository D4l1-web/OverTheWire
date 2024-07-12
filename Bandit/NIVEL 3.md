En este nivel entenderemos como leer y listar directorios o ficheros ocultos.

Anteriormente utilizamos el comando "ls" ahora añadiremos el argumenos "-l" o "-la" en distribuciones PARROT.

```
ls -l
```
Gracias a esto podremos listar los directorios ocultos e encontrar dicho fichero para sacar la contraseña.
En este caso es un fichero llamado ".hidden". 
Aprendemos que los ficheros que llevan un "." delante son ocultos.

Para leerlo:
```
cat .fichero
```
