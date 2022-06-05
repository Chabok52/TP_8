# 12) Ingresar 10 números enteros usando la variable X. Determinar e imprimir un mensaje informando:
# la cantidad de números POSITIVOS, la cantidad de números NEGATIVOS y, la cantidad de CEROS ingresados.
```mermaid
flowchart
A[Positivos = 0] --> B[Negativos = 0]
B --> C[Ceros = 0] --> 1[Contador = 0]
1 --> D[mientras Contador < 10:]
D --> |No| F[X = Ingrese numero entero]
F --> G{X == 0?}
G -->|Si| H[Ceros += 1] --> 2[Contador += 1]
2 --> D
G --> |No| I{X > 0?}
I --> |Si| J[Positivos += 1] --> 3[Contador += 1]
3 --> D
I --> |No| K[Negativos += 1] --> 4[Contador += 1]
4 --> D
D --> |Si| M[print: Positivos Negativos Ceros]
```
```python
Positivos = 0
Negativos = 0
Ceros = 0
Contador = 0
while Contador < 10:
    X = int(input("Ingrese un numero entero"))
    if X == 0:
        Ceros += 1
        Contador += 1
    elif X > 0:
        Positivos += 1
        Contador += 1
    else:
        Negativos += 1
        Contador += 1
print(f"Total: positivos: {Positivos} negativos: {Negativos} y ceros: {Ceros}")
```