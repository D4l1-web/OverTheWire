#NIVEL 6 d4l1

#INICIO

Nos dice que en toda la máquina en la que nos hemos conectado debemos buscar un archivo con estas propiedades:
1. Owned user bandit 7
2. Owned group bandit 6
3. 33 bytes size

Sabiendo el anterior caso pensaremos que este es muy sencillo, pero hay que pensar un poquito.

Aqui aprenderemos que gracias al comando "find /" podemos buscar por todo el servidor
```
find /
```
Aprenderemos los argumentos "-user" y "-grop"
```
find -user -group
```
Nos encontraremos que si ponemos "size 33c" no conseguiremos hacer nada .

### IMPORTANTE

Debemos aprender el concepto de "/dev/null" (agujero negro)

Si queremos reventar un pc:
```
mv /* /dev/null
```
y en caso que lo queramos utilizar para que no nos salgan errores
```
2>/dev/null
```
Gracias a esto y con todo entendido.

#FINAL

```
find / -user bandit6 - group bandit7 -size 33c 2>/dev/null | xargs cat | xargs
```
