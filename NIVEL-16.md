Nos encontramos con lo mismo que el anteiror pero no sabemos el puerto, nos dan un ranto [30000-32000]

Aquí utilizaremos la herramient "nmap"
```
nmap --open -T5 -v -n -p31000-32000 127.0.0.1
```
Ahora deberemos encontrar cual de ellos estan hablando en SSL.

Probaremos el comando anterior
```
openssl s_client -connect 127.0.0.1:puerto
```
Vemos que nos devuelve una !CLAVE PRIVADA!

Todos los linux tienen un archivo temporal para probar con 
```
mktemp -d
```

Cambiamos los permisos 
```
chmod 600 name
```
Hacemos como anteriormente 
```
ssh -i id_rsa bandit17
```
