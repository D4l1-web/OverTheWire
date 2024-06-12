En este caso nos encontramos otro archivo hexadumpeado y que se ha sido repetidamente comprimido.

Nos comentan qe esta bien crear un directorio en la ruta "/tmp" y trabajar ahi.

Aprendemos el comando "xxd" para parsar a hexadecimal
```
xxd
```

Si hacemos un "file" al archivo vemos que es un GZIP

```
file archivo
```
Aprendemos a crear un "Script" para Bash para descomprimir, creando un ".sh" y dandole permisos de ejecución "chmod +x programa"
```
chmod +x programa"
```
Mejoramos con el "grep"
```
grep "Name" -A 2
```
Hace que liste en parametro mas dos líneas abajo "-A" "-B" "-C"

Utilizamos "gzip -d" para descomprimir
```
gzip -d
```
## PASOS
```
cat data.txt | xxd -r > data
file data
mv data data.gz
gzip -d data2.gz
file data2
mv data2 data3.bz
```
Así sucesivamente hasta llegar a un "tar".

Llegaremos al 9 y encontaremos la contraseña.
