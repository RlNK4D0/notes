#programacion 

las funciones se usan para dividir un programa en partes mas chiquitas, las funciones cumplen una tarea especifica, solo hacen una cosa y nada mas

guidelines: [[cohesion y acoplamiento]]

minificacion: esto quiere decir que al usar funciones, el programa se vuelve mucho mas fácil y sencillo de leer

depuracion: las funciones hacen mas fácil poder debuggear un programa al poder ir directamente a la parte que se encarga de esa tarea que esta dando problema

modifcacion: 

reutilizacion: las funciones son re-utilizables, reducen las redundancias y tiempos de escritura

independencia: una función es independiente de otra, ya que cada función hace cada cosa 

```
def calcular_precio_con_iva():
	print("cosa)

```
se utiliza para *definir* una función 
las palabras print(), input(), len(), son funciones, el código para que estas funcionen esta integrado en el lenguaje python

las funciones después se llaman o invocan

```
calcular_precio_con_iva()

```

como resultado va a printear "cosa"
las funciones también reciben parámetros, cualquier función con paréntesis recibe parámetros o argumentos, son sinónimos

las variables declaradas en los parámetros se les llama variables *locales* de la función

```
#print()

  

#los nombres de las funciones se escriben en snake_case

#las funciones tienen que tener un verbo porque justamente hacen una accion en especifico

  

def calcular_precio_con_iva(precio, iva): #desarrollo de la funcion, firma

#variable LOCAL de la funcion son las que se declaran dentro de los parametros

	resultado = 2 * 3

	print

  
  
  
  

calcular_precio_con_iva(1000, 1.21) #llamada de la funcion|| 1000es el valor de la variable precio, y 1.21 del iva

```

las variables *locales* con el mismo nombre que las variables *globales*, van a tener prioridad las variables locales 

los paramertos en las funciones con valores literales, pueden ser pisados al asignarle los parametros a la llamada de la funcion por lo tanto se los llama *parametros opcionales*

las *entradas de datos* a las funciones, van a ser por parametros

#### return
```
solo se puede usar 
return()
```
dentro de funciones 
se utiliza para sacar un resultado de la funcion, es decir sacar un VALOR de la funcion hacia el programa MAIN 
el return tambien cumple la funcion de un brake [[break y continue]]

en tanto la funcion encuentre un return, va a romper la funcion, y no se ejecuta NADA que este por debajo, interrumpe y finaliza la funcion

es recomendable por ahora que solo se use return al final de la funcion


```
def sumar_enteros(num_a , num_b):

	suma = num_a + num_b
	
	return suma

  

num_a = int(input("numero a: "))

num_b = int(input("numero b: "))

  

resultado = sumar_enteros(num_a, num_b)

print(f"resultado A y B {resultado}")

num_c = int(input("numero c: "))

  

resultado = sumar_enteros(resultado , num_c)

  

print(f"resultado A+B y C: {resultado}")
```

esto es conveniente porque si en algún momento tengo que volver a sumar números, solamente voy a llamar a la función y lo va a hacer automáticamente 
no lo tengo que escribir de nuevo

es **MUY** buena practica en python definir el tipo de dato en la función 
```
def sumar_enteros(num_a:int|float , num_b:int|float) -> float:

```
de esta forma se dice al programador, que tipo de datos se esperan en la función y que tipo de dato va a retornar 

se puede validar los [[tipos de datos]] que se ingresan a la función de la siguiente manera [[Validaciones]]

parametros formales, son como se declaran los parametros
-> num_a, num_b son los parametros de esta funcion

```
def sumar_enteros(num_a:int|float , num_b:int|float) -> float:

```

parametros actuales

son los valores que toman los parametros al momento de llamar a la funcion
-> num_a = 5, num_b = 11

```
resultado = sumar_enteros(resultado , num_c)
```

parametros opcionales 
```
def calcular_precio_con_iva(precio, iva = 1.21)
```
el iva es un parametro opcional

en funciones se puede usar TODO, incluyendo [[match]], [[bucles anidados]] [[bucle for]], [[bucle while]], [[condicionales]], y se debe tener en cuenta el [[uso de memoria]]

