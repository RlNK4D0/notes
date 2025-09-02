los componentes basicos de toda red domestica son los modems, routers, switches, y wireless access points 

generalmente estos 4 dispositivos vienen integrados todo en uno 

# Modem
el modem es la puerta de acceso o salidao (gateaway) al internet, conectandose al *ISP* (internet service provider) 
los modems generalmente tienen 1 solo puerto Ethernet, por eso se necesitan mas dispositivos para una red domestica 

##### what it does ? 
- convirten señales de largo rango en señales de corto rango para ser utilizados por otros dispositivos. Las señales de corto rango son mas seguras y pueden ser utilizadas por electronicos mas baratos y simples 
- reformatea la informacion encriptada del ISP a un formato entendible por los dispositivos domesticos
- actua como un puente entre la conexion domestica y el ISP

##### tipos de modems
- **Cable modem**: se conecta al ISP por cable coaxial, envia y recibe señales electromagneticas a traves del cable (muy parecido a las señales de radio, pero en distintas frecuencias y forzada a traves de un cable en vez de ser transmitidas al aire. vease [[radio communications]])
- **DSL modem**: se conecta a travez de cable de par trenzado, de los que se usan para lineas telefonicas. Utiliza señales electromagneticas como el cable modem, pero en distintas frecuencias. *los cables telefonicos tipicamente tambien llevan electricidad para poder alimentar los telefonos, esto puede ser peligroso si el voltaje llega a ser alto*
- **Fiber Modem**: se conecta por cable de fibra-optica. Propiamente dicho, terminal de red optica / optical network terminal (ONT). Transmite luz (*fotones*). el cable esta hecho de fibras de silicio, las cuales son transparentes 
- **Cellular modem**: se conecta inalambricamente a la torre celular mas cercana. Es la misma tecnologia utilizada por un celular pero el ISP provee una cja parecida a un *DSL modem*, tipicamente se posicionan cerca de una ventana para mejor recepcion
- **Dialup modem**: se conecta por cable de par tranzado. utiliza un pequeño rango de señales electromagneticas que los telefonos utilizan para representar sonido

---

# Router
dirige el trafico de paquetes entre la red local domestica y el internet [[pfsense router]]

##### what it does? 
- permite tener mas dispositivos conectados a la red
- si se conecta un dipositivo directamente al modem, solamente ese dispotivo tendra acceso al internet, conectandose directamente a una *WAN*, en lugar de una *LAN*
- los routers crean una segunda red interna (*LAN*), para poder conectar mas de un dispositivo al internet
- dirigen el trafico dentro de la red local *LAN*, y el trafico entrante del internet *WAN*, al dispositivo correcto dentro de la red y a la vez el trafico entre los dispositivos dentro de la red local domestica
- NAT (network address translation): traducec las *IP's* privadas de los dispositivos en la *LAN*, a una sola *IP* publica provista por el *ISP*

# switch
un switch añade  puertos ethernet para dispositivos en tu red local *LAN*

##### what it does? 
- expande conectividad al proveer mas puertos para mas dispositivos, como un [[NAS - Network Attached Storage]]
- el switch sabe que dispositivo esta conectado a tal puerto por lo tanto puede redirigir el trafico de forma eficiente, a diferencia de un HUB

##### use case
se conectaria el puerto LAN del [[pfsense router]] a CUALQUIER puerto del switch 

##### virtual LAN support
no todos los switches soportan la creacion de VLANs, pero son muy utiles para crear una red de visitas o una red para dispositivos *IoT (internet of things ~~duck this shit~~)* que no sean confiables

# wireless access points
proveen accceso a la red a traves de WI-FI, inalambricamente, mayormente utilizada por dispositivos moviles

##### what it does? 
- provee conexion inalambrica al router o switch, al transmitir una señal WI-FI
- NO dirige trafico, solo añade los puertos inalambricos a la red

##### use case

los WAPs se pueden posicionar en distintas zonas de la casa para asegurar tener una buena señal conectandose con un cable [[Ethernet]] al router o switch
los WAPs generalmente funcionan de forma que reconectan tu dispositivo al WAP con mejor señal, es un proceso muy rapido y eficiente que no se nota que estas siendo reconectado
