En este nivel tendremos problemas para logearnos con bandit26, porque no tiene /bin/bah, en el directio /home nos encontramos un "id_rsa"

Simplemente nos conectamos con la id_rsa
```
ssh -i id_rsa bandit26@localhosts -p 2200
```
La solución es minimizar la pantalla para que no cargue y pulsar "v" y posteriormente "SHIFT + :" y editaremos para leer
```
/etc/bandit_pass/bandit26
```
