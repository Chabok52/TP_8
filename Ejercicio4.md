## 4) Escriba un diagrama de flujo que permita generar e imprimir los primeros 5 números enteros negativos
```mermaid
flowchart TD
    A[C = 0] --> B[C -= 1]
    B --> C[C > -6?]
    C --> |Si| D[Print C]
    D --> B
    C -->|No| F[end]