#programacion 

# por cada valor en este objeto, itero


porque existe el bucle **for**:
	el bucle while esta pensado para una cantidad de iteraciones indeterminadas, en cambio el bucle **for** esta pensado para una cantidad de iteraciones **determinada**

[[objetos iterables]], todo objeto que se pueda leer con la funcion **len()** es iterable
es decir **strings**
porque guardan MAS de un valor a la vez, por lo tanto en los strings hay varios valores, como caracter 1, caracter 2, 3 , 4 etc 

el bucle for itera SOBRE objetos, la cantidad de bucles depende la CANTIDAD de valores que almacene la variable convirtiendola en un objeto iterable

```
var = "string"

print ( len(var))

contador_for = 0

for caracter in var:

	#code

	print("\n" ,caracter)

	contador_for += 1

  

print("\n", contador_for)


```


el bucle for **SOLO** puede iterar strings (objetos iterables) [[tipos de datos]]

```
range(5) -> [0, 1, 2, 3, 4] 
```

**range** es una funcion que nos va a crear una serie de valores enteros, los cuales nos va a permitir iterar con el for, creando un [[objetos iterables]] , 

*tambien* una vez el interprete llega a la linea donde se escribe el range, el range es lo primero que se resuelve, se genera el objeto iterable, despues se ejecuta el bucle 


```
  

rango = range(5)

print(rango)

print(type(rango))

print(list(rango))

  

for num in rango:

	print(num)

```

**resultado**:

```
range(0, 5)
<class 'range'>
[0, 1, 2, 3, 4]
0
1
2
3
4
```

itera las 5 veces que le dimos al range


CUANDO usamos WHILE y CUANDO FOR?

**si no conocemos la cantidad de iteraciones, se usa WHILE, si sabemos cuantas iteraciones, se usa FOR**

el bucle for en python, siempre inicia en 0 y va dando pasos de 1 en 1 por default, se puede cambiar este comportamiento:
```
#los parametros en range indican un HASTA, o sea, en este caso, excluye el valor 10

  

for i in range(10):

	print (i)

	#print (i + 1)

  

#Range con DOS parametros, primer valor es DESDE (incluye) y el segundo valor es HASTA (lo exluye)

  

for num in range( 3 , 8 ):

	#de 3 a 7
	
	print(num)

  

#range con TRES parametros, primer y segundo parametro no cambian su funcion, el tercer parametro es el PASO, de cuanto en cuanto, 2 en 2 , 3 en 3, etc

for valor in range(8 , 20 , 2):
	
	print(valor)

#el paso tambien puede ser negativo, -2 por ej

```

---

el bucle for each, solo puede tener el valor, no el indice

```
for num in lista:
	print (num)
```

for in range > for each

buscar el indice de un valor en la lista
![[Pasted image 20250425204446.png]]

