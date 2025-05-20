# Resumen de Tecnologías relevantes

## De 1G a 5G

### 1G
La primera generación del estándar de conectividad apareció en 1980 y permitía solamente llamadas de voz a distancias cortas.
La tecnología 1G operaba a una frecuencia de 800 MHz y proporcionaba una velocidad de transmisión de datos de solo 2,4 Kbps. A pesar de esto, 1G es un hito importante en el desarrollo de las redes de telecomunicaciones.

### 2G
La segunda generación de las comunicaciones estándar aparecieron en 1991: esta fue la primera tecnología digital que permitió no solo llamadas de voz sino también SMS.
2G opera en la banda de 900 MHz con tasas de datos de hasta 64 Kbps.Este estándar de comunicación dio origen a GSM y CDMA, que todavía están en uso en algunas partes del mundo hoy.

### 3G

El estándar 3G se introdujo en 2001 y permitió la transmisión de datos a velocidades más altas que 2G. La tecnología 3G opera en la banda de 2,1 GHz y tiene un ancho de banda de hasta 2 Mbps.
3G dio a los operadores móviles la capacidad de ofrecer una gama más amplia de servicios, como mensajería multimedia, videollamadas y acceso a Internet en dispositivos móviles.

### 4G

4G, también conocido como LTE, se introdujo en 2009 y ofrecía velocidades de datos más altas, una gama más amplia de servicios y conectividad confiable.
4G opera en la banda de frecuencia de 2,6 GHz y proporciona un ancho de banda de hasta 100 Mbps. Con esta tecnología, los operadores móviles pueden proporcionar a los usuarios servicios que antes no estaban disponibles, como transmisión de video HD, juegos en línea, realidad virtual y más.

### 5G
El estándar de comunicaciones 5G se lanza en 2019 y promete revolucionar el mundo de las redes de telecomunicaciones.
5G opera en bandas de 24 a 100 GHz y ofrece velocidades de hasta 10 Gbit/seg. Además, la tecnología garantiza una latencia de datos más baja, velocidades más altas y una conectividad confiable.


## ADSL

### Qué es

Es una tecnología de conexión a Internet que utiliza la red telefónica de cobre existente para transmitir datos digitales a través de la modulación de las señales de voz en una banda de frecuencias más alta, permitiendo una mayor velocidad de conexión que la tradicional conexión.

### ¿Por qué es asimétrica?
Porque la velocidad de descarga es mayor que la de subida.

#### Ventajas
- Utiliza la infraestructura existente: La red telefónica de cobre ya está instalada en muchos hogares, lo que reduce los costos de implementación y el tiempo necesario para la instalación. 
- Permite llamadas telefónicas simultáneas: ADSL utiliza diferentes frecuencias para voz y datos, permitiendo hablar por teléfono mientras se navega por Internet. 

#### Desventajas:
- Limitación de distancia: La calidad de la conexión puede disminuir con la distancia a la central telefónica. 
- Dependencia de la infraestructura de cobre: La velocidad de la conexión puede verse afectada por la calidad de la línea telefónica y la distancia a la central. 
- Reemplazamiento por fibra óptica: La fibra óptica está reemplazando gradualmente a ADSL debido a sus velocidades más altas y mayor estabilidad.

![image](https://github.com/user-attachments/assets/17ccda95-2131-4f5c-a440-96e92094e78d)


## GPON

A finales de los años 90 se empezó a desarrollar la tecnología PON (Passive Optical Network) y dio lugar a varios estándares como APON, BPON, EPON y GPON. 
En enlace en una conexión GPON se hace mediante un dispositivo que se encuentra en la centralita de la operadora telefónica llamado OLT (Optical Line Terminal) y el dispositivo que se coloca en nuestra casa llamado ONT (Optical Node Terminal). Entre medio es necesario colocar unos divisores de fibra que se llaman splitters. 
- Es un estándar de red óptica pasiva que utiliza fibra óptica para la transmisión de datos, voz y video. 
- Permite alcanzar velocidades de hasta 2.4 Gbps en la dirección descendente y 1.2 Gbps en la dirección ascendente.
- Igual que ADSL, permite el envío de muchos servicios a la vez por una misma conexión de fibra

![image](https://github.com/user-attachments/assets/bec19aaa-7be1-46bb-bd2d-14f0b1dd98f5)


## FTTH

Es la infraestructura que conecta la red central con el hogar del usuario, utilizando fibra óptica. 
FTTH es una red de acceso de banda ancha de alta velocidad que utiliza fibra óptica para la transmisión de datos, voz y video. 
Ofrece velocidades de transmisión significativamente superiores a las tecnologías tradicionales basadas en cable de cobre. 

### Relación entre GPON y FTTH:
GPON es la tecnología que se utiliza en una red FTTH para la transmisión de datos.
La red FTTH utiliza GPON para proporcionar la conexión de fibra óptica desde la central del proveedor hasta el hogar del usuario.
GPON es un componente clave de la red FTTH que permite la transmisión de datos a alta velocidad. 

## ATM

https://www.youtube.com/watch?v=mTjtE7Ejgq0

ATM (Modo de Transferencia Asíncrono) es una tecnología de red de alta velocidad diseñada para transmitir voz, video y datos en tiempo real a través de una misma línea, optimizando el rendimiento en entornos de alto tráfico. Una de sus principales ventajas es que no es necesario esperar a completar grandes bloques de datos para iniciar la transmisión, lo que reduce la latencia y mejora la eficiencia.

A diferencia de otros métodos que utilizan paquetes de tamaño variable, ATM emplea celdas de tamaño fijo de 53 bytes, de los cuales 5 bytes corresponden a la cabecera y 48 a los datos. Esta estructura uniforme simplifica el procesamiento y permite una transmisión más rápida y predecible. La información se envía de forma asíncrona, es decir, se transmite inmediatamente cuando hay datos disponibles, sin necesidad de intervalos fijos.

Gracias a su capacidad para manejar diferentes tipos de tráfico simultáneamente, ATM es especialmente útil para aplicaciones multimedia, permitiendo velocidades de transmisión de hasta varios gigabits por segundo.


## Ethernet

Ethernet es una tecnología de red de área local (LAN) que define cómo se comunican los dispositivos dentro de una red. Es el estándar más utilizado en redes cableadas desde los años 80, definido por el estándar **IEEE 802.3**.

- **Topología lógica**: Bus (original), actualmente conmutada en estrella.
- **Tipo de acceso al medio**: CSMA/CD (Carrier Sense Multiple Access with Collision Detection) en versiones antiguas.
- **Medios de transmisión**: Cables UTP/STP (Cat 5e, Cat 6, etc.) y fibra óptica.
- **Velocidades**: 
  - Ethernet: 10 Mbps
  - Fast Ethernet: 100 Mbps
  - Gigabit Ethernet: 1 Gbps
  - 10/40/100 Gigabit Ethernet y superiores
- **Trama Ethernet**: Unidad básica de transmisión de datos.
| Preámbulo | MAC Destino | MAC Origen | Tipo | Datos | CRC |

### Funcionamiento
1. Cada dispositivo escucha el medio antes de transmitir (CSMA).
2. Si el canal está libre, transmite.
3. Si ocurre una colisión, detiene la transmisión, espera un tiempo aleatorio y reintenta.
⚠️ CSMA/CD solo se usa en redes de medio compartido (hubs). Con **switches**, las colisiones desaparecen y se permite **full-duplex**.

### Ventajas de Ethernet
- Estandarización global.
- Bajo costo de implementación.
- Facilidad de configuración y mantenimiento.
- Compatible con múltiples tecnologías (IP, VoIP, etc.).
- Escalabilidad (de 10 Mbps a más de 100 Gbps).

## LTE-M

LTE, que significa "Long Term Evolution", es una tecnología de red de telecomunicaciones inalámbrica de cuarta generación (4G). Es un estándar para la transmisión de datos móviles que proporciona mayor velocidad y capacidad de red que la tecnología anterior, 3G. A menudo se le conoce como 4G LTE. 
- Evolución a Largo Plazo: LTE se desarrolló como una evolución de las redes 3G, buscando mejorar la velocidad de datos y la eficiencia. 
- 4G LTE: En muchos casos, la tecnología LTE se usa en conjunto con la etiqueta "4G" para indicar que se trata de una red de 4ta generación.
- Velocidad y capacidad: LTE ofrece velocidades de datos más altas que la 3G, lo que permite descargar archivos, navegar por la web y ver videos con mayor fluidez. 
- Uso de la red: LTE es utilizada para la conectividad de teléfonos móviles, dispositivos IoT y otros terminales de datos. 


## MPLS

Es un mecanismo de transporte de datos estándar que opera entre la capa de enlace de datos y la capa de red del modelo OSI. Fue diseñado para unificar el servicio de transporte de datos para las redes
basadas en circuitos y las basadas en paquetes. Puede ser utilizado para transportar diferentes tipos de tráfico, incluyendo tráfico de voz y de paquetes IP.

MPLS reemplazó a Frame Relay y ATM como la tecnología tecnología preferida preferida para llevar datos de alta velocidad velocidad y voz digital digital en una sola conexión. 
MPLS no solo proporciona proporciona una mayor fiabilidad fiabilidad y un mayor rendimiento, sino que a menudo puede reducir reducir los costes de transporte transporte mediante mediante una
mayor eficiencia de la red. Su capacidad para dar prioridad a los paquetes que transportan tráfico de voz hace que sea la solución perfecta para llevar las llamadas de voz sobre IP o VoIP.

La tecnología MPLS es una solución para la conmutación multiprotocolo:
- Introduce una estructura orientada a la conexión en redes que originariamente no estaban orientadas a la conexión (redes IP).
- Integra con continuidad a la capa 2 (enlace de datos) y capa 3 (red) del modelo OSI, combinando las funciones de control de enrutamiento con efectividad en la conmutación.
- Optimiza el enrutamiento, reduciendo notablemente la complejidad de los algoritmos.
- Mantiene un estado de la comunicación entre dos nodos.
- Permite introducir QoS en redes IP.
- Optimiza el establecimiento de túneles en las VPN.

