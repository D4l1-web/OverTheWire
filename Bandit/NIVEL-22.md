Aquí también estamos jugando con Cron y hacemos lo mismo y nos vamos a "/etc/cron.d"

Si abrimos el archivo tenemos una función tal que así
```
myname= $(whoami) | [Variable = quien es]
mytarger= $(echo I am user) $my name|m5sum|
cut -d'' -F 1
```
Nos comenta que bandit23 esta hasheado, esa es la función

Copia dicho hash y dice que es necesario para sacar la siguiente pass.

Lo primero que haremos es sacar dicho hash (Copiaremos la función y pondremos el nombre de bandit23)

Y leeremos la ruta /tmp/$mytarget y nos dará la pass
