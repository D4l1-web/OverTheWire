En este nivel nos encontramos que nos dicen que la flag se puede conseguir del puerto "3000" del localhost.

Para comprobar si esta abierto
```
echo ">/dev/tcp/127.0.0.1/30000
```

Si no sale error sabemos que esta abierto.

Dando la contraseña del mismo bandit, le pasamos una cadena de caracteres

```
echo "pass" |nc localhost 30000
```
Otra forma sería por telnet
```
telnet localhost 30000
```
