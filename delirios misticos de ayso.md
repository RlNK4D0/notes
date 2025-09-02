
antes se compraba un servidor distinto para poder correr los nuevos programas
ahora se crea una [[virtual machines]] con todas las dependencias de la aplicacion que se utilizaron en el entorno de desarrollo

en caso de que se necesiten mas maquinas virtuales para sostener el servicio con todas las llamadas que se le hacen, se multiplica las vms con herramientas de despliegue de vms

docker es una de estas herramientas de despliegue, es distinto de una vm porque esto es contenedores
docker despliega contenedores los cuales contienen las dependencias para que la aplicacion funcione

docker traduce las rutas de forma automatica entre sistemas operativos
las varibles de entorno tambien, puertos tambien, usuarios y permisos


microservicio:
 microservicio se le llama a modularizar el programa de forma tal que cada programa se encargue de una parte distinta y que no se caiga todo el servicio si se satura
 con docker esto se puede escalar de forma tal que se puede hacer multiples instancias del microservicio
 