#programacion 


la forma correcta de buscar un maximo y minimo es utilizando una bandera **flag = True | false**, la cual se ejecute en el primer ciclo del bucle, para que las variables que van a almacenar los maximos o minimos, tomen un valor base

las variables maximo y minimo van a tener como valor inicial *none*

y en el primer ciclo van a tomar el primer valor que se lea

```
#1) forma larga (vamos a usar este para poder aplicar en otros lenguajes)

#variable de bandera, es un concepto unicamente

if flag == True: # if i == 0: la diferencia es que la flag es un caso universal

	nombre_mejor_alumno = nombres
	
	notas_mejor_alumno = notas
	
	flag = False

#esta bandera, nos va a servir UNICAMENTE para tener un primer valor guardado con el cual comparar


```

y para encontrar valores maximos o minimos podemos dividirlo en el else del if de la bandera
[[condicionales]]

```
else: #comparacion de notas guardando tambien el nombre del alumno y la nueva nota maxima
	
	if notas > notas_mejor_alumno:
	
		nombre_mejor_alumno = nombres
		
		notas_mejor_alumno = notas
	
	else:
	
		if notas < notas_mejor_alumno:
		
			nombre_mejor_alumno = nombres
			
			notas_mejor_alumno = notas
			
```




----


