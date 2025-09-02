#programacion 

son un [[tipos de datos]]

las listas son una coleccion de elementos de distintos tipos de datos en una misma lista 

una lista *en python unicamente* puede tener elementos numericos, string, bool por ser un lenguaje *dinamico*
-> en [[matrices]] es posible manejar listas con distintos tipos de datos ya que las trabajamos en forma de listas paralelas 
	![[Pasted image 20250526192815.png]]
	- en python es posible utilizar la primera forma 
	- en otros lenguajes hace falta decir que tipo de datos almacena la lista, por lo tanto es posible SOLO utilizar el segundo ejemplo 
	- probablemente inútil porque en [[métodos]] se va aprender como almacenar listas con distintos tipos de datos mas eficientemente 


las listas se pueden recorrer, convirtiéndolas en [[objetos iterables]] y se navegan con el [[indices]] 

mutables 
indexables
iterables


una lista con 4 elementos, va a tener una longitud de 4 y un index 0,1,2,3

---

### tipos de datos en una lista

[[tipos de datos]] en una lista

```
lista[i]

```

esto se refiere SIEMPRE a que tipo de dato esta almacenando la lista en ESE indice

por ej:

```
lista = ["str", int, "str"]

lista [i] 

va a ser el tipo de dato en el que caiga, si el indice es 0, un str, si es 1 es un int, si es 2, un str

cabe aclarar que NO es recomendable combinar tipos de datos en listas

esto solo es para efectos de explicacion

```


---
## arreglos uni-dimensionales

un array, o arreglo uni-dimensional, o un vector es una lista

son un tipo de dato mutable e index-able, es decir que se puede modificar los datos de una lista y su longitud 

para acceder a un elemento se debe indicar el numero el del elemento

```
saludo = "hola mundo"
print (saludo[3]) -> a 
```

```

#el valor que se le asigna a la lista, es una lista en si, la variable lista de alumnos esta concatenando los valores ingresados, nombre1,nombre2,nombre3

#esto es una union de 2 listas

lista_de_alumnos += [nombre]

```

en python se puede ingresar distintos tipos de datos en una lista, en otros lenguajes **NO** funciona asi 

listas en [[uso de memoria]]

las listas se pueden anidar
```
list = [1,2,3,4,[1,2,3]]
```

recorrer listas  con for each

```
for num in lista:
	
```

este for no tiene indices, pero si tiene el valor

---

a las listas se pueden aplicar los [[operadores aritméticos en python]] 

```
lista = [none] * 5


devuelve 5 [None]
[None]
[None]
[None]
[None]
[None]
 
```


para pisar un valor en una lista se puede hacer

```
lista [0] = "string" / int / float / lo que pinte
```

*0* es el [[indices]] de la lista

si mi lista tiene elemento en indice 0 y quiero añadir  elemento en el indice 2 va a retornar error porque la lista no esta inicializada 
```
#lista no inicializada
lista = []

#lista inicializada
lista = [None] * 5

```
esta lista inicializada va a tener 5 elementos con [[pointers]] hacia el objeto *none* 

si se une un elemento nuevo a la lista 
```
lista += ["hola"]
```
este nuevo elemento se va a añadir al final de la lista, va a devolver 5 None y 1 Hola al final

las listas al sumarlas, se unen o concatenan, como se especifica en [[tipos de datos]]

en cambio si yo quiero asignar un valor (=) a un lugar en el indice 

```
lista [0] = "chau"
```
esto va a devolver un chau al inicio, 3 none y 1 hola al final 

y finalmente si volvemos a intentar asignarle otro valor al indice 2 

```
lista [2] = "juan"
```

va a devolver:
0-chau
1-none
2-juan
3-none
4-none
5-hola

son 6 elementos en total, indice termina en 5 

![[Pasted image 20250425213908.png]]

---

para imprimir el ultimo valor de una lista de la cual no conozco la cantidad de elementos
```
	print (lista [ ( len (lista) -1) ] )
```
len devuelve la cantidad de elementos, pero como el indice inicia en 0, el valor que estoy buscando es -1 de la longitud total

---
para ingresar un valor el cual va a ser usado como indice y que no ingrese un valor superior al máximo 

![[Pasted image 20250425220157.png]]

---


### formas de cargar una lista

https://onlinegdb.com/hfaPlWZfSk

Secuencial:
para el tipo de carga secuencial, NO hace falta inicializar la lista, es decir pre generar los elementos [None, None]

```
def ingreso_datos_enteros_lista(iteraciones:int, mensaje:str = "") -> list:

"""

ingresa datos numericos a una lista \n

iteraciones: cantidad de iteraciones de la funcion \n

mensaje: output para el usuario \n

retorna una lista con valores enteros agregados \n

"""

lista = []

for i in range(iteraciones):

min = input (mensaje)

  

if valid_int_input(min) == True:

lista += [int(min)]

else:

break

return lista


```


carga aleatoria:

para la carga aleatoria es NECESARIO que la lista este inicializada 

```
lista = [None,None,None,None,None]
```

![[Pasted image 20250428194852.png]]



---

## copiar una lista

```
lista_a = lista_b
```
lista_a apunta a lista_b [[pointers]], hace una referencia [[uso de memoria]]
si modificamos una se modifican ambas listas 

```
lista_b = lista_a + []

```
de esta forma se puede hacer una copia de la lista, concatenarle una lista al final es crear un objeto nuevo

otra forma es 

```
lista_b = lista_a

lista_b += []

```
esta otra sintaxis es como ejecutar un [[métodos]] .append()

forma correcta:

![[Pasted image 20250505200541.png]]

-> shallow copy
```
lista copia = lista[:]

lista_copia = lista.copy()
```

-> explicacion:
	se le llama shallow copy porque esta creando una copia de la CANTIDAD de elementos para almacenar objetos, y solo guarda las [[referencias]]
	-> al modificar alguno de los elementos de la lista copia, se elimina la referencia anterior y se almacena la referencia del nuevo objeto
	![[Pasted image 20250526193650.png]]
	diagrama en memoria 

-> shallow copy en [[matrices]]
```
matriz = [[5,4],
		  [2,1]]

matriz_copia = matriz.copy()
matriz_copia[1][0] = 15

```
-> tanto la matriz original como la copia van a imprimir un 15 en lugar del 2 
	![[Pasted image 20250526194646.png]]
	diagrama en memoria
	para copiar elementos inmutables el .copy funciona bien guardar la referencia
	pero para objetos mutables se guarda la referencia a la lista, por lo tanto al hacer un cambio se modifica la lista dentro de la matriz original
	![[Pasted image 20250526201055.png]]
	

-> deep copy 
	 [[matrices]] -> deep copy
	 
[[cadenas de caracteres]] -> slicing 

---


