## 13) Ingresar 2 números naturales P y Q, donde P representa el multiplicando y Q el multiplicador.
## Se pide que, utilizando solamente la operación de suma, calcule el resultado de la operación P * Q
## e imprima el valor de P, de Q y de P * Q.
```mermaid
flowchart TD
    A((1)) --> B((2))
    B --> C((3))
    C --> D((4))
    style D fill:#03FAAF,color:#000000
    D --> C
    D --> E((5))
    E --> F((6))
    style F fill:#03FAAF,color:#000000
    F --> E
    F --> G((7))
    style G fill:#03FAAF,color:#000000
    G --> H((8))
    H --> I((9))
    I --> G
    G --> J((10))
    J --> K((11))
    K --> L((12))
    style L fill:#E51512,color:#fffff
```
Calculo ciclomático: |
---------------------|
Nodos = 12 |
Aristas = 12 |
Regiones = 2 |
Aristas - Nodos + 2 = 2 |
Nodos predicados + 1 = 2 |

Caminos posibles: |
------------------|
 1, 2, 3, 4, 5, 6, 7, 8, 9, 7...
 1, 2, 3, 4, 5, 6, 7, 10, 11, 12...
