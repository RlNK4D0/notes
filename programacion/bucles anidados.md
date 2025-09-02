#programacion 

**lo recomendable es hacer solo 3 niveles de anidamiento explicito**


```
for i in range(3):

	print (f"\n ============= A: {i} ===================")
	
	for j in range(5):
	
		print(f"B: {j}")

resultado:

 ============= A: 0  ===================
B: 0
B: 1
B: 2
B: 3
B: 4

 ============= A: 1  ===================
B: 0
B: 1
B: 2
B: 3
B: 4

 ============= A: 2  ===================
B: 0
B: 1
B: 2
B: 3
B: 4



```
ejecuta todas las iteraciones del bucle B, entonces vuelve al bucle A, hasta agotar las iteraciones del bucle A

basicamente, 3 iteraciones de bucle A es igual a 5 iteraiones del bucle B , 3 * 5 = 15 + 3 iteraciones del bucle A 

las funciones de [[break y continue]] afectan al bucle **mas cercano**, si yo ingreso un break en el bucle B, va a romper el bucle B volviendo al bucle A
