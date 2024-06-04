# Ejercicio CiberKillChain - Ataque

Alumno: Luis Gabriel Rueda Yarlequé

## Sistema víctima

El sistema víctima es un sistema de estacionamiento itinerario inteligente, el cual mejorar la gestión de estacionamientos en la ciudad Lima, utilizando tecnología IoT, sensores de ultrasonido, nodos de comunicación ESP32 y una plataforma en la nube de AWS para proporcionar información en tiempo real sobre la disponibilidad de estacionamientos y gestionar los límites de tiempo de estacionamiento. 

El objetivo principal es facilitar la vida de los conductores en la ciudad, al ayudarles a encontrar estacionamientos disponibles de manera más eficiente y evitar multas por exceder los límites de tiempo permitido.

![Diagrama de bloques](Diag_bloques.png)


## Cyberkillchain

Armar una cyberkillchain usando técnicas de la matriz de Att&ck para un escenario relacionado al trabajo práctico de la carrera.

### Objetivo del ataque

El atacante es una organización criminal que antes de la implementación de este sistema de estacionamiento itinerario inteligente controlaban los estacionamientos, cobrando a los usuarios por el uso de los estacionamientos y el cuidado de los automoviles; cuando se implemento el sistema de estacionamiento itinerario se puso mas seguridad en los estacionamientos, por lo cual, ya no pueden operar.

El atacante se ha asesorado y busca sabotear el sistema de estacionamiento itinerario con la finalidad de que los usuarios vean inutil el sistema y a traves de reclamos se de la baja del sistema y los estacionamientos se continuen manejando por esta organización criminal.

### Ataque

* Reconnaissance
  - Recopilar información sobre la arquitectura, componentes, protocolos de comunicación y flujo de datos del sistema. [T1592 - Gather Victim Host Information](https://attack.mitre.org/techniques/T1592/)

* Weaponization
  - Desarrollar herramientas y códigos maliciosos para interceptar y modificar los datos enviados por los sensores/nodos ESP32. [T1587.001 - Develop Capabilities: Malware](https://attack.mitre.org/techniques/T1587/001/))
  -------------------------------------------------------------------
* Delivery
  - Obtener acceso físico a los nodos ESP32 o puntos de acceso en la red mediante ingeniería social. T1557 - https://attack.mitre.org/techniques/T1556/
  
* Exploit
  - Explotar vulnerabilidades en los protocolos de comunicación o en la configuración de seguridad de los nodos ESP32 o la red. [T1190 - Exploit Public-Facing Application](https://attack.mitre.org/techniques/T1190/)
  
* Installation  
  - Instalar herramientas de interceptación y manipulación de tráfico en los puntos de acceso comprometidos. 
[T1556 - Modify Authentication Process](https://attack.mitre.org/techniques/T1556/)
  - Configurar reglas o scripts para modificar los datos. T1600 - Proxy Malicioso

* Command & Control
  - Establecer un canal de comunicación encubierto con los puntos de acceso comprometidos. T1573 - Protocolo de Red Encubierto
  - Utilizar técnicas como canales encubiertos, túneles inversos o redes de comando y control. T1572 - Comunicación Encubierta entre Hosts
  
* Actions on Objectives
  - Interceptar y modificar los datos enviados por los sensores/nodos ESP32 sobre la disponibilidad de estacionamientos o los límites de tiempo permitidos. T1499 - Sabotaje de Datos
  - Inyectar información falsa o engañosa para mostrar estacionamientos disponibles o tiempos límite incorrectos. T1565 - Inyección de Datos Manipulados
  - Eliminar rastros de la actividad maliciosa, como el borrado de registros de eventos o archivos temporales. T1070 - Borrado de Credenciales
