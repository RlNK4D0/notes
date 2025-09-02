#programacion 

las referencias es como se maneja la memoria en el programa [[uso de memoria]]

las [[Variables en python]] son etiquetas, referencias al objeto

al pasar un dato por valor, estamos pasando una copia del dato, NO la variable como tal

yo al pasar una variable con un valor,  como parametro, a una funcion, la funcion va a copiar y trabajar con esa copia dentro de la funcion. la variable ORIGINAL *NO* se modifica

al pasar un dato como referencia, se modifica directamente el [[objetos]] en memoria ( [[uso de memoria]]) 

los [[tipos de datos]] inmutables, bool, str, int, float, no se les puede modificar su valor 

las listas son tipos de datos mutables, que se modifican por referencia, se modifican en memoria 
[[funciones]]

los datos *inmutables* se pasan por parametros, por valor
los datos *mutables* se pasan por parametros, por referencia

cuando se trabaja con referencia en una funcion, se modifica el objeto original
cuando se trabaja con valor en una funcion, se modifica la copia dentro de la funcion

