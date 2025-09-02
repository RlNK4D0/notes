#programacion 

validar un string para [[casting]] a int

```
def verificar_digito_numerico (valor:str) -> bool:

"""

documentacion

"""

retorno = True

for char in valor:

	# 0 -> 48 | 9 -> 57
	
	#8 -> 56 < 48 or 56 > 57
		
	if char < "0" or char > "9":
		
		retorno = False
		
		break

return retorno
```

en esta funcion no usamos las funciones de [[manipulacion de strings]] por restricciones de la clase

el if tiene un rango de solo los caracteres del 0 y el 9  en el codigo ascii
el string tiene de rango maximo los 256 caracteres del codigo ascii [[tipos de datos]]
