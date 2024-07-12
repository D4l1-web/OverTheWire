## NIVEL 5 D4l1

En este caso nos encontramos con muchos directorios y OverTheWire nos pide que tenemos que encontrar la contraseña con unas propiedades particulares:
1. Human-readable
2. 1033 bytes size
3. not executable

Gracias a esto aprenderemos el comando "find" con el argumento "-type f"

```
find -type f
```
posteriormente nos pide que tiene que ser leido por el ser humano
```
find -type f -readable
```
##TIPS

Un tip que quiero dejar es que en bash si ponemos un "!" hacemos lo contrario con lo cual si queremos buscar algo que no sea ejecutable:

```
!-executable
```

##FINAL

Con todo esto solo nos falta los bytes que aqui utilizaremos el argumeno "-size 1033c" para especificar los bytes, con todo esto el comando final sera:

```
find -type f -readable !-executable -size 1033c
```
Si posteriormente queremos leer el resultado sin problemas alfinal del comando ponemos :
```
| xargs cat o | xargs cat | xargs
```
