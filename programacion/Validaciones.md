#programacion 

# para validar siempre se usa un bucle while
[[bucle while]]


```
password = input ("password")

while password != "password":
	password = input ("incorrect password")
print("bienvenido")


```
para validar un rango de edad
```
edad = 0

while edad < 18 or edad > 125:

	edad = int(input("ingrese su edad (18-125)"))

  

print ("edad validada" , edad)

```
de esta forma si se ingresa una edad mayor a 125 o menor a 18, el programa se estanca en el bucle while

al inicializar la variable ``edad`` en 0, forzamos al programa a entrar al bucle, es valido tambien preguntar primero antes de entrar al bucle 
```
edad = input("ingrese la edad ")
```
la alternativa para strings es inicializar la variable con un string vacio
```
string = ""
```
para validar datos, se debe **INCUMPLIR** la condicion

```
art_ingresado = ""

while art_ingresado != "Jabon" and art_ingresado != "Barbijo" and art_ingresado != "Shampoo" :

	art_ingresado = input(" ingrese el articulo de nuevo: ")

print (f"compraste {art_ingresado}")

```
es decir, los valores ingresados deben ser **DISTINTOS** de los valores validos

tambien para validar rangos de numeros, se valida poniendo un limite (18 en este caso) hacia el -infinito **O** 125 hacia + infinito

para validar tipos de datos para ejecutar una [[funciones]] se puede escribir 

```
while type(variable) == int or type(variable) == float
	reingresar o ejecutar funcion 
```


[[validacion de string para castear a int]]

