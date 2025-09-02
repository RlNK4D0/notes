#AySO 

los permisos se modifican con *CHMOD*
existen 3 permisos
r = read
w = write
x = e*x*ecute
```
chmod u +/- r / w / x
```
para sumar o restar permisos a un usuario

```
chmod g +/- r / w / x
```
lo mismo pero para el grupo

forma alternativa

```
chmod 777 file
```

primer numero para el usuario
segundo para el grupo
tercero para invitados

esto viene del binario
r-w-x = 111 = 7
r -w-  = 110 = 6
r -  -x = 101 = 5
r - -    = 100 = 4

