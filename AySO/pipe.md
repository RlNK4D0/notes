#AySO 

el pipe es una cosa que recibe un output para darle como input a otro comando

por ej
```
ps -ef | wc
```

ps va a listar todos los procesos y [[wc contador de lineas]] va a tomar el output de ps para contar las lineas 

```
ps -ef (or aux) | wc -l
```
este comando por ej va a contar la cantidad de lineas (ps lista los procesos)
y de esta forma wc nos dice la cantidad total de procesos activos


pipe se puede utilizar mas de 1 vez por linea
![[Pasted image 20250429212631.png]]
esto es el resultado de preguntar por todos los procesos, se agrupan [[grep]] por usuario y luego se cuenta cuantos procesos son del usuario 
