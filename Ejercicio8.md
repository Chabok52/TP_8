#8) Escriba un diagrama de flujo que permita ingresar 6 pares de números naturales que representan notas de parciales,
# en las variables N1 y N2, y que calcule e imprima el promedio de cada par de notas.
```mermaid
flowchart TD
A [contador = 0] --> B {Es contador = 12?}
B --> |NO| C [N1 = Ingresar nota 1]
C --> D [N2 = Ingresar nota 2]
D --> E [promedio = (N1+N2)/2]
E --> F [print(promedio)]
F --> G (contador += 1)
G --> B
B --> |Si| --> H [end]

```

```python
contador = 0
while contador != 12:
    N1 = abs(int(input("Ingrese nota... ")))
    N2 = abs(int(input("Ingrese la otra nota... ")))
    promedio = (N1 + N2)/2
    print(promedio)
    contador += 1
```