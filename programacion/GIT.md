git es un tracker de versiones, o sea cambios en archivos

#### inicializar un repositorio local *repo*
``` 
your/repo/path
git init
```

un *repo* es un directorio el cual git va a supervisar para tener los cambios

### git add

add se utiliza para añadir archivos al repo, un archivo puede existir en el directorio pero no ser trackeado por git

```
git add . #. para trackear todos los archivos
git add archivo.py 
```
### Commit
los commit son snapshots de la version actual del codigo, esto funciona con vectores, no haciendo copias, es decir:

```
version1 -> cambios -> commit -> version 2 

git commit -m "mensaje" 
```

version 2 no tiene guardada una copia de version 1, solo tiene almacenados los cambios que se hicieron

*los mensajes deben ser  precisos y descriptivos * [[tipos de datos]] -> string

al hacer un commit se limpian los cambios y se guardan en el commit
se genera un *head* , que seria el commit mas reciente

##### good commit practices
- many small commits
	- se evitan perdidas grandes de codigo 


### Branch (es)
branch(es) o ramas, son versiones distintas de un repo a partir de cierto punto que tienen su propio historial de cambios

- #### master
	- es la rama principal de desarrollo, nombre default 

```
git branch name-of-the-branch
```

###### checkout
para cambiar de rama activa en el desarrollo

```
git checkout name-of-the-branch
git checkout master
```

### Merge
merge combina los cambios de una branch con la branch master, creando un nuevo *head*

```
git merge name-of-the-branch
```

### ignore
ignore se utiliza para que git no registre un archivo

```
git ignore archivo.txt
```