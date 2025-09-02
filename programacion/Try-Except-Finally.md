#programacion #juego
(Try-Catch-Finally en otros lenguajes)
se utiliza para manejar errores 

es una estructura [[condicionales]]

es preferible utilizar [[funciones]] propias u otros metodos antes que utilizar esta estructura

```
try : #intentamos ejecutar algo que puede producir un error 
	indice = lista.index(3)
	 
except(ValueError): #cuando se produce un error  <- catch en otros   programas
	print("error, pero no explota el programa")
	 
except(ZeroDivisionError):
	print("mensaje")
	 
finally: #se hace siempre
	print("esto se ejecuta siempre")
	
```

los prints son ejemplos, se puede ejecutar cualquier cosa dentro de cada condicion

-> Try:
	cuando se produce un error en el bloque Try, hace un break y salta directo al bloque except

-> except:
	se ejecuta unicamente cuando en el bloque try se produce un error
	----------------------------------------------------------------------------------
	except puede recibir parametros en el cual espera un tipo de error y podemos ejecutar distintos bloques de codigo dependiendo del tipo de error dentro del parametro
	[[funciones]] 
-> Finally:
	funciona como un else, es opcional ponerlo o no, pero si existe el finally, se ejecuta SIEMPRE



