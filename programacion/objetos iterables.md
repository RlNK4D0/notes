#programacion 

objeto iterable, todo objeto que se pueda leer con la funcion **len()** es iterable
es decir **strings**
porque guardan MAS de un valor a la vez, por lo tanto en los strings hay varios valores, como caracter 1, caracter 2, 3 , 4 etc 

los **STRINGS** son objetos iterables

**range** es una funcion que nos va a crear una serie de valores enteros, los cuales nos va a permitir iterar con el for, creando un [[objetos iterables]] , 

**tambien** una vez el interprete llega a la linea donde se escribe el range, el range es lo primero que se resuelve, se genera el objeto iterable, despues se ejecuta el bucle 

la funcion *len()* devuelve un entero, por lo tanto en un bucle 
```
for i in range(len(alumnos))
```
devuelve un valor entero, para la cantidad de iteraciones que va a tener el bucle for

en programaion **SIEMPRE** se empieza a contar desde 0
si la lista tiene 3 elementos, el [[indices]] va a ser 0,1,2 


