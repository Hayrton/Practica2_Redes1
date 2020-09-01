###### Universidad de San Carlos de Guatemala
###### Facultad de Ingeniería
###### Escuela de Ciencia y Sistemas
###### Redes de Computadoras 1
###### Nombre: Hayrton Omar Ixpatá Coloch
###### Carnet: 201313875

# Manual de Reportes
  - Calculo de los dominios de Brodcast y de los dominios de colicion
    - #### HUB
      - Dominios de Colicion 1
      - Dominios de Broadcast 1
    - #### SWITCH
      - Dominios de Colicion n (n = numero de puertos conectados )
      - Cominio de Broadcast 1
    - #### ROUTER
      - Dominio de Colicion 1
      - Dominio de Broadcast 1 por cada interface conectada
      
![Texto alternativo](/image/calculo.JPG "DC_DB")

  - Captura de Paquetes
    - Se realiza un ping extendido a un dispositivo conectado a la red
      - ip origen: 192.168.13.150
      - ip destino: 192.168.13.3
      
![Texto alternativo](/image/ping_vpc1.JPG "ping_extendido")

  - En GNS3 se debera de buscar un punto por el cual podremos capturar los paquetes, y pulsar sobre el circulo verde de la interfaz, precionando
    donde dice inicar captura, el cual nos abrira una ventana del programa Wireshark, nos mostrara los paquetes que se encuentran pasando por el
    dispositivo indicado, filtraremos los paquetes por icmp.
 
 ![Texto alternativo](/image/captura_paquete.JPG "paquetes")

      
