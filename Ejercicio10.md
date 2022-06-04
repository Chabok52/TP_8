# 10) Ingresar números enteros en la variable B y, MIENTRAS el valor ingresado en B sea
POSITIVO, calcular la cantidad de números ingresados e imprimirla en un mensaje.
```mermaid
flowchart TD
	A[numeros = 0] --> B[B = Ingrese un número entero]
	B --> C{B > 0?}
	C --> |No| D(print el total de numeros ingresados fue: 'numeros')
	C --> |Si| E[numeros += 1]
	E --> B
	D --> F(end)
```

```python
numeros = 0
B = int(1)
while B > 0:
    B = int(input("Ingrese numero entero... "))
    numeros += 1
print(numeros)
```