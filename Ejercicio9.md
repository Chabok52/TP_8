## 9) Ingresar un número natural en la variable A. Determinar e imprimir un mensaje informando: si A
es múltiplo de 3 o no. 
```mermaid
flowchart TD
	A[A = Ingrese un número] --> B{A >= 0?}
	B --> |No| A
	B --> |Si| C{A % 3 == 0?}
    C --> |Si| D[print: A es multiplo de 3]
    C --> |No| E[print: A no es multiplo de 3]
```

```python
A = int(input("Ingrese un número "))
assert A >= 0, "El número debe ser positivo"
if A % 3 == 0:
    print(f"{A} es múltiplo de 3")
else:
    print(f"{A} no es múltiplo de 3")
```