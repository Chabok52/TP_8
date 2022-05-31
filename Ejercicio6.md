#6) Escriba un diagrama de flujo que permita generar e imprimir los primeros 5 números naturales 
pares (a partir de 2).
```mermaid
flowchart TD
	A[C = 2] --> B{C >= 7?}
	B --> |NO| C[print C]
	C --> D[C = C+2]
	D --> B
	B --> |SI| E[end]
```