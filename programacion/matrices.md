#programacion 

son [[listas]] de listas, o matrices anidades

```

matriz = [ [1, 2], [3,4] ]

```

[[uso de memoria]] matrices

para acceder a un elemento dentro de una matriz necesito por ej:

```
matriz [1] [1]

= 4
```

lista 1, elemento 1  = 4
lista 1, elemento 0 = 3
lista 0, elemento 1 = 2
lista 0, elemento 1 = 1
vease [[indices]]

el segundo indice, se le llama sub indice 
```
							[1]     [1]
									sub-indice
```

```
len (matriz) = 2
len (matriz[1]) = 2

```

para printear una matriz necesitariamos un [[bucle for]] anidado

```
def print_matriz(matriz:list)->None:

	for i in range(len(matriz)):
	
		for j in range (len(matriz[i])):
		
			print(matriz[i][j], end= ", ")
			
	print("")
```

de esta forma lo que hace el primer for es recorrer los elementos de la matriz

los elementos de una matriz son las listas

el segundo for recorre los elementos de cada lista 

formato para declarar una matriz

```
matriz = [[1,3,5],
		  [9,8,7]]
```

la matriz se debe pensar como una planilla de calculo, en filas y columnas

```
def inicializar_matriz(filas:int, columnas:int, valor_inicial:any)->list:

#valor inicial = son valores que van a tomar el lugar de los elementos de las listas de la matriz, para que reserve el espacio

"""

inicializa una matriz con un valor deseado para operar \n

filas: int | cantidad de filas de la matriz \n

columnas: int | cantidad de columnas de la matriz \n

valor inicial: any | tipo de objeto que va a rellenar los espacios de la matriz para reservar memoria \n

"""

matriz = []

for i in range (filas):

	fila = [valor_inicial] * columnas
	
	matriz += [fila]

return matriz

```

resultado:

![[Pasted image 20250505215758.png]]
matriz de 5 filas x 3 columnas, con valor inicial de 0


carga de datos de una matriz

se puede cargar de 2 formas, aleatoria o secuencial al igual que con las [[listas]], porque las matrices son listas, comparten las mismas propiedades

secuencial
![[Pasted image 20250505223528.png]]

aleatorio

![[Pasted image 20250505223551.png]]

tambien se puede buscar un valor en una matriz de la siguiente manera

![[Pasted image 20250505223640.png]]

-> deep copy:
	copia los elementos en listas nuevas en lugar de copiar solo las referencias
	![[Pasted image 20250526201449.png]]
	lo ideal seria utilizar [[recursividad]] para ver si el tipo de dato que esta viendo es un [[tipos de datos]] primitivo / inmutable, o un tipo de dato mutable
	-----------------------------------------------------------------------
	![[Pasted image 20250526201747.png]]
	va a copiar los elementos primitivos dentro de matrices o listas para devolver una copia real de los datos dentro de la matriz independientemente de cuantas dimensiones tenga
	![[Pasted image 20250526201954.png]]
	.deepcopy() es un [[métodos]]
	--------------------------------------------------------------------------------
	