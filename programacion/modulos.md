#programacion 

los modulos deben estar siempre en el mismo directorio 
los modulos se deben **IMPORTAR** con un comando import, siempre al inicio del main 

los import se deben hacer en el modulo donde se van a utilizar, por ej: 
importo random en funciones en vez de en main.py

tambien si tengo que usar validate.py
puedo importar validate en funciones.py 

y en main importar SOLO funciones.py

se compone por el programa main.py
```
# Programa Principal (Main)
# Un poco de logica (bucle, menu, mensajes, variables, prints, invocaciones de funciones)
# import random
# print(random.randint(1, 5))


# 1°
# import funciones
# resultado = funciones.sumar(3, 4)
# print(resultado)
# resultado = funciones.es_numero_entero("Hola")
# print(resultado)

# 2° 
# from funciones import * # * -> Importamos todo
# resultado = sumar(3, 2)
# print(resultado)

# 3°
# from funciones import sumar, restar # Importar una o mas funciones especificas
# resultado = sumar(3, 2)
# print(resultado)
# resultado = restar(3, 2)
# print(resultado)

# 4° 
import funciones as f # Alias -> ponerle un nombre mas corto o identificativo al modulo
import random as r
#import test_prueba as t # Con guion bajo, SIN ESPACIOS!!
# t.test()
# "Hola".center() # Metodo ! NO LO PUEDEN UTILIZAR

# f.sumar()
# f.restar() # NO es un METODO, es un modulo con funciones 
# f.es_numero_entero()

# Programa principal

# pedir las edades de 5 estudiantes y sus notas del primer examen

bandera = False

for alumno in range(5):
    # Entrada de datos
    edad = f.validar_numero_entero("Ingrese la edad (13-17): ", 13, 17)
    nota = f.validar_numero_entero("Ingrese la nota (1-10): ", 1, 10)
	
    # Logica
	
    # Salida de datos

   ========================================================================
```
estas son 3 formas distintas de importar modulos

de esta forma estoy importando mi modulo de funciones en el mismo directorio 

con la logica basica y funcional para que las funciones puedan trabajar.
en el main se van a almacenar generalmente constantes [[tipos de datos]]


y el programa funciones.py
```
def sumar (a, b):
	return a + b

```
donde se definirán todas las [[funciones]] , Y NADA MAS, ningún dato suelto, variable, etc NADA suelto
