#AySO 


los grupos tienen un ID especifico y gestionan los permisos, un grupo puede tener 0 o mas usuarios 

**gID** 

los grupos se almaenan en
```
/etc/group
```

crear un grupo:

```
sudo groupadd group
```

crear un usuario y añadirlo a un grupo
```
sudo useradd -m -d /home/dev2 -c "dev2" -G developers dev2
```

-d definir nombre del home
-m para indicar que se cree un home para el usuario  
-c para agregar un comentario  
-s para indicar el interprete de comandos (bash/zsh/other)

añadir un usuario a un grupo
![[Pasted image 20250506205006.png]]
```
sudo usermod -aG developers dev2
```
a;adir al dev2 al grupo developers


????

![[Pasted image 20250506205515.png]]

se añade un usuario, -m indica la creacion de un home, -s para designarle el shell bash, -d para indicar que el usuario va a tener su home en /home/dev2, -c para un comentario, -G para designarle un grupo
