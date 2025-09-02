#programacion 

recursividad implica que una funcion se llame a si misma

[[uso de memoria]]

esto en memoria quiere decir que el programa se  pausa cuando se invoca por primera vez la funcion, y al volver a llamarse a la funcion dentro de si misma, se vuelve a pausar pero con otro valor asignado, en el caso de los *factoriales* es el numero anterior , es decir, inicia en 3, segunda llamada inicia en 2, tercera en 1 , cuarta en 0 

en memoria, estas llamadas recursivas, se aplican en el *stack*, una vez la ultima **instancia** (llamada de la funcion) se resuelva, se van a ir **des-apilando** del stack en memoria 

una vez se llega a la ultima instancia y se resuelve, se devuelve el resultado a la instancia anterior, de esa forma se resuelve devolviendo recursivamente 

ultima instancia = 1
tercera instancia = 1
segunda instancia = 2
primera instancia = 6

inputs : 
3 * 2 * 1 * 1 = 6

una vez se llega a la primera llamada de la funcion, en el programa main, para almacenar el resultado, recien ahi se genera el contenedor con el [[pointers]] del resultado de las funciones 

![[Pasted image 20250421221700.png]]

ventajas:
![[Pasted image 20250421222929.png]]

desventajas:

![[Pasted image 20250421222948.png]]


![[Pasted image 20250512184102.png]]
compara un valor a partir de un indice inicial
esto es un buscador de secuencia de numeros 

![[Pasted image 20250512184335.png]]
???????


![[Pasted image 20250512184443.png]]
transversar una matriz?
