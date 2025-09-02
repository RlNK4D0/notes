#AySO 

el comando awk es casi un lenguaje de programacion en si mismo, con sus propias funciones

awk recorre las *COLUMNAS* de un archivo, por ej:

```
awk '{print $5}' path/to/file
```
va a imprimir la quinta columna de un archivo

sintaxis:

```
- Print the fifth column (a.k.a. field) in a space-separated file:
    awk '{print $5}' path/to/file

  - Print the second column of the lines containing "foo" in a space-separated file:
    awk '/foo/ {print $2}' path/to/file

  - Print the last column of each line in a file, using a comma (instead of space) as a field separator:
    awk -F ',' '{print $NF}' path/to/file

  - Sum the values in the first column of a file and print the total:
    awk '{s+=$1} END {print s}' path/to/file

  - Print every third line starting from the first line:
    awk 'NR%3==1' path/to/file
  - 
```

```
cat /etc/passwd | awk -F ':' '{print "USER: " $1 " UID: " $3 " GID: " $4 " HOME: " $6}' | grep vagrant

```
*cat* va a leer el archivo passwd
*awk* va a leer en la fila (-F) separando las columnas por ":" y va a imprimir la columna 1, 3, 4 y 6 
Los mensajes en el string de print deben ir con comillas dobles

[[grep]] va a agrupar los resultados por "vagrant"

