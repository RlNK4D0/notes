#programacion 


## Todos estos datos, son del tipo INMUTABLE

int -> integer :
	nuemero entero 
float -> floating:
	numero flotante, decimal ``3.14``

### los valores numericos se suman +=

bool -> boolean:
	el booleano solo tiene 2 valores, true or false, nada mas, un ejemplo de booleano y a la vez de [[casting]] es la sentencia **IF**
```
	var_test = 10
	if var_test >= 10:
		#codigo en caso de que if sea true
	else:
		#codigo en caso de que if sea false
```
	
	esto nos hace ver como python hace un casting de int a bool
	en la funcion **IF** 
	
string -> str :
	un string puede ser desde 0 caracteres '' hasta infinitos caracteres dentro del ' ' 
	se puede usar " " también para crear un string
	el string tiene de rango máximo los 256 caracteres del codigo ascii
	los strings tambien son indexables [[indices]] 
### los strings se concatenan +=


## Tipo de dato mutable

listas -> [[listas]]
las listas al ser un tipo de dato mutable, se pueden modificar en una funcion y no hace falta que la devuelva porque la lista original ya se modifico.
vease [[uso de memoria]] 
![[Pasted image 20250505191540.png]]

en este ejemplo, se modifica un elemento de la lista y se mantiene el ID

en los tipos de dato inmutable, se cambia el ID, porque se destruye el objeto anterior y se asigna una referencia nueva


### las listas se unen o concatenan con otras listas +=