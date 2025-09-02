#programacion 

algoritmos que buscan ordenar elementos en base a un criterio

existen millones de algoritmos de ordenamiento con ventajas y desventajas 

pero en la cursada vamos a ver el metodo *bubble sort* 

buble sort va a tomar el primer elemento y va a comprararlo contra el resto de elementos y entonces los va a ordenar 

toma el elemento1, pregunta si esta ordenado respecto al elemento2 y entonces va a mover de lugar ambos elementos

 para el algoritmo necesitamos 2 [[bucle for]]  anidados, tomando el primer elemento en el primer for, y el resto de elementos en el segundo for
  
los bucles arranacan
primer for: recorre desde el [[indices]] 0 hasta el ANTE-ultimo ` i -1`
segundo for: recorre desde el indice siguiente al primer for `i + 1` hasta el ultimo indice

```
for i in range (len(lista) -1 ):
	for j in range(i+1):
```

#### bubble sort

```
def ordenar_lista(lista:list) -> None:

"""

documentacion

"""

for i in range(len(lista) - 1):

	for j in range(i + 1, len(lista)):
		
		#pregunta
		
		if lista [i] > lista [j]:
			
			#swap
			
			aux = lista[i]
			
			lista [i] = lista [j]
			
			lista [j] = aux
```

![[Pasted image 20250516200051.png]]
funcion doble, ascendente y descendente en una sola condicion 

-> funcion para ordenar listas paralelas ej

![[Pasted image 20250516204632.png]]
