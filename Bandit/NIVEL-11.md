En este nivel nos encontraremos un archivo donde las letras estan rotadas 13 posiciones.

Utilizaremos el comando "tr" para rotar

```
tr
```

Para que entendamos = abcdefghijklmnñopqrstuvwxyz

Cogemos la primera letra de su contenido "G"

```
cat data.txt | tr '[G-ZA-Fg-za-f]''[T-ZA-St-za-s]'
```
Haciendo esto conseguimos que las mayusculas y minusculas las interprete y "G +13" = T son 13 posiciones
