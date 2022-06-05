## 9) Ingresar un número natural en la variable A. Determinar e imprimir un mensaje informando: si A es múltiplo de 3 o no. 
```mermaid
flowchart TD
1((1)) --> 2((2))
2 --> 1
2 --> 3((3))
3 --> 4((4))
3 --> 5((5))
style 2 fill:#03FAAF,color:#000000
style 4 fill:#E51512,color:#fffff
style 5 fill:#E51512,color:#fffff
```

Calculo ciclomático: |
---------------------|
Nodos = 5 |
Aristas = 5 |
Regiones = 2 |
Aristas - nodos + 2 = 2 |
Nodos predicados + 1 = 2 |

Caminos posibles: |
------------------|
 1, 2... |
 1, 2, 3, 4 |
 1, 2, 3, 5 |