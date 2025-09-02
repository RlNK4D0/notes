#AySO 

linux es un SO multiusuario con diferentes permisos si es necesario 

TODOS los usuarios tienen un userID
```
vagrant:x:1000:1000:,,,:/home/vagrant:/bin/bash
```
el usuario vagrant tiene contrase;a encriptada, userID 1000, groupID 1000
3tel usuario tiene una carpeta de usuario en home /home/vagrant
y su shell es /bin/bash

tipos de usuarios: 

root: todos los permisos posibles, es el *superuser* del sistema, ID 0
```
root:x:0:0:root:/root:/bin/bash
```
x: contrase;a encriptada o no, x es encriptada
primer 0: userID
segundo 0: group userID
/bin/bash: shell del usuario (bin es la carpeta de binarios y ejecutables)

todos los usuarios se almacenan en 

```
/etc/passwd
```

las contraseñas se almacenan en :

```
/etc/shadow
```

los usuarios se pueden crear on el comando 

```
sudo useradd -m -c 'user'
```

-d definir nombre del home
-m para indicar que se cree un home para el usuario 
-c para agregar un omentario 
-s para indicar el interprete de comandos (bash/zsh/other)

cambiar de usuario:

```
su user

password:
```
nos va a pedir la contrase;a del usuario

como borrar un usuario 
```
sudo userdel -r user
```

añadir contraseña al usuario 

```
sudo passwd user
```
