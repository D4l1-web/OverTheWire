# Nivel 10 

Nos encontramos con lo mismo que el nivel anterior, pero nos dice que ahora depende que cosas hay que filtrarlas.

![image](https://github.com/user-attachments/assets/d191e511-a58f-48a5-841a-31e92d3ac3a0)

Vemos en el código fuente que los caracteres ";" , "|" , "&" son ilegales .

![image](https://github.com/user-attachments/assets/335a2238-f7ac-4e90-b751-6ca667c6d032)

El comando "grep -i" nos permite realizar la búsqueda de palabras introducidas.

Si en el input lo ponemos tal que a sí "c /etc/natas_webpass/natas11" estaría buscando la letra c en el fichero "dictionary.txt" y en la ruta /etc/natas_webappas/natas11 donde se encuentra la contraseña para acceder al siguiente nivel.

He probado con eso y no ha funcionado con lo cual probare otros caracteres como ".*"

```
.* /etc/natas_webpass/natas11
```

![image](https://github.com/user-attachments/assets/2c224475-f06d-4660-9dc7-7d2169ea0e43)

La passe es: UJdqkK1pTu6VLt9UHWAgRZz6sVUZ3lEk

GG

