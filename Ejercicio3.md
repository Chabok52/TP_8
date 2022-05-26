## 3) Escriba un diagrama de flujo que permita generar e imprimir los primeros 5 números naturales (a partir de 1).
partir de 1).
```mermaid
graph TD
    A[C = 1] --> B[print(C)]
    B --> C[C = C+1]
    C --> D{¿C == 5?}
    D -->|No| B
    D -->|Si| F[end]