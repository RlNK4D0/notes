#programacion 

python tiene una función condicional llamada [^1]elif, que se escribe en la misma tabulacion que el if y else, en otros lenguajes de programacion no existe el elif, por lo tanto seria mejor aprender a **ANIDAR** if y else de la siguiente manera

otro condicional [[match]]

```
	if condicion:
		proceso
	else:
		if condicion:
			proceso
		else:
			if condicion:
				proceso
			else:

```

cuando se trabajen con condicionales, y estos preguntan sobre un rango de datos, por ej: si necesitamos ejecutar distintos bloques de codigo en un rango de datos como altura. Si tenemos que ejecutar un bloque de codigo si el dato es de 160cm o menos, 180 o menos, etc. seria buena idea evitar redundancias

Es decir:
```
	if altura > 160
		codigo
	else:
		if altura > 180
			codigo
		else:
			if altura > 200:
				codigo
			else:
			
```
de esta forma se descarta el rango menor a 160, y se ejecuta el else, tambien se descarta el rango de 180 si es el caso

 ---   |   ---  |   --- | 
    160     180     200

tambien es buena practica reducir la redundancia de preguntar si la persona es mayor a 200cm, si por logica ya sabemos que si 




[^1]: elif puede existir en otros lenguajes, tal vez con otro nombre como else if, pero siguen recomendando aprender anidacion
