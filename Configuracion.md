
###### Universidad de San Carlos de Guatemala
###### Facultad de Ingeniería
###### Escuela de Ciencia y Sistemas
###### Redes de Computadoras 1
###### Nombre: Hayrton Omar Ixpatá Coloch
###### Carnet: 201313875

# Manual: Configuracion de Topología Practica 1
## 1. Topologia realizada
![Texto alternativo](/image/Topologia.JPG "Topologia")

## 2. Configuracion de Rauter c3725
  - Comandos utilizados
    - conf t
    - int f0/0  -> elegimos la interfaz a configurar
    - ip add {ip} {Mascara de subred}
    - no shut
    - exit
    - exit
    - sh ip int br -> Mostramos el estado de las interfaces
  - IP utilizadas en las interfaces
    - f0/0 -> ip: 192.168.13.1
    - f0/1 -> ip: 192.168.13.65
    - f1/0 -> ip: 192.168.13.129
    
![Texto alternativo](/image/conf_router.JPG "Rauter")

## 3. Configuracion de VPC
  - Comandos utilizados
    - ip {ip} {Mascara de subred} gateway {ip de interfaz}
    - sh ip -> Muestra la configuracion de red de la vpc
  - Ip Utilizada en host "Finanzas"
    - vpc1 -> ip: 192.168.13.2  gateway: 192.168.13.1
    - vpc2 -> ip: 192.168.13.3  gateway: 192.168.13.1
  - IP utilizadas en host "Ventas"
    - vpc3 -> ip: 192.168.13.100    gateway: 192.168.13.65
    - vpc4 -> ip: 192.168.13.110    gateway: 192.168.13.65
    - vpc5 -> ip: 192.168.13.120    gateway: 192.168.13.65
  - IP utilizadas en maquina virtual Linux
    - Linux -> ip: 192.168.13.150   gateway: 192.168.13.129
 
![Texto alternativo](/image/conf_vpcs.JPG "Vcp1")
  
  - Las subredes que fueron creadas tienen como submascara /26

### 4. Configuracion de maquina virtual linux

![Texto alternativo](/image/conf_linux.JPG "linux")
 
