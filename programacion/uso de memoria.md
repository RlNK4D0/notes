#programacion 

el interprete reconoce que existe una [[funciones]] propia, nada mas, no lee el código de dentro de la función, ni parámetros

cuando el interprete llega a la invocación / llamada de la función 

la memoria se divide en memoria *stack* y en memoria *heap*
los [[objetos]] se guardan en la memoria *heap* / montón 

el *stack* guarda el ID del [[objetos]], guarda las funciones propias 

al llamar a una función, se almacena en el *stack* 

el interprete al llamar a la función, toma los parámetros y ejecuta la función hasta terminar de resolver la función 

las funciones propias y las funciones del lenguaje (como el print) se apilan en el *stack*
una vez que la función anidada,en este caso el print, termina de ejecutarse, se elimina del *stack*
 una vez que la función invocada por nosotros termina, también se des-apila como el print

```
resultado = funcion()
```

el resultado va a tomar el resultado de la funcion desde el *heap*, esto se llama **referencia**
un [[pointers]] 
en el caso de los booleanos, al ser solo 2 tipos de datos, se guardan en el *heap* y se reutilizan 

dentro de las [[funciones]] , si el valor original de un objeto cambia, se crea otro objeto con el nuevo valor, y el objeto original ahora tiene de [[referencias]] el objeto nuevo
pero tambien los objetos creados dentro de las funciones, desaparecen una vez que dejan de ser utilizados 
por lo tanto si el valor original es 5, dentro de la función cambia a 6, y al salir de la funcion, en el programa main, se vuelve a imprimir el valor original, va a seguir siendo 5, porque la funcion trabaja con una **copia**


![[Pasted image 20250421223104.png]]


## listas en memoria

[[listas]]

![[Pasted image 20250425202636.png]]

el objeto de la lista, en python reserva los lugares de memoria para guardar n cantidad de elementos

y estos elementos son objetos independientes
por lo tanto la lista guarda otros objetos

![[Pasted image 20250505192639.png]]


---

matrices en memoria

la etiqueta matriz se guarda en el stack y almacena la referencia del un objeto lista, el [[tipos de datos]] de una matriz es *list*

el [[indices]] de una matriz se refiere NO a los elementos, sino a las listas que almacena

```

matriz = [ [1, 2], [3,4] ]

```
en este caso el indice 0 es 1 y 2 y el indice 1 es 3 y 4

los elementros de las listas dentro de la matriz tambien almacenan objetos de forma independiente, con su propio ID, tipo de dato y valor

![[Pasted image 20250505193318.png]]

