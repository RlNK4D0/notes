#programacion #juego 
los archivos son una coleccion de datos almacenados NO en RAM, sino en almacenamiento

existen los archivos de texto | TXT , [[CSV]] , [[JSON]] | 
	-> al abrirlos en un editor de texto podemos leer que contienen
	-> TXT y CSV se van a trabajar de forma algoritmica
	-> JSON se va a trabajar con [[métodos]]

los archivos binarios que no son legibles, imagenes, videos, pdf
	-> este tipo de archivos al abrirlos en un editor de texto, es totalmente illegible

abrir un archivo -> open( )
-> open( ) recibe 2 parametros: 
	->1er parámetro: la ruta del archivo o path (siempre como [[tipos de datos]] -> str)
		->puede ser absoluta o relativa (al proyecto), siempre la relativa
		-> por buena practica, se le va a cambiar las \ por / en la ruta
	->2do parametro: modo de apertura -> str
		-> 1er modo: "r" | read | lee un archivo
			->si el archivo no existe y lo abrimos con el modo "r" va a dar un error,      se debe manejar este error con el [[Try-Except-Finally]]
			-------------------------------------------------------------------------
		->2do modo: "w" | write | escribe un archivo
			->si el archivo SI existe: va a limpiar el archivo, borrando todo
				-> primero se debe abrir en modo lectura, extraer la informacion y      despues abrirlo con w
			->si no existe y lo abrimos con "w" va a crear el archivo
			->los archivos deben cerrarse, para esto se debe usar el metodo
			archivo.close( ) 
			-------------------------------------------------------------------------
		->3er modo: "a" | anexar | append (agrega datos al final del archivo)
			-> si el archivo existe, va a escribir al final del archivo sin borrar el                contenido anterior

```
#opcion 1)
archivo = open(ruta, "a")

#SE DEBE SI O SI CERRAR EL ARCHIVO

archivo.close()

#opcion 2)

#se debe guardar el retorno de open y entregarle un alias [[modulos]]

with open(ruta, "r") as archivo -> with tiene una estructura condicional
	datos = archivo.read()     -> devuevle todo el contenido del archivo                                      en formato str
	archivo.write("str")       -> agrega el str al archivo

lista = ["nombres"]
with open(ruta, "w") as archivo
	archivo.writelines( )      -> recibe un iterable y escribe linea por                                     linea en el archivo y a la vez va a                                        borrar el contenido del archivo por                                        estar en modo w
	
	archivo.readlines( )       -> devuelve una lista de lineas y cada                                        linea es un elemento
	

#no hace falta cerrar el archivo porque with lo cierra al terminar la tabulacion [[funciones]] [[condicionales]]

```
->[[modulos]]
->[[funciones]]
-> [[condicionales]]

los datos extraidos de los archivos deben ser NORMALIZADOS, LIMPIADOS y ORGANIZADOS



