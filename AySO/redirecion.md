#AySO 
la redireccion se utiliza con **>**

para guardar el texto output de un comando como *cat* o [[wc contador de lineas]] en otro archivo

ej:
```
ps aux | grep user | wc -l > numero_de_procesos_usuario.txt
```

```
echo "hola mundo" > file.txt
```

`>>` añade los datos a un archivo en la ultima linea o modifica el archivo
