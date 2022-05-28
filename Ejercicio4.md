## 4) Escriba un diagrama de flujo que permita generar e imprimir los primeros 5 números enteros negativos
```mermaid
flowchart TD
    A[C = -1] --> B{C > -6?}
    B --> |Si| C[Print C]
    C --> D[C -= 1]
    D --> B
    B -->|No| F(end)
