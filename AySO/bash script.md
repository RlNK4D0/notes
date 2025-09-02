#AySO 

```
echo "string" $(ps aux | grep rin | wc -l) > info.txt
```
resultado:

![[Pasted image 20250429213026.png]]

`>` es utilizado para escribir en un archivo
`>>` añade los datos a un archivo

```
cat passwd | echo "cantidad de usuarios: $(wc -l)" > /home/vagrant/cantidad_usuarios.txt
```
ejemplo de leer el contenido de un archivo (passwd) [[pipe]] 
echo "str $(wc -l )" 

el $ quiere decir [[shell]], el *$(wc -l)* quiere decir comando de shell, que lo ejecuta dentro del string [[tipos de datos]]

los scripts son instrucciones que resuelven tareas repetitivas que tienen que ver con el shell 

y se deben guardar en un archivo .sh

```
bash_script.sh
```

dentro del archivo se van a guardar instrucciones como

```
cp -r dir backup/dir
sudo pacman -Syu

```
luego se ejecuta solo el archivo 
```
bash_script.sh
```
y ejecutara las instrucciones de adentro