# 12) Ingresar 10 números enteros usando la variable X. Determinar e imprimir un mensaje informando: la cantidad de números POSITIVOS, la cantidad de números NEGATIVOS y, la cantidad de CEROS ingresados.
```mermaid
flowchart
A((1)) --> |i| B((2))
B -->|ii| C((3)) -->|iii| 1((4))
1 -->|iv|D((5))
D --> |v|F((6))
F --> |vi|G((7))
G --> |vii|H((8)) --> |viii|2((9))
2 --> |ix|D
G --> |x|I((10))
I --> |xi|J((11)) --> |xii|3((12))
3 --> |xiii|D
I --> |xiv|K((13)) -->|xv| 4((14))
4 --> |xvi|D
D --> |xvii|M((15))
style D fill:#03FAAF,color:#000000
style G fill:#03FAAF,color:#000000
style I fill:#03FAAF,color:#000000
style M fill:#E51512,color:#fffff
```

Calculo ciclomático: |
---------------------|
Nodos = 15 |
Aristas = 17 |
Regiones = 4 |
Aristas - nodos + 2 = 4 |
Nodos predicados + 1 = 4 |

Caminos posibles: |
------------------|
 1, 2, 3, 4, 5, 6, 7, 8, 9, 5 ..., 15 |
 1, 2, 3, 4, 5, 6, 7, 10, 11, 12, 5 ..., 15 |
 1, 2, 3, 4, 5, 6, 7, 10, 13, 14, 5 ..., 15 |
 1, 2, 3, 4, 5, 6, 7, 8, 9, 5, 6, 7, 10, 11, 12, 5, 6, 7, 10, 13, 14, 5, ..., 15 |
