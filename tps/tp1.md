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

7- ¿Cómo está formado un paquete de datos en TCP/IP? ¿Qué es un "flag" en un
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

33- Diferencias entre IPV4 e IPV6

34- (Individual para cada integrante del grupo) ¿Qué experiencia tienen en redes?
Ejemplos.: Accedo y configuro el router de mi casa como admin, en mi trabajo hago
tareas relacionadas a networking, configuro una PAN hogareña para mi o mi familia,
amigos/as etc (Personal Area Network, todo dispositivo Wireless o no), no tengo
ninguna experiencia, etc.


## Desarrollo


# 🌐 **1- ¿Qué es una VLAN?**
**VLAN** (Virtual Local Area Network) es una red lógica que se crea dentro de una red física. Permite segmentar la red en grupos, lo que ayuda a:
- **Reducir tráfico innecesario** 🚦
- **Mejorar el rendimiento** ⚡
- **Aumentar la seguridad** 🔒
- **Aislar dispositivos** según su función o ubicación 🏢

```mermaid
graph TD
    Switch[Switch Principal]
    PC1[PC Marketing]
    PC2[PC Marketing]
    PC3[PC Finanzas]
    PC4[PC Finanzas]
    Server1[Servidor Marketing]
    Server2[Servidor Finanzas]

    Switch --- PC1
    Switch --- PC2
    Switch --- PC3
    Switch --- PC4
    Switch --- Server1
    Switch --- Server2

    subgraph VLAN 10 - Marketing
        PC1
        PC2
        Server1
    end

    subgraph VLAN 20 - Finanzas
        PC3
        PC4
        Server2
    end

    classDef vlan10 fill:#FF4444,stroke:#000000,stroke-width:2px,color:#FFFFFF
    classDef vlan20 fill:#44AA44,stroke:#000000,stroke-width:2px,color:#FFFFFF
    class PC1,PC2,Server1 vlan10
    class PC3,PC4,Server2 vlan20
```

---

# 🔒**2- ¿Qué es una VPN?**
Una **VPN** (Virtual Private Network) te permite utilizar una IP diferente frente a páginas web, servidores, etc. Esto se logra a través del servicio de un proveedor de Internet (ISP). Algunas empresas que ofrecen este servicio son:
- **Proton**
- **GhostVPN**
- **SurfShark**

En IT, se utiliza generalmente para el **trabajo remoto** 🏠.

---

# 💾 **3- ¿Qué es una SAN?**
Una **SAN** (Storage Area Network) es una red especializada para acceder a dispositivos de almacenamiento. Comúnmente está compuesta de:
- **Hosts**
- **Switches**
- **Elementos de almacenamiento** interconectados usando diversas topologías y protocolos.

---

# 🔄 **4- Diferencias entre un Hub, Repetidor, Router y SWITCH. Explicar las diferencias.**
- **Hub**: Conecta varios dispositivos en una red y transmite datos a todos ellos. No distingue a dónde va la información, envía todo a todos. 🖥️
  
- **Repetidor**: Regenera y amplifica una señal. Se usa para extender el alcance de una red, pero no filtra ni dirige datos. 📡

- **Router**: Conecta diferentes redes entre sí y provee acceso a Internet. Decide la mejor ruta para enviar datos basándose en direcciones IP. 🌍

- **Switch**: Conecta dispositivos en una red local y envía datos solo al destinatario correcto. Aprende direcciones MAC y mejora el rendimiento de la red. ⚙️

```mermaid
graph LR
    Internet((Internet))
    Router[Router]
    Switch[Switch]
    Hub[Hub]
    Repeater[Repeater]
    PC1[PC 1]
    PC2[PC 2]
    PC3[PC 3]
    PC4[PC 4]

    Internet --- Router
    Router --- Switch
    Switch --- PC1
    Switch --- PC2
    Hub --- PC3
    Hub --- PC4
    Repeater --- Hub
```

---
# 📜 **5- ¿Qué es un protocolo de comunicaciones?**
Es un conjunto de reglas que permite que las redes "hablen en el mismo idioma" y se comuniquen entre sí. Un protocolo define:
- **Restricciones**
- **Procedimientos**
- **Formatos** para el intercambio de paquetes.

---

# 📦 **6. TCP/IP y NetBIOS: Definición y diferencias**
- **TCP/IP** (Transmission Control Protocol/Internet Protocol) es un conjunto de protocolos que permite la comunicación entre dispositivos en redes, incluyendo Internet. Ofrece:
  - **Confiabilidad** ✅
  - **Corrección de errores** 🛠️
  - **Direccionamiento** a través de direcciones IP 🌍

- **NetBIOS** (Network Basic Input/Output System) es una interfaz de comunicación utilizada en redes locales (LAN) para permitir la conexión entre equipos sin necesidad de direcciones IP, usando nombres de dispositivos. 🖥️

- **Diferencias**: 
  - **TCP/IP** es más robusto y escalable, funcionando en redes grandes. 
  - **NetBIOS** es más limitado y suele utilizarse en redes pequeñas sin enrutamiento externo. 

---

# 📦 **7. Estructura de un paquete TCP/IP y los "flags"**
Un paquete TCP/IP está estructurado en encabezados IP y TCP, que contienen información como direcciones IP, puertos, números de secuencia y flags.

- **Encabezado IP** (Protocolo IP - Capa de Red): 
  - Proporciona las direcciones de origen y destino, así como información sobre cómo debe ser manejado el paquete en la red. 
  - Este encabezado es crucial para los routers, ya que les permite tomar decisiones basadas en la información contenida en él. 📬

- **Encabezado TCP**: 
  - Contiene detalles como los puertos de origen y destino, el número de secuencia y la suma de verificación hash. 
  - Básicamente se encarga de dividir los datos en partes más pequeñas, numerarlas y asegurarse de que lleguen completas y en orden. 📦

- **Flags**: 
  - Son indicadores en el encabezado que controlan el estado de la conexión, como:
    - **SYN** (inicio de conexión) 🔄
    - **ACK** (confirmación) ✅
    - **FIN** (cierre de conexión) ❌

---
# 🌍 **8. Tipos de redes según la geografía Las redes pueden clasificarse por su alcance geográfico:**
Las redes pueden clasificarse por su alcance geográfico:
- **PAN** (Personal Area Network): Para dispositivos personales, como Bluetooth. 📱
- **LAN** (Local Area Network): Redes pequeñas, como las de hogares o empresas. 🏠
- **MAN** (Metropolitan Area Network): Conectan ciudades o áreas grandes. 🌆
- **WAN** (Wide Area Network): Redes globales, como Internet. 🌐

---

# 🔗 **9. Tipos de redes según la topología Las redes también se clasifican por su estructura de conexión:**
Las redes también se clasifican por su estructura de conexión:
- **Red en estrella**: Dispositivos conectados a un nodo central. ⭐
- **Red en bus**: Todos los dispositivos comparten un único canal de comunicación. 🚌
- **Red en anillo**: Cada dispositivo está conectado con el siguiente, formando un círculo. 🔵
- **Red en malla**: Cada dispositivo tiene múltiples conexiones, ofreciendo redundancia. 🔗

```mermaid
graph TD
    subgraph Star Topology
        S_Central((Central))
        S_Node1[Node 1]
        S_Node2[Node 2]
        S_Node3[Node 3]
        S_Central --- S_Node1
        S_Central --- S_Node2
        S_Central --- S_Node3
    end

    subgraph Ring Topology
        R_Node1[Node 1]
        R_Node2[Node 2]
        R_Node3[Node 3]
        R_Node4[Node 4]
        R_Node1 --- R_Node2
        R_Node2 --- R_Node3
        R_Node3 --- R_Node4
        R_Node4 --- R_Node1
    end
```

---
# 📡 **10- Explicar el servicio de DHCP.**
Un servicio de **DHCP** es el cual se utiliza para asignar una IP a un dispositivo. Sin esta, se necesitaría asignar una IP estática como 192.168.1.X manualmente.

# 🌐 **11- Explicar el servicio de DNS.**
El **DNS** (Sistema de Nombres de Dominio) traduce los nombres de dominios aptos para lectura humana (por ejemplo, www.amazon.com) a direcciones IP aptas para lectura por parte de máquinas (por ejemplo, 192.0.2.44). 
Esto permite a los usuarios acceder a sitios web utilizando nombres fáciles de recordar, en lugar de tener que recordar direcciones IP numéricas. 🌍

sequenceDiagram
    participant Client
    participant DNS
    participant Website
    Client->>DNS: Query: www.example.com
    DNS->>Client: Response: 93.184.216.34
    Client->>Website: HTTP Request

---
# 📡 **12- Explicar las tecnologías Wireless, y sus estándares.**
"**Wireless**", o comunicación inalámbrica, describe la transmisión de datos entre dispositivos utilizando ondas de radio u otras ondas electromagnéticas, eliminando por completo la necesidad de cables para la comunicación de los mismos.

### Estándares:
- **IEEE 802.11**: Estándar para redes de área local inalámbricas (WLAN), conocido como **Wi-Fi**. Permite la conexión de dispositivos dentro de un área limitada, como hogares u oficinas, usando ondas de radio en las bandas de 2.4 GHz y 5 GHz, y en versiones más recientes también 6 GHz (Wi-Fi 6E). 📶

- **IEEE 802.15**: Estándar para redes de área personal inalámbricas (WPAN). Incluye tecnologías como **Bluetooth**, que permite la comunicación entre dispositivos personales mediante un proceso de emparejamiento, con un alcance típico entre 1 y 100 metros, y **ZigBee**, usada en aplicaciones de bajo consumo como domótica e IoT. 🔗

- **IEEE 802.16**: Estándar para redes metropolitanas inalámbricas (WMAN), conocido como **WiMAX** (Interoperabilidad Mundial para Acceso por Microondas). Utiliza una topología punto a multipunto para ofrecer acceso de banda ancha inalámbrico sobre grandes distancias, ideal para zonas rurales o sin infraestructura cableada. 🌆

- **GSM** (Sistema Global para Comunicaciones Móviles): Estándar de comunicaciones móviles de segunda generación (2G). Incluye especificaciones de la capa física que permiten la implementación del protocolo **GPRS** (Servicio General de Radio por Paquetes) para la transmisión de datos sobre redes de telefonía celular. 📱

---

# 🔄 **13- ¿Qué es un Proxy?**
Un **proxy** es un servidor que recibe las peticiones de un usuario y las traslada a otro servidor. Una **VPN** también funciona como un servidor proxy, pero toma todo el tráfico entrante de un usuario, en vez de solamente algunas peticiones. 🔍

---
# 🌉 **14- Explicar el protocolo Spanning tree.**
El **Spanning Tree Protocol (STP)** es un protocolo de red de capa 2 (Enlace de Datos) que evita la formación de tramas duplicadas al detectar y bloquear automáticamente caminos redundantes que puedan generar bucles en una red de switches. 
STP asegura que haya un único camino activo entre dos dispositivos de red, creando una topología lógica libre de bucles (spanning tree), mientras mantiene la redundancia física disponible para recuperación ante fallos. 🔄

---
# 🛣️ **15- Explicar el protocolo de comunicaciones OSPF.**
El protocolo **OSPF** (Open Shortest Path First) es un tipo de enrutamiento que ayuda a encontrar el mejor camino para que los datos viajen por una red. 
Para hacerlo, detecta cómo están conectados los routers cercanos, comparte esa información con ellos y, si hay varias rutas posibles hacia un destino, elige la más rápida o conveniente según ciertas reglas. 
Además, si la red cambia, OSPF actualiza las rutas automáticamente para que los datos siempre tomen el mejor camino disponible. 🚀

---
# 🔗 **16- Explicar el protocolo ARP.**
El protocolo **ARP** (Address Resolution Protocol) es un sistema que ayuda a conectar las direcciones IP, que pueden cambiar, con las direcciones físicas fijas de los dispositivos en una red local (LAN). 
Básicamente, convierte una dirección IP en la dirección **MAC** de un dispositivo para que los datos puedan llegar a su destino correctamente dentro de la red. 📡

---

# 🔥 **17- ¿Qué es un Firewall?**
Un **firewall** es una herramienta de seguridad que controla qué datos pueden entrar o salir de una red o computadora. 
Actúa como una especie de "puerta" o "filtro" entre tu red y el resto de Internet, permitiendo solo el tráfico autorizado y bloqueando el que puede ser peligroso. 🔒

```mermaid
graph LR
    Internet((Internet))
    Firewall1{External Firewall}
    Firewall2{Internal Firewall}
    DMZ[DMZ]
    Internal[Internal Network]
    WebServer[Web Server]
    MailServer[Mail Server]

    Internet --- Firewall1
    Firewall1 --- DMZ
    DMZ --- WebServer
    DMZ --- MailServer
    Firewall1 --- Firewall2
    Firewall2 --- Internal

    classDef secure fill:#44AA44,stroke:#000000,stroke-width:2px,color:#FFFFFF
    classDef danger fill:#FF4444,stroke:#000000,stroke-width:2px,color:#FFFFFF
    class Internet danger
    class Internal,WebServer,MailServer secure
```

---
# 🛡️ **18- ¿Qué es una DMZ?**
Una **DMZ (Zona Desmilitarizada)** en un área separada dentro de una red donde se colocan los servidores que deben ser accesibles desde Internet, como páginas web o correos electrónicos, pero sin dar acceso directo a la red interna principal. Funciona como una zona intermedia de seguridad: si alguien intenta atacar desde afuera, solo llega a la DMZ y no a los sistemas más importantes de la red interna.

---

# 🌉 **19- ¿Qué es un Gateway?**
Una **gateway** o puerta de enlace es el dispositivo que conecta distintas redes. Su propósito es traducir la información del protocolo utilizado en una red de origen al protocolo usado en la red de destino. 
Si un dispositivo dentro de una red quiere comunicarse con otro que está fuera de esa misma red, se necesita una gateway. 

Hoy en día, es muy común que las gateways se combinen con los enrutadores, por lo que muchas veces se puede hablar de una gateway refiriéndose a un enrutador. 
Un ejemplo muy común de esta combinación es el router que te instalan cuando contratás un servicio de internet en tu casa: este utiliza una gateway para conectar los dispositivos de la red local con redes externas, como Internet. 🌐

---

# ⚖️ **20- Según Microsoft, ¿qué significa NLB?**
**NLB** significa **Network Load Balancing** o en español, **equilibrio de carga de red**. 
Es una función de Windows Server que sirve para distribuir y equilibrar el tráfico de red entre varios servidores como si fueran uno solo, mejorando así la **disponibilidad** y la **escalabilidad**. 📈

---
# 📶 **22- Describir la tecnología LTE.**
**Long Term Evolution (LTE)** es un estándar de comunicación inalámbrica de cuarta generación (4G) que ofrece:
- **Velocidades de datos más rápidas** y menor latencia que tecnologías anteriores como 3G, siendo entre 5 y 10 veces más rápido que 3G. ⚡
- Puede alcanzar hasta **100 Mbps de descarga** y **50 Mbps de carga**. 
- Está basada en el protocolo IP, lo que facilita la transmisión de datos, voz y video de forma más eficiente, en lugar de utilizar sistemas de conmutación por circuitos como en generaciones anteriores (3G y 2G). 📱

Además, tiene soporte de voz (**VoLTE**), lo que mejora la calidad de las llamadas de voz y permite realizar llamadas y navegar por Internet de manera simultánea. 
LTE fue fundamental para el avance de la tecnología móvil, ya que no solo permite un acceso más rápido a Internet, sino que también soporta aplicaciones avanzadas como **streaming**, **realidad aumentada** e **IoT**. También facilita la transición hacia la tecnología **5G**. 🚀

---

# 💬 **23- Explique la solución de Microsoft Teams. Si quieren describir otra solución de otra empresa es también válido**
**Microsoft Teams** es una plataforma para la comunicación y colaboración entre personas de un mismo equipo, empresa u organización. 
Es una aplicación de mensajería que combina:
- **Chat persistente** en el lugar de trabajo
- **Videoconferencias**
- **Almacenamiento de archivos**
- **Integración de aplicaciones** 📂

Otra solución sería **Slack**, que es una plataforma de comunicación y colaboración para equipos basada en canales. Permite a las personas conectar, compartir información y colaborar en proyectos. 🔗

---

# 📊 **24- ¿Qué significa aplicar calidad en un enlace MPLS?**
Aplicar calidad significa definir y garantizar un nivel de tráfico suficiente y aplicar mecanismos para asegurar que el tráfico de la red se transmita de forma eficiente. 
Esto se hace mediante **QoS** (Quality of Service). 

De esta manera, clasificás el tráfico, priorizás lo que necesita menor latencia, reservás una parte mínima de ancho de banda para ciertos tipos de tráfico crítico, aplicás políticas para evitar saturaciones y se usan técnicas para manejar el retardo y la pérdida de paquetes. 
Eso es aplicar calidad en un enlace MPLS, y todo esto sirve para mejorar la experiencia del usuario, garantizar el funcionamiento de servicios críticos y optimizar el uso del enlace MPLS. 📈

---

# 🔌 **25- ¿Qué diferencias puede encontrar entre una conexión Coaxial, UTP o Fibra?**
### Coaxial
- **Velocidad**: Hasta 1 Gbps.
- **Alcance**: Medio. A medida que el tramo se alarga, se pierde calidad y velocidad.
- **Interferencias**: Resistente a interferencias externas.
- **Costo**: Medio.
- **Uso principal**: Aún se utiliza bastante para televisión por cable, servicios de internet y redes telefónicas interurbanas. 📺

### UTP
- **Velocidad**: Hasta 40 Gbps en categoría Cat8.
- **Alcance**: Bajo. Para alcanzar los 40 Gbps (Cat8), el tramo debe ser de hasta 15 metros como máximo.
- **Interferencias**: Más vulnerable a interferencias electromagnéticas.
- **Costo**: Bajo.
- **Uso principal**: Muy utilizado en redes LAN, conexiones telefónicas y sistemas de cámaras de seguridad.

### Fibra
- **Velocidad**: Puede alcanzar velocidades del orden de los Tbps.
- **Alcance**: Alto. Permite transmitir datos a varios kilómetros sin pérdidas significativas.
- **Interferencias**: Inmune a interferencias electromagnéticas (transmite mediante luz, no electricidad).
- **Costo**: Alto, aunque tiende a reducirse con el tiempo.
- **Uso principal**: Se emplea en cables submarinos, sistemas de audio óptico y para ofrecer internet de alta velocidad tanto en hogares como en empresas. 

---

# 📜 **26- Según Cisco, ¿qué significa CCENT, CCNA y CCNP? Descripción breve del Track Routing & Switching y de  algún otro a elección (ej. Wireless, Security, Cloud, etc).**

- **CCENT** (Cisco Certified Entry Networking Technician): Certificación de entrada que valida habilidades para instalar, operar y solucionar problemas en pequeñas redes empresariales, incluyendo seguridad básica. 🛠️

- **CCNA** (Cisco Certified Network Associate): Certificación de nivel asociado que valida la capacidad de gestionar redes enrutadas y conmutadas de tamaño mediano, incluyendo conexiones WAN. 🌐

- **CCNP** (Cisco Certified Network Professional): Certificación profesional que valida conocimientos avanzados en planificación, implementación y solución de problemas en redes empresariales complejas. 📈

### Track Routing & Switching
El track de **Routing & Switching** (Enrutamiento y Conmutación) era la base fundamental de las certificaciones Cisco, centrado en tecnologías y protocolos para redes cableadas. Los profesionales deben demostrar habilidades en:
- Manejo de direcciones IP (IPv4 e IPv6) y subredes. 🌍
- Configuración y solución de problemas en routers y switches Cisco. 🔧
- Creación y gestión de VLANs para segmentar redes y mejorar seguridad. 🔒

### Track Wireless
El track de **Wireless** (Inalámbrico) está enfocado en diseño, implementación y solución de problemas en redes inalámbricas. 
Los profesionales deben ser capaces de:
- Comprender tecnologías Wi-Fi (IEEE 802.11) y sus estándares. 📶
- Implementar métodos de autenticación y seguridad (como WPA2/3). 🔐
- Solucionar problemas de cobertura, interferencia y rendimiento en redes inalámbricas. 📡

---

# 🌐 **27- Explique el modelo OSI.**
El **Modelo OSI** (Open Systems Interconnection) es un marco de referencia que estandariza las funciones de comunicación en redes de computadoras en **siete capas**, facilitando la interconexión entre diferentes sistemas. 

Las capas son:

1. **Capa Física**: Transmite datos en forma de bits a través de medios físicos. 🔌
2. **Capa de Enlace de Datos**: Proporciona la transferencia de datos entre nodos en la misma red y maneja errores de transmisión. 📡
3. **Capa de Red**: Se encarga del enrutamiento de datos entre diferentes redes y gestiona direcciones IP. 🌍
4. **Capa de Transporte**: Asegura la entrega confiable de datos y controla el flujo y la segmentación. 📦
5. **Capa de Sesión**: Establece, gestiona y termina sesiones de comunicación entre aplicaciones. 🔄
6. **Capa de Presentación**: Traduce y formatea los datos para la capa de aplicación, asegurando que sean comprensibles. 🖥️
7. **Capa de Aplicación**: Proporciona servicios de red a las aplicaciones del usuario final, como correo electrónico y navegación web. 📧

```mermaid
graph TB
    A["Capa 7. Aplicación"]
    B["Capa 6. Presentación"]
    C["Capa 5. Sesión"]
    D["Capa 4. Transporte"]
    E["Capa 3. Red"]
    F["Capa 2. Enlace"]
    G["Capa 1. Física"]
    
    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G

    style A fill:#2d3436,stroke:#636e72,stroke-width:2px,color:#fff
    style B fill:#2d3436,stroke:#636e72,stroke-width:2px,color:#fff
    style C fill:#2d3436,stroke:#636e72,stroke-width:2px,color:#fff
    style D fill:#0984e3,stroke:#74b9ff,stroke-width:2px,color:#fff
    style E fill:#0984e3,stroke:#74b9ff,stroke-width:2px,color:#fff
    style F fill:#00b894,stroke:#55efc4,stroke-width:2px,color:#fff
    style G fill:#00b894,stroke:#55efc4,stroke-width:2px,color:#fff
```

---
# 📡 **29- Explicar el estándar IEEE 802.3 regula la red. Cómo se implementa, ventajas y desventajas.**
**IEEE 802.3**: Es un estándar que regula las redes **Ethernet**, definiendo las especificaciones para la transmisión de datos en redes de área local (LAN) mediante cables.

### Implementación
Se implementa a través de dispositivos como switches y routers que utilizan cables de par trenzado o fibra óptica para conectar computadoras y otros dispositivos en una red. 🔗

### Ventajas
- **Alta velocidad**: Soporta velocidades de hasta **100 Gbps** en versiones avanzadas. ⚡
- **Estandarización**: Amplia aceptación y compatibilidad entre diferentes fabricantes. 🤝
- **Costo-efectividad**: Los componentes de Ethernet son generalmente más económicos y fáciles de obtener. 💵

### Desventajas
- **Alcance limitado**: La distancia máxima para cables de par trenzado es de **100 metros**, lo que puede ser una limitación en grandes instalaciones. 📏
- **Interferencias**: Puede ser susceptible a interferencias electromagnéticas
- **Colisiones**: En redes más antiguas, el uso de CSMA/CD puede llevar a colisiones de datos, aunque esto disminuyo con el uso de switches.


# 📡 **30- Explicar el estándar IEEE 802.4 regula la red.**
El estándar **IEEE 802.4** regula las redes de área local (LAN) utilizando un **método de acceso por token bus**. 
Se implementa mediante un sistema de **token** que permite a los dispositivos en la red tomar turnos para transmitir datos, evitando colisiones. 
Este enfoque se basa en un **cable coaxial** como medio de transmisión. 🔗

---
# 📧 **31- ¿Qué protocolos se usan para enviar y recibir correo?**
Los protocolos que se usan para enviar y recibir correo son:
- **SMTP** (Simple Mail Transfer Protocol) para el envío de correos. 📤
- **POP3** (Post Office Protocol Version 3) para la recepción de correos. 📥

---
# 📬 **32- ¿Qué protocolo puede usarse para leer correo recibido?** 
El protocolo que puede usarse para leer correo recibido es el **POP3**. 📧

---
# 🌐 **33- Diferencias entre IPV4 e IPV6**
### **IPV4:**
- **Lanzamiento**: 1981
- **Tamaño de direcciones**: 32 bits
- **Formato de la IP**: Notación decimal con puntos (ej: 192.168.0.1)
- **Cantidad de IPs**: 2³² = 4 mil millones
- **Tamaño de paquete mínimo requerido**: 576 bytes
- **Configuración**: DHCP o manual
- **Observaciones**: Se reutilizan direcciones IP. Tiene rangos reservados para uso privado, loopback, broadcast y red. 🔄

### **IPV6:**
- **Lanzamiento**: 1999
- **Tamaño de direcciones**: 128 bits
- **Formato de la IP**: Notación hexadecimal, separada por dos puntos (ej: 2001:0db8:85a3::8a2e:0370:7334)
- **Cantidad de IPs**: 2¹²⁸ = 340 undecillones
- **Tamaño de paquete mínimo requerido**: 1.280 bytes
- **Configuración**: Permite configuración automática sin necesidad de DHCP
- **Observaciones**: Está diseñado para que nunca falten direcciones. Cada persona podría tener trillones de IPs sin problema. 🌌

```mermaid
graph LR
    subgraph IPv4
        IPv4_Header[32 bits header]
        IPv4_Addr["192.168.1.1"]
    end

    subgraph IPv6
        IPv6_Header[128 bits header]
        IPv6_Addr["2001:0db8:85a3::8a2e:0370:7334"]
    end
```

---

# 👥 **34- (Individual para cada integrante del grupo) ¿Qué experiencia tienen en redes?**
**Ulises**: He configurado una aplicación para producción usando Nginx, creando un subdominio en los registros de DNS con un CNAME y asignando los Certificados con Let's Encrypt.

**Nicolas**: Configuré varios repetidores de manera inalámbrica y hace poco conecté un repetidor mediante cable Ethernet que tuve que configurar el repetidor para que no asignara direcciones IP, sino que las asignara solo el router principal. Recientemente, ingresé al panel de configuración de mi router para cambiar la contraseña.

**Agustin**: trabaje configurando router y switch en un curso de redes y participe en un tendido de fibra optica. 
