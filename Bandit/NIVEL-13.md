Nos encontramos claves y nos comentar que la contraseña se almacena en "/etc/bandit_pass/usuario" 
Solo se puede leer con el usuario "Bandit14"

Deberemos conseguir conectandonos por "ssh" al siguiente nivel.

Nos dan una clave privada

Aprendemos a crear par de claves
```
sshkeygen
```
Como utilizarlo para conectarnos por ssh sin necesidad de contraseñas, entendiendo esto ya nos podemos conectar.
```
ssh -i "key" bandit14@localhost
```
En este cao he aprendido que con "Putty" no se puede hacer y necesitas tu propia máquina virtual.
