#programacion 

el break, en un bucle, apenas sea leido por el interprete, va a romper el bucle mas cercano?

```
for num in range(10):
	if num == 3
		continue 
	print num
	if num == 7 
		break




resultado :


0 al 7, se ignora el 8 al 9

imprime el 7 porque el range llega hasta 7 y rompe el bucle 

```

continue, corta el bucle, y vuelve a iterar la en el proximo continue, ignora todo lo que sigue en esa iteracion, es decir todo lo que este por debajo del continue

en el caso del continue, el resultado va a ser 0 al 2, y despues desde el 4 al 7, el valor 3 no se va a imprimir porque el continue esta arriba del print

