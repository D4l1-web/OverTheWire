# Nivel 8 Natas

Nos encontramos con un nivel muy parecido al nivel 6 vamos a ver.

Nos deja la opción de ver como funciona el código secreto .

![image](https://github.com/user-attachments/assets/cbfadb96-7bf4-4b7d-9e51-72ce0ab40351)

Vemos que el código secreto nos lo estan dando y que esta códificado en hexadecimal, invertido y codificado en base64 vamos haya

- (bin2hex) : binario a hexadecimal
- (strrev) : Invertir String
- (base64_encode) : Codificar en base64

Vamos a probar a ejecutar ese código en PHP

```
$encodedSecret = "3d3d516343746d4d6d6c315669563362";

function decodeSecret($encodedSecret) {
  $secret = base64_decode(strrev(hex2bin($encodedSecret)));
  return($secret);
}

echo decodeSecret($encodedSecret);
```
![image](https://github.com/user-attachments/assets/9ddc33f1-d159-496f-ac87-853478f8fe9c)

Sacamos la "secret key" 

![image](https://github.com/user-attachments/assets/4e0a84c7-e8c0-4815-9dd1-fece51a02b54)

La pass es : ZE1ck82lmdGIoErlhQgWND6j2Wzz6b6t

GG
