## 7) Escriba un diagrama de flujo que permita generar e imprimir los primeros 5 números naturales
## impares (a partir de 1).
```mermaid
flowchart TD
	A((1)) --> B((2))
    style B fill:#03FAAF,color:#000000
    B --> C((3))
    C --> D((4))
    D --> B 
    B ---> E((5))
    style E fill:#E51512,color:#fffff
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
 1, 2, 3, 4, 2... |
 1, 2, 5. |