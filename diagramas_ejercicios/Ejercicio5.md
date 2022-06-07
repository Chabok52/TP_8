## 5) Escriba un diagrama de flujo que permita generar e imprimir los primeros 5 números naturales en orden descendente (a partir de 5). 
```mermaid
flowchart TD
    A[numero = 5] --> B{numero > 0?}
    B --> |Si| C[Print numero]
    C --> D[numero -= 1]
    D --> B
    B --->|No| E[end]
```

```python
numero = 5
while numero > 0:
    print(numero)
    numero -= 1
```
