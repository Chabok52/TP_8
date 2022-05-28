## 3) Escriba un diagrama de flujo que permita generar e imprimir los primeros 5 números naturales (a partir de 1).
```mermaid
flowchart TD
    A[C = 1] --> B{c < 6?}
    B --> |Si| C[print c]
    C --> D[c = c+1]
    D --> B
    B -->|No| F(end)
