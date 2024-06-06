# Ejercicio CyberKillChain - Defensa

Alumno: Luis Gabriel Rueda Yarlequé

## Enunciado

Desarrollar la defensa en función del ataque planteado en orden inverso. No es una respuesta a un incidente, hay que detectar el ataque independientemente de la etapa.

Para cada etapa elegir una sola defensa, la más importante, considerar recursos limitados.

## Resolución

* Actions on Objectives
  - Realizar copias de seguridad regulares y almacenarlas de forma externa para garantizar la disponibilidad de los datos en caso de un ataque. [M1053 - Data Backup](https://attack.mitre.org/mitigations/M1053/)
 
* Command & Control
  - Implementar soluciones de seguridad de red que monitoreen y bloqueen el tráfico de red malicioso, filtrar las solicitudes DNS a dominios y recursos desconocidos. [M1037 - Filter Network Traffic](https://attack.mitre.org/mitigations/M1037/)
 
* Installation
  - Limitar los permisos para la modificación y/o creación de servicios en systemd, solo se reserva esta acción usuario root y usuarios con privilegios de administración. [M1026 - Privileged Account Management](https://attack.mitre.org/mitigations/M1026/)
 
* Exploit
  - Utilizar herramientas de detección de intrusos para detectar intentos de explotación de vulnerabilidades y bloquearlos automáticamente. [M1031 - Network Intrusion Prevention](https://attack.mitre.org/mitigations/M1031/)
 
* Delivery
  - Implementar soluciones de filtrado de correo electrónico para detectar y bloquear correos electrónicos de phishing. [M1054 - Software Configuration](https://attack.mitre.org/mitigations/M1054/)
  - Entrenar a los usuarios contra el phishing para detectar y no caer en phishing. [M1017 - User Training](https://attack.mitre.org/mitigations/M1017/)
 
* Weaponization
  - Mantener los sistemas, firmware, software y bases de datos actualizados con los últimos parches de seguridad para mitigar las vulnerabilidades conocidas. [M1051 - Update Software](https://attack.mitre.org/mitigations/M1051/)
    
* Reconnaissance
  - Implementar controles de acceso adecuados para limitar la cantidad de información sensible disponible públicamente. [M1056 - Pre-compromise](https://attack.mitre.org/mitigations/M1056/)










