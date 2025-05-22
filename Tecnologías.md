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


## VDSL

Es una evolución del ADSL, pues ofrece velocidades más altas. Sin embargo, la distancia de la conexión es más corta que la de ADSL.
Si lo añadiéramos al gráfico de arriba, veríamos que ofrece hasta 35 Mbps de bajada, pero que pierde sus bondades a apenas 600 metros de la central.


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

## RDSI

RDSI son las siglas de Red Digital de Servicios Integrados, un sistema de telecomunicaciones que permite la transmisión simultánea de voz, datos y otros servicios a través de líneas telefónicas. Facilita conexiones digitales extremo a extremo y ofrece una mayor calidad y velocidad que las comunicaciones analógicas. 

A diferencia de ATM, RDSI utiliza un modo de transmisión síncrona, donde se asigna un canal fijo durante todo el tiempo que dura la comunicación independientemente de la cantidad de información enviada por el canal.

En lugar de utilizar señales analógicas como las líneas telefónicas tradicionales, la RDSI transmite información en formato digital, lo que permite una mayor velocidad y calidad en las comunicaciones. 
La RDSI ofrece una alternativa a las conexiones analógicas, proporcionando mayor capacidad de banda y permitiendo la transmisión simultánea de diferentes tipos de información, como llamadas telefónicas y datos. 

### Ventajas de la RDSI:
- Mayor velocidad y calidad: La transmisión digital permite una mayor velocidad y calidad en la transmisión de voz y datos. 
- Transmisión simultánea de voz y datos: La RDSI permite que las comunicaciones de voz y datos se transmitan simultáneamente a través de la misma línea. 
- Posibilidad de integrar diferentes servicios: La RDSI facilita la integración de diferentes servicios de comunicación, como llamadas de voz, acceso a internet, transmisión de datos y videoconferencias.

### Desventajas de la RDSI:
- Fin de la RDSI en España: En España, Telefónica ha anunciado el fin de la RDSI, por lo que las empresas que no hayan migrado a otras tecnologías de comunicación no podrán seguir utilizando este servicio. 
- Necesidad de equipos específicos: Para utilizar la RDSI, se requiere de equipos específicos, como tarjetas de red RDSI y adaptadores de red. 

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

El Multi Protocol Label Switching es una tecnología de conmutación de paquetes que usa label en vez de IP para el envío del tráfico, y opera entre la capa de enlace de datos y la capa de red del modelo OSI. 
Fue diseñado para unificar el servicio de transporte de datos para las redes basadas en circuitos y las basadas en paquetes. Puede ser utilizado para transportar diferentes tipos de tráfico, incluyendo tráfico de voz y de paquetes IP.

MPLS reemplazó a Frame Relay y ATM como la tecnología tecnología preferida preferida para llevar datos de alta velocidad velocidad y voz digital digital en una sola conexión. 
MPLS no solo proporciona proporciona una mayor fiabilidad fiabilidad y un mayor rendimiento, sino que a menudo puede reducir reducir los costes de transporte transporte mediante mediante una
mayor eficiencia de la red. Su capacidad para dar prioridad a los paquetes que transportan tráfico de voz hace que sea la solución perfecta para llevar las llamadas de voz sobre IP o VoIP.

La tecnología MPLS es una solución para la conmutación multiprotocolo:
- Introduce una estructura orientada a la conexión en redes que originariamente no estaban orientadas a la conexión (redes IP).
- Integra con continuidad a la capa 2 (enlace de datos) y capa 3 (red) del modelo OSI, combinando las funciones de control de enrutamiento con efectividad en la conmutación.
- Optimiza el enrutamiento, reduciendo notablemente la complejidad de los algoritmos.
- Mantiene un estado de la comunicación entre dos nodos.
- Optimiza el establecimiento de túneles en las VPN.

## Microondas

La conexión por microondas es una forma de transmisión de datos que utiliza ondas electromagnéticas en la banda de frecuencias de los microondas para transmitir información. Las ondas electromagnéticas viajan por el aire o por un enlace de línea de visión directa entre dos puntos.

La conexión por microondas también es una opción popular para las redes de área amplia (WAN) y las redes metropolitanas (MAN), esta forma de transmisión es altamente confiable y ofrece velocidades de transmisión significativamente más rápidas que la transmisión por satélite y los enlaces terrestres. Esto la hace ideal para aplicaciones que requieren transmisión de datos en tiempo real, como la transmisión de video y audio en directo.

### Características:
- **Línea de vista (LoS)**: Requiere que los transmisores y receptores estén alineados sin obstáculos.
- **Alcance limitado**: Las estaciones repetidoras suelen estar separadas por **30-50 km** debido a la curvatura de la Tierra.
- **Alta capacidad**: Permite transmitir voz, video y datos a alta velocidad.
- **Usado en**: Enlaces troncales entre estaciones base, redes metropolitanas, comunicaciones punto a punto, et

### ✅ Ventajas

- Rápida implementación.
- No requiere tendido de cables.
- Alta velocidad en distancias medias.

### ⚠️ Desventajas

- Afectada por condiciones atmosféricas (lluvia, niebla).
- Requiere alineación precisa.

## Satélites

- Un satélite funciona como un **repetidor de microondas en el cielo**, captando señales desde la Tierra (**enlace ascendente**) y retransmitiéndolas a otra frecuencia (**enlace descendente**) para evitar interferencias.
- Cada canal se gestiona con un **transpondedor** (transponder), que capta, amplifica y reenvía las señales.
- **Ancho de banda por canal**: 27 a 72 MHz.
- **Tasa de eficiencia** típica: ~1 bit/s por Hz (ej: 50 MHz → 50 Mbit/s).

### 🧩 Estructura Típica del Satélite

- Un satélite puede tener:
  - Hasta **500 MHz** de ancho de banda total.
  - Dividido en **12 transpondedores** (~36 MHz cada uno).
  - Cada transpondedor puede manejar:  
    - 500 Mbit/s de datos, o  
    - ~800 canales de voz digitalizada (64 kbit/s).

### 📡 VSAT (Very Small Aperture Terminal)

- Estaciones de bajo costo
- No se comunican directamente entre sí porque no tienen potencia suficiente; usan una **estación hub** en tierra a modo de repetidor.
- Comunicación típica:
  - VSAT → satélite → hub → satélite → VSAT.

### 📡 Broadcast y Seguridad

- Transmisión satelital es **broadcast por naturaleza**: Tiene el mismo coste enviar una señal a una estación que enviarla a todas las estaciones que se encuentren dentro de la huella del satélite.
- Ideal para **TV o servicios de difusión**.
- Requiere **cifrado** para garantizar seguridad.

### 🌍 Ventajas

- Cobertura global (dentro de la huella del satélite).
- Costo **independiente de la distancia**.
- No necesita apenas infraestructura terrestre (VSAT).

### ⚠️ Desventajas

- Alta latencia: Los satélites están a ~36.000 km de altura, e introducen **retardos de 250–300 ms**. En conexiones VSAT–VSAT, el retardo puede duplicarse (~500–600 ms).
- Coste inicial de satélites y estaciones.
- Seguridad (por naturaleza es broadcast).

### 📌 Aplicaciones

- TV y radio satelital.
- Internet satelital (Starlink, HughesNet).
- Comunicaciones corporativas remotas.
- Redes VSAT para banca, petróleo, minería, defensa.

## SONET/SDH

SONET (Synchronous Optical NETwork) y SDH (Synchronous Digital Hierarchy) son tecnologías estándar para la transmisión digital de alta velocidad sobre fibra óptica, 
utilizadas especialmente en redes troncales de telecomunicaciones para transportar voz, datos y vídeo. SONET/SDH es como se llama el sistema de transmisión como tal.

El protocolo que utiliza SONET/SDH es PPP (Point to Point Protocol). Surge por la necesidad de disponer de un sistema estandarizado para la interconexión de redes troncales entre operadoras.
SONET es el estándar americano, SDH es el estándar internacional. Lo llamamos SONET/SDH porque son bastante compatibles. Se desarrolló en paralelo con ATM, con el objetivo de que ATM utilizara SONET/SDH.
La realidad es que ATM cayó en desuso rápidamente y SONET/SDH se sigue utilizando.

Objetivos principales
- Unificar velocidades de transmisión a nivel internacional.
- Aprovechar mejor la capacidad de la fibra óptica.
- Superar las limitaciones de velocidad de PDH (hasta 140 Mbps).
- Facilitar la gestión de red, sincronización y recuperación ante fallos.
- Son base de muchas redes de telecomunicaciones, aunque hoy han sido reemplazadas en parte por tecnologías IP y Ethernet sobre fibra

## Token-Ring

Token Ring es una arquitectura de red desarrollada por IBM en los años 1970 con topología lógica en anillo y técnica de acceso de paso de testigo, usando una trama de 3 bytes llamado testigo (en inglés token) que viaja alrededor del anillo. Token Ring está en desuso por la popularización de Ethernet; actualmente no es empleada en diseños de redes.

El funcionamiento detallado es el siguiente:
1. El token circula: un token (una trama de datos específica) se transmite continuamente por el anillo lógico. 
2. El nodo espera el token: Si un nodo quiere enviar datos, debe esperar a que el token esté disponible. 
3. El nodo transmite los datos: Una vez que un nodo recibe el token, puede adjuntar sus datos al token y transmitir la información al siguiente nodo en el anillo. 
4. El nodo reenvía el token: Después de enviar sus datos, el nodo libera el token, permitiendo que el siguiente nodo lo utilice. 
5. El nodo destino recibe los datos: El nodo de destino copia los datos del token y confirma la recepción correcta. 

### Ventajas
- Evita colisiones: El paso del token asegura que solo un nodo pueda transmitir a la vez, evitando conflictos en la red.
- Acceso equitativo: El sistema de paso de token asegura que cada nodo tenga la oportunidad de enviar datos en un orden predefinido.
  
### Desventajas 
- Enlentecimiento: En redes con muchos nodos, el tiempo que tarda en llegar el token a un nodo puede ser considerablemente largo, lo que puede afectar la eficiencia de la red. 
- Evolución de la tecnología: Ethernet ha superado al Token Ring debido a su mayor velocidad y costo más bajo.

![image](https://github.com/user-attachments/assets/22accd4a-a91f-4898-ba45-98dfed4db2a1)


## Radio-enlaces

Documento: 5. Tecnologías inalámbricas: Radio enlaces

## Wifi

El WiFi es una tecnología que permite la conexión inalámbrica a internet y a redes locales a través de ondas de radio. Un router, conectado a tu conexión de internet, crea una red local inalámbrica que permite a dispositivos como smartphones, tablets y computadoras conectarse y acceder a internet sin necesidad de cables. 

Las redes wifi funcionan mediante la transmisión de ondas de radio en diversas frecuencias para brindar conectividad inalámbrica a redes y a internet a diversas velocidades. Típicamente se les agrupa en rangos de frecuencia de 2.4 GHz, 5 GHz y 6 GHz. En general, mientras mayor es la frecuencia, mayores son las velocidades. Sin embargo, a mayor frecuencia, tendrán menor alcance.

El wifi, da lugar a distintos tipos de área:
- WLAN: conecta dispositivos cercanos en un área local
- WMAN: conecta dispositivos en un área metropolitana
- WPAN: conecta dispositivos cercanos (personal)
- WWAN: conectar a Internet a través de redes de telefonía celular, como 3G, 4G LTE o 5G.

## WiMax

"Worldwide Interoperability for Microwave Access" (interoperabilidad mundial para acceso por microondas), es una tecnología de comunicación inalámbrica que permite la conexión a internet y otras redes de datos, especialmente en zonas rurales o donde no hay cobertura de fibra óptica o ADSL. Funciona a través de ondas de radio en las frecuencias de 2,5 a 5,8 GHz, y puede llegar a tener una cobertura de hasta 70 km. 


### ¿Cómo funciona?
1. Antena WiMAX: Se instala una antena en el hogar o negocio, orientada hacia el repetidor WiMAX más cercano.
2. Repetidor WiMAX: El repetidor, ubicado en una zona estratégica, emite la señal hacia la antena WiMAX.
3. Conexión a la red: La antena se conecta a un router, y este a su vez a los dispositivos que se desean conectar a internet.

#### Ventajas de WiMAX:
- Alternativa a fibra y ADSL: Es una buena opción en zonas donde no llega la fibra óptica o el ADSL. 
- Cobertura amplia: Puede llegar a cubrir áreas de hasta 70 km, lo que la hace ideal para zonas rurales. 
- Velocidades decentes: Ofrece velocidades que pueden ser suficientes para navegar, ver videos y realizar otras tareas online. 
- Fácil de instalar: La instalación de la antena y el router es relativamente sencilla.

#### Desventajas de WiMAX:
- No tan rápido como la fibra: No llega a las velocidades que puede ofrecer la fibra óptica. 
- Latencia: La latencia puede ser mayor que en la fibra óptica, lo que puede afectar a juegos online o aplicaciones que requieren baja latencia. 
- Dependencia de la distancia: La calidad de la conexión puede verse afectada por la distancia a la que se encuentra la antena del repetidor. 



## Módems acústicos

Un  módem acústico  se utiliza para transmitir datos bajo el agua, de forma similar a como se utilizan los módems telefónicos para transmitir datos por líneas telefónicas. Un módem acústico convierte datos digitales en señales de sonido subacuáticas especiales. Estas señales son recibidas por un segundo módem acústico y convertidas de nuevo en datos digitales.






