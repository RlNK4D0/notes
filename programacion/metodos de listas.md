#programacion 

[[métodos]] aplicados a listas

->append()
```
lista.append("hola")
lista_nombres ["juan","ana","matias"]
print *ambas listas*

```
a la *lista* se le va a añadir al final un objeto string "hola", lo concatena 
	-> [[cadenas de caracteres]]
a la *lista_nombres* no se le va a;adir nada ya que no se le aplica ningun metodo


->clear()

```
lista [5,3,2,7]
lista_nombres ["juan","ana","matias"]

lista.clear()

resultado 
	lista = []
	lista_nombres = [todos sus elementos normal]
```
-> clear borra los elementos de la lista 

->copy()
```
lista [5,3,2,7]
lista_nombres ["juan","ana","matias"]

lista_copia = lista.copy()

```

-> copia una lista [[listas]] | shallow copy con su propio ID
	se debe guardar esta copia 

->.deepcopy()
```
import copy
copia_matriz = copy.deepcopy()
```

-> [[matrices]] -> deepcopy()

->.count()
```
lista.count(valor) <- valor = elemento a contar
```

-> va a contar cuantas veces aparece el valor en la lista

->.extend()
```
lista = [nombres]
lsita2 = [99,205,105]
lista.extend(lista2)

resultado
lista = [nombres, 99,205,105]
------------------------------------------------------------------

lista2.extend(lista)

resultado 
lista = [99,205,105 , nombres]
```
-> va a concatenar 2 listas 
	el id de la lista resultante va a ser el ID de la lista a la cual se le aplica el metodo [[uso de memoria]]

->.index() [[indices]]
```
lista.index(valor , 3) <- el segundo parametro es el indice desde el cual inicia a buscar | DESDE el indice 3


```

-> devuelve el primer indice con ese valor, es decir que si tenemos una lista con varias ocurrencias de ese elemento, solo va a devolver el primer indice 

-> si el valor no esta presente en la lista devuelve un error y corta el programa
	ValueError:  [[Try-Except-Finally]]
	

-> .insert()
```
lista.insert(4, 100) <- primer parametro indice, segundo valor
```

-> inserta un valor en el indice determinado, no sobreescribe el elemento que tenia el indice, sino que mueve el resto de elementos para acomodar el elemento en ese indice
-> si se inserta en un indice que no existe, lo inserta igual aunque de indice le des un 15.000

-> .pop()
```
lista.pop(indice)
```

-> elimina un elemento en el indice indicado y devuelve el elemento eliminado 
	si existen 2 elementos con el mismo valor , se elimina la ultima ocurrencia por default

->.remove()
```
lista.remove(valor)
```
-> borra la primera ocurrencia de el elemento y no lo devuelve

-> .reverse()
```
lista.reverse()
```
-> da vuelta la lista, ultimo elemento pasa a ser el primero y asi sucesivamente 

->.sort()
```
lista.sort()
```
-> ordena la lista ascendente-mente por default
	-> reverse: parámetro | bool
		reverse = true: ordena descendente-mente

