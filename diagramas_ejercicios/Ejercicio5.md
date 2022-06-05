## 5) Escriba un diagrama de flujo que permita generar e imprimir los primeros 5 números naturales en orden descendente (a partir de 5). 
```mermaid
flowchart TD
    A[C = 5] --> B{C > 0?}
    B --> |Si| C[Print C]
    C --> D[c -= 1]
    D --> B
    B --->|No| E[end]
```

```python
c = -1
while c > -6:
    print(c)
    c -= 1
```
