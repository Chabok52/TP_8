## 13) Ingresar 2 números naturales P y Q, donde P representa el multiplicando y Q el multiplicador.
## Se pide que, utilizando solamente la operación de suma, calcule el resultado de la operación P * Q
## e imprima el valor de P, de Q y de P * Q.
```mermaid
flowchart TD
	A[contador = 0]
    A --> B[multiplicacion = 0]
    B --> C[P = Ingrese un multiplicando]
    C--> K[assert P > 0, El número debe ser mayor a 0]
    K --> |No| C
    K --> |Si| D[Q = Ingrese un multiplicador]
    D --> L[assert P > 0, El número debe ser mayor a 0]
    L --> |No| D
    L --> |Si| E{contador < Q?}
    E --> |Si| F[multiplicacion += P]
    F --> G[contador += 1]
    G --> E
    E ---> |No| H[print: P vale: P]
    H --> I[print: Q vale Q]
    I --> J[print: El resultado de P * Q es: multiplicacion]
```

```python
contador = 0
multiplicacion = 0
P = int(input("Ingrese el multiplicando "))
assert P >= 0, "El multiplicando debe ser positivo"
Q = int(input("Ingrese el multiplicador "))
assert Q >= 0, "El multiplicador debe ser positivo"
while contador < Q:
    multiplicacion += P
    contador += 1
print(f"P vale: {P}")
print(f"Q vale: {Q}")
print(f"El resultado de P * Q es: {multiplicacion}")
```