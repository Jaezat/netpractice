# Wtf is subnetting?

## IP adresses

- Phone number for each device.
- It opens up communication.
- ex: IPv4 address: 4 set of numbers, 4 "octets" 32 bits, 8 bits = 1 octet.
- why most of the ip adresse start with 192.168.1? 


## Subnet mask

- 255.255.255.0
- also 4 octets
- if we have the octects 255 that means that the numbers in our IP adress will always stay the same in our network.
- so if we have this ip adress:
	```192.168.1
- and the mask for it is:
	```255.255.255.0``` -> that means that the first three octets will never change. 
- on that sense, when we have a 0, that means that the number will change
- Basically the last number since is the "host" number it will change depending of what device is assigned to.

#### Ok but what is the mask actually for?
- Basicamente el masks sirve para entender que parte es el network portion y que parte es el host portion.
- Para saber que parte es el street en donde se vive y que parte es la casa en donde viok exve


#### Why do we have to know the network portion of the IP address?
- El network portion of the IP adress es como la calle en donde viven los Ip adresses
- En una area en donde estan todos conectados por el mismo router es muy propable que los ip addresses de los devices tengan el mismo network portion, pero el host cambie (el ultimo octet que pertenece digamos al numero de casa)
- Pero que pasa si queremos enviar algo a un Ip adress que no esta en la misma calle y que tiene el netowrk portion totalmente diferente del nuestro?
	- Lo que pasa en este caso es que no podemos conectar directamente con el device, al contrario de cuando tenemos devices que se comunican entre ellos porque estan en el mismo LAN (Local Area Network)
	- De esta manera tienen que pasar a traves del Router (Default Gateway).
- En el ultimo octet hay hasta 256 posibilidades conexion incluyendo 0, pero lo que no se dice/muestra es que hay dos IP addresses que estan reservados, que no puedo tocar y no puedo usar.
- el primero es mi propio IP adress so:
	- De todas las posibilidades, 192.168.1.0, este IP address nunca puedo tocar. 
	- El segundo es: 192.168.1.255 este numero siempre esta reservado para el broadcast.
		- El broadcast sirve para compartir abiertamente la informacion
	- El tercero, es el router que guardamos tambien el espacio, asi que quiere decir que en realidad tenemos 253 espacios y no 256 




