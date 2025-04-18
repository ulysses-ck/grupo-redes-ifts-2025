# PROGRAMACIÓN SOBRE REDES

## TRABAJO PRACTICO TEORICO

## Programación sobre Redes

### Trabajo Practico Teórico

1- ¿Qué es una VLAN?

2- ¿Qué es una VPN?

3- ¿Qué es una SAN?

4- Diferencias entre un Hub, Repetidor, Router y SWITCH. Explicar las diferencias.

5- ¿Qué es un protocolo de comunicaciones?

6- Explique TCP/IP y NetBios, resuma sus diferencias. (Acá sí explicar cada uno y sus
diferencias)

7- ¿Cómo está formado un paquete de datos en TCP/IP? ¿Qué es un “flag” en un
paquete de TCP/IP?

8- Defina la red según su geografía. Explicar distintas variantes.

9- Defina una red según su topología. Explicar distintas variantes.

10- Explicar el servicio de DHCP.

11- Explicar el servicio de DNS.

12- Explicar las tecnologías Wireless, y sus estándares.

13- ¿Qué es un Proxy?

14- Explicar el protocolo Spanning tree.

15- Explicar el protocolo de comunicaciones OSPF.

16- Explicar el protocolo ARP.

17- ¿Qué es un Firewall?

18- ¿Qué es una DMZ?

19- ¿Qué es un Gateway?

20- Según Microsoft, ¿qué significa NBL?


21- Tipos de enlace: MPLS, LAN to LAN, microonda, VSAT. a. Explique cada uno de estos
tipos de enlace. b. Agregue dos tipos de enlaces, no mencionados anteriormente. c.
Ranking de enlaces según lo pedido (de uno a seis, siendo uno el mejor): Por
económico, performance, mayor capacidad, mayor o mejor configuración de
restricciones, soporte a mayor distancia, menor esfuerzo de configuración. d. Elija un
tipo de enlace para los siguientes escenarios: 1 d. Conectividad de varios de call centers
con un data center central. 2 d. Conectar los datos de los pozos petroleros durante 15
minutos por día. 3 d. Comunicar dos edificios enfrentados en la misma calle.

22- Describir la tecnología LTE.

23- Explique la solución de Microsoft Teams. Si quieren describir otra solución de otra
empresa es también válido.

24- ¿Qué significa aplicar calidad en un enlace MPLS?

25- ¿Qué diferencias puede encontrar entre una conexión Coaxial, UTP o Fibra?

26- Según Cisco, ¿qué significa CCENT, CCNA y CCNP? Descripción breve del Track
Routing & Switching y de algún otro a elección (ej. Wireless, Security, Cloud, etc).

27- Explique el modelo OSI.

28- Realizar cuestionario online y copiar el resultado: (1 por cada integrante)
https://es.educaplay.com/es/recursoseducativos/706834/test_de_redes_y_comunicacion
es.htm (OPCIONAL)

29- Explicar el estándar IEEE 802.3 regula la red. Cómo se implementa, ventajas y
desventajas.

30- Explicar el estándar IEEE 802.4 regula la red.

31- ¿Qué protocolos se usan para enviar y recibir correo?

32- ¿Qué protocolo puede usarse para leer correo recibido?

33- Diferencias entre IPV4 e IPV

34- (Individual para cada integrante del grupo) ¿Qué experiencia tienen en redes?
Ejemplos.: Accedo y configuro el router de mi casa como admin, en mi trabajo hago
tareas relacionadas a networking, configuro una PAN hogareña para mi o mi familia,
amigos/as etc (Personal Area Network, todo dispositivo Wireless o no), no tengo
ninguna experiencia, etc.


## Desarrollo


**1- ¿Qué es una VLAN?**
VLAN (Virtual Local Area Network) es una red lógica que se crea dentro de una red física, lo
que permite segmentar la red en grupos y asi poder reducir trafico innecesario, mejorar el
rendimiento y la seguridad, y tambien poder aislar dispositivos según su función o ubicación  

**2- ¿Qué es una VPN?**
Se trata de una red privada virtual(VPN, Virtual Private Network), la cual te permite utilizar
una IP diferente, frente a las páginas webs, servidores, etc; a la que se asigna
habitualmente a traves del servicio de proveedor de Internet(ISP, Internet Service Provider).
Existen diferentes empresas que ofrecen esto, como ser Proton, GhostVPN, SurfShark, etc.
En IT se utiliza generalmente para el trabajo remoto.  

**3- ¿Qué es una SAN?**
Una red de área de almacenamiento(Storage Area Network) es una red especializada para
acceder a dispositivos de almacenamiento.Estas están comúnmente compuesta de Hosts,
Switches y de elementos de almacenamiento interconectadas entre sí usando una gran
variedad de topologías y protocolos.

**4- Diferencias entre un Hub, Repetidor, Router y SWITCH. Explicar las diferencias.**
Hub:Conectar varios dispositivos en una red y transmitir los datos a todos ellos, su uso común es en redes pequeñas. No distingue a dónde va la información, envía todo a todos

Repetidor: Regenerar y amplificar una señal, su uso común es para extender el alcance de una red. No tiene capacidad para filtrar, dirigir o interpretar datos

Router: Conectar diferentes redes entre sí, su uso común es para proveer acceso a Internet. Decide la mejor ruta para enviar los datos basándose en direcciones IP  

Switch: Conectar dispositivos en una red local y enviar los datos solo al destinatario correcto, Su uso común es en redes domésticas o de oficina. Aprende las direcciones MAC y mejora el rendimiento de la red

**5- ¿Qué es un protocolo de comunicaciones?**
Es un conjunto de reglas, que al respetarse permite que las redes puedan "hablar en el mismo idioma" y comunicarse entre sí. Un protocolo define restricciones, procedimientos y formatos que definen el intercambio de paquetes para lograr la comunicación entre 2 o más servidores.

**6. TCP/IP y NetBIOS: Definición y diferencias**
- TCP/IP (Transmission Control Protocol/Internet Protocol) es un conjunto de protocolos que permite la comunicación entre dispositivos en redes, incluyendo internet. Ofrece confiabilidad, corrección de errores y direccionamiento a través de direcciones IP.

- NetBIOS (Network Basic Input/Output System) es una interfaz de comunicación utilizada en redes locales (LAN) para permitir la conexión entre equipos sin necesidad de direcciones IP, usando nombres de dispositivos.

- Diferencias: TCP/IP es más robusto y escalable, funcionando en redes grandes, mientras que NetBIOS es más limitado y suele utilizarse en redes pequeñas sin enrutamiento externo.

**7. Estructura de un paquete TCP/IP y los "flags"**
- Un paquete TCP/IP consta de varias capas:
- Capa de enlace de datos: Encabezado con dirección MAC.
- Capa de red: Encabezado con dirección IP origen y destino.
- Capa de transporte: Encabezado TCP o UDP con puertos de origen/destino.
- Capa de aplicación: Datos de la comunicación (HTTP, FTP, etc.).

- Flags en TCP: Son indicadores en el encabezado que controlan el estado de la conexión, como SYN (inicio de conexión), ACK (confirmación) y FIN (cierre de conexión).

**8. Tipos de redes según la geografía Las redes pueden clasificarse por su alcance geográfico:**
- PAN (Personal Area Network): Para dispositivos personales, como Bluetooth.
- LAN (Local Area Network): Redes pequeñas, como las de hogares o empresas.
- MAN (Metropolitan Area Network): Conectan ciudades o áreas grandes.
- WAN (Wide Area Network): Redes globales, como internet.

**9. Tipos de redes según la topología Las redes también se clasifican por su estructura de conexión:**
- Red en estrella: Dispositivos conectados a un nodo central.
- Red en bus: Todos los dispositivos comparten un único canal de comunicación.
- Red en anillo: Cada dispositivo está conectado con el siguiente, formando un círculo.
- Red en malla: Cada dispositivo tiene múltiples conexiones, ofreciendo redundancia.

**10- Explicar el servicio de DHCP.**
Un servicio de DHCP es el cual se utiliza para asignar una IP a un dispositivo. Sin esta, se necesitaría asignar una IP estática como 192.168.1.X manualmente.

**13- ¿Qué es un Proxy?**
Un proxy se trata de un servidor que recibe las peticiones de un usuario y este las traslada a otro servidor. Una VPN también funciona como un servidor proxy, solamente que está toma todo el tráfico entrante de un usuario, en vez de solamente algunas peticiones.

**19- ¿Qué es un Gateway?**
Una gateway o puerta de enlace es el dispositivo que conecta distintas redes. Su propósito es traducir la información del protocolo utilizado en una red de origen al protocolo usado en la red de destino. Si un dispositivo dentro de una red quiere comunicarse con otro que está fuera de esa misma red, se necesita una gateway. Hoy en día es muy común que las gateways se combinen con los enrutadores, por lo que muchas veces se puede hablar de una gateway refiriéndose a un enrutador. Un ejemplo muy común de esta combinación es el router que te instalan cuando contratás un servicio de internet en tu casa: este utiliza una gateway para conectar los dispositivos de la red local con redes externas, como internet.

**31- ¿Qué protocolos se usan para enviar y recibir correo?**
Los protocolos que se usan para enviar y recibir correo son: SMTP(Simple Mail Transfer Protocol), POP3(Post Office Protocol Version 3)

**32- ¿Qué protocolo puede usarse para leer correo recibido?** 
El protocolo que puede usarse para leer correo recibido es el POP3

**34- (Individual para cada integrante del grupo) ¿Qué experiencia tienen en redes?**
Ulises: He configurado una aplicación para producción usando Nginx, creando un subdominio en los registros de DNS con un CNAME y asignando los Certificados con Let's Encrypt.
