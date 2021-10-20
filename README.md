## Creacion de un servidor Bind9 y Ubuntu

## Comandos usados:

## Maquina Ubuntu
### apt update --> actualizar todos los paquetes
### apt-get install -y iputils-ping --> para que ping funcione
### apt-get install iputils-tracepath --> este paquete instala tracepath 
### apt install net-tools --> necesario para poder usar ifconfig y route
### apt-get install -y ifupdown 
### apt-get install dnsutils -y --> isntala dig y dns commands
### apt-get install -y whois --> instalar el comando whois
### apt install -y curl --> permite descargar archivos desde 

## Maquina Bind
### apt-get install net-tools

## Con todo esto nuestra máquinas estan listas.

### Ahora debemos configurar nuestra resolv.conf de la máquina ubuntu 
### apt install nano --> editor de texto de ubuntu
#### Debemos modificarlo y escribir la ip de nuestra maquina bind
#### Luego simplemete hacemos dig www.google.com y al final el servidor que nos provee DNS deber ser la ip de nuestro bind

## ;; Query time: 1010 msec
## ;; SERVER: 172.21.0.3#53(172.21.0.3)
## ;; WHEN: Wed Oct 20 16:47:51 CEST 2021
## ;; MSG SIZE  rcvd: 87