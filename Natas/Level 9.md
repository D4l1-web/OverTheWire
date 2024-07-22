# Nivel 9 Natas

Una vez accedido a este nivel encontramos un cuadro en el que nos dice que busquemos palabras que contengas un boton de buscar.

![image](https://github.com/user-attachments/assets/1b28b97a-c2e2-4fbe-930d-0edea5c0e74a)

Dentro del código nos encontramos con : 

![image](https://github.com/user-attachments/assets/6e179362-c24e-4a3b-9fc9-a8c87254972b)

Analizamos y vemos que se utiliza la función "passthru" permitiendo ejecutar comandos como las funciones "exec" y "system"

El comando "grep -i" nos permite búscar las palabras ignorando mayúsculas y minúsculas dentro del fichero "dictionary.txt"

Entonces entendiendo esto simplemente deberemos parar de hacer el comando grep con un ; o | y hacer un cat al fichero de las contraseñas
```
; cat /etc/natas_webpass/natas10
```

![image](https://github.com/user-attachments/assets/9a28f4ca-ff06-47b6-a611-eeb5c8547a50)

La pass es : t7I5VHvpa14sJTUGV0cbEsbYfFP2dmOu

GG 
