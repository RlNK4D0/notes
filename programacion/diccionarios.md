#programacion 

[[tipos de datos]] -> dict -> mutables, iterables, NO indexables

se declaran con {} al igual que los [[sets]] 

pregunta de parcial, diferencia entre sets y diccionarios:
	->**los sets almacenan elementos como una lista, los diccionarios almacenan items**

```
diccionario = {item1,item2,item3}
```
no son elementos. los diccionarios se componen por ITEMS
->todos los items tienen 2 cosas:
	-> una clave: se utiliza para acceder al valor, las claves son *strings*, DEBE SER UNICA, NO se debe repetir en el mismo diccionario
		si existen 2 claves iguales, va a acceder a la ultima clave que se repita
		NO existe forma de acceder al valor de la primera clave repetida
	-----------------------------------------------------------------------------------
	->un valor: el valor del item : Any, puede repetirse el valor sin problema

NO se utilizan [[indices]] para acceder a un valor


pregunta de parcial:
	-> al imprimir un diccionario con print, imprime las { } vacías
	->en cambio el set lo imprime con ( ) vacíos

```
diccionario = { "string":"valor", "edad":36, "notas":[4,6]}
primer item: clave = str : valor = str
segundo item: clave = str : valor = int
tercer item: clave = str : valor = list
```

##### ejemplo: [[listas]] de diccionarios 

![[Pasted image 20250530201358.png]]

->los tipos de datos cambian y se leen distinto dependiendo donde esta 
(**PREGUNTA DE PARCIAL**)

```
lista[i] -> type: dict

lista[i]['notas'] -> type: list | el item con clave 'notas' tiene como                                       valor una lista

lista[i]['notas'][0] -> type: int | el valor dentro de la lista es un int
```

print diccionarios con [[métodos]]
valores:
![[Pasted image 20250530202510.png]]
claves:
![[Pasted image 20250530202039.png]]
devuelve los items en [[tuplas]]
![[Pasted image 20250530202359.png]]

update()
![[Pasted image 20250530204848.png]]
-> modifica los valores si la clave existe y añade un item si la clave no existe
ejemplo de ingreso de datos con metodo update()
![[Pasted image 20250530210208.png]]

