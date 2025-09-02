#programacion 

es un concepto en el cual se intercambia los valores de 2 o mas variables

```
a = 5
b = 7
```
si se hace 
```
a = b
```
esto va a eliminar el 7 y ambas variables pasan a apuntar [[pointers]] al 5
[[uso de memoria]]

lo correcto seria utilizar una variable auxiliar

```
a = 5
b = 7

aux = a
#aux = 5
```
ahora tanto aux como a apuntan al objeto 5
y ahora al hacer:
```
a = b
# a = 7
b = aux
# b = 5
```

se intercambian los pointers porque aux ya guardaba el pointer original de a 

esto se denomina swap / intercambio
