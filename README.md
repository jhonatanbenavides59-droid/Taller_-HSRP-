# Taller HSRP

Para la actividad mencionada se pide recrear un laboratorio de manera física sobre el uso que tiene el protocolo HSRP que nos permite crear una redundancia entre 2 o 3 router Cisco creando un Gateway virtual para que en caso de que el router principal tenga una falla el router de respaldo suba de manera automática para que el servicio no presenta caídas, en el ejercicio planteado se pide configurar 3 router para que cada uno tenga una prioridad diferente y tener una mayor redundancia, pero por limitaciones físicas de los dispositivos que se tiene en el laboratorio solo se usaran dos router.

### Paso 1

Cambiar nombre de los router R1, R2 para poder identificar cual tiene la prioridad de cada uno y saber cuál es el activo y cual estará en standby


-	Comandos para cambio de nombre
  
<img width="655" height="561" alt="image" src="https://github.com/user-attachments/assets/117b68a4-a01a-40e3-8ff5-754238f1147c" />


### Paso 2
Crear la configuración de los segmentos virtuales y físicas al igual que asignar el protocolo HSRP a la interfaz que quiera usar para tal medio, como no se tiene un servidor que nos arroje un servicio de DHCP como en el ejercicio se configura una IP estática en la tarjeta física del equipo para poder realizar la simulación. 


-	Tabla de configuración IP
  
<img width="625" height="198" alt="image" src="https://github.com/user-attachments/assets/e021f612-27b6-4e27-aca6-167945eec6cd" />


- Configuración Gateway virtual con protocolo HSRP prioridad 150

 <img width="677" height="674" alt="image" src="https://github.com/user-attachments/assets/5149aeef-dad6-4e86-93ba-551adbd67a8e" />


- Configuración Gateway virtual con protocolo HSRP prioridad 100

<img width="725" height="442" alt="image" src="https://github.com/user-attachments/assets/efde7b6b-e69e-4145-b7a3-2c88ee6e83c8" />


- Configruacion de puerto físico bajo el segmento 192.168.1.254

<img width="869" height="541" alt="image" src="https://github.com/user-attachments/assets/5e5aaffc-3cf5-4bf3-8fdf-70f964ac32c4" />


- Protocolo HSRP funcionando donde el R1 estado en modo activo y el R2 estado modo standby

<img width="921" height="1105" alt="image" src="https://github.com/user-attachments/assets/97bfe6da-d9b3-4710-b9fb-fc79ea97ff6f" />


- Prueba de funcionamiento con el equipo local, que logre hacer ping a la red virtual.

<img width="472" height="440" alt="image" src="https://github.com/user-attachments/assets/b755dcbf-157f-486d-9a35-4edf74de6cc9" />




    



