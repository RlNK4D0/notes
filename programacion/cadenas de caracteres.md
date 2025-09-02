#programacion 
[[tipos de datos]]  -> *str*


string -> str :
	un string puede ser desde 0 caracteres '' hasta infinitos caracteres dentro del ' ' 
	se puede usar " " también para crear un string
	el string tiene de rango máximo los 256 caracteres del codigo ascii
	los strings tambien son indexables [[indices]] 
	y son [[objetos iterables]]

la \ es un caracter de escape para los strings, *ignora el proximo caracter del string*

```
marca = 'chilli\'s'

resultado = "chilli's"
```

![[Pasted image 20250512185501.png]]

	chr() -> [[funciones]] que se utiliza para convertir un numero ascii en     el caracter correspondiente

	ord() -> se utiliza para convertir un caracter en un numero ascii

###### los strings se concatenan +
en memoria [[uso de memoria]] , al concatenar strings, cada string tiene su ID 
al concatenarlos, se crea un nuevo objeto con su ID propio 


**python permite multiplicar los strings * 

-> en los strings la multiplicación, * significa repetición 

```
str = "string" * 3

output -> 3 veces el string

```

-> forma de imprimir \n que es un caracter especial de salto de linea
```
print("\\n")

output -> "\n"
```

###### los strings se pueden comparar 
-> con los [[operadores relacionales en python]]  
	en los comparadores que no sean de == python va a tomar los valores ascii de los str y comprar estos valores numericos
	

###### slicing / rebanando / sub-cadenas

```
saludo = "Hola mundo!"
saludo = saludo[5::10] /// [5:10:1] el tercer parametro 1 es opcional
output -> "mundo"
```

-> corta un string desde el indice 5 hasta el indice 10 exclusivamente (excluye el 10)

```
corta el string:

 primer  : -> desde
 segundo : -> hasta
 tercer  : -> contador (1 por default)
```

-> el tercer parametro es un contador para saber de a cuanto en cuanto va a recorrer el str -> vease [[bucle for]]

-> si se deja un : va a hacer una copia del *str* , haciendo un [[pointers]] hacia el mismo objeto, por lo tanto van a tener el mismo ID en memoria 

el slicing tambien aplica para [[listas]]
![[Pasted image 20250512195028.png]]


-> alternativa a .lower() para convertir los caracteres en minusculas
![[Pasted image 20250512202402.png]]

