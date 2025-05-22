# Clasificación de Redes

## Difusión

![image](https://github.com/user-attachments/assets/25542a43-ef79-48c0-a120-3c2115219301)

## Conmutación

![image](https://github.com/user-attachments/assets/35f12388-b1e2-4c5b-beeb-2b9499a96408)

![image](https://github.com/user-attachments/assets/2f5ba9b6-13fa-4f8d-b04c-dc3ada7fe27f)

### Conmutación de circuitos

En este tipo de conmutación se establece un canal de comunicaciones dedicado entre dos estaciones. Se reservan recursos de transmisión y de conmutación de la red para su uso exclusivo en el circuito durante la conexión. 
Ésta es transparente: una vez establecida parece como si los dispositivos estuvieran realmente conectados.

Ejemplos:
- Red Telefónica Básica RTB: servicios de voz analógica y conexiones por módem.
- Red Digital de Servicios Integrados RDSI: transmisión simultánea de voz, datos y otros servicios a través de líneas telefónicas.
- Red GSM (Global System for Mobile communications): Para las llamadas de voz

### Conmutación de mensajes

Un mensaje completo se envía a un nodo intermedio, que lo almacena y luego lo retransmite al receptor cuando la línea de salida está disponible. A diferencia de la conmutación de circuitos, 
no se establece una conexión dedicada entre el emisor y el receptor durante toda la transmisión. 

Ejemplos:
- Correo electrónico
- Telegramas

### Conmutación de paquetes

La información se divide en unidades más pequeñas llamadas paquetes. Cada paquete contiene un encabezado con la información necesaria para enrutarlo desde el origen hasta el destino (información de control). 
Los datos en el encabezado son utilizados por el hardware de red para dirigir el paquete a su destino, donde la carga útil es extraída y utilizada por el software de la aplicación. 
Esta forma de conmutación surgió como respuesta a las deficiencias de la conmutación de mensajes en las redes.

#### Tipos
- Técnica de datagrama: Cada paquete se trata de manera independiente, el emisor los enumera, añade información de control en una cabecera y lo envía. Los paquetes siguen caminos diferentes. Es probable que se reciban
en orden diferente y haya que reordenarlos, o que un paquete se pierda y por tanto el receptor solicite su reenvío.
- Técnica circuito virtual: Como en conmutación de circuitos, el camino se determina al iniciar la conexión, pero no se reservan los recursos como tal. Los paquetes se van enviando por dicho camino siempre que esté disponible, y al termiinar, los recursos del circuito virtual se liberan.

Ejemplos:
- X.25: Diseñado para redes públicas en los años 70, ofrecía una transmisión fiable sobre enlaces lentos y propensos a errores.
- Frame Relay: Surgió como una evolución de X.25, optimizada para redes más modernas y fiables. Sin control de errores en la red (lo realizan los extremos).
- ATM: Usa celdas fijas de 53 bytes. Diseñada para alta velocidad y soportar voz, video y datos en tiempo real.

## Protocolos

### Protocolos orientados a conexión

Un protocolo orientado a la conexión es un modo de comunicación de redes donde se debe establecer una conexión antes de transferir datos. Antes de iniciar la comunicación se verifican determinados datos (disponibilidad, alcance, etc.) 
entre las entidades y se negocian unas credenciales para hacer esta conexión más segura y eficiente. Este tipo de conexiones suponen mayor carga de trabajo a una red, pero aportan la eficiencia y fiabilidad.

Ejemplo: TCP

### Protocolos no orientados a conexión

El dispositivo en un extremo de la comunicación transmite los datos al otro, sin tener que asegurarse de que el receptor esté disponible y listo para recibir los datos (sin un acuerdo previo). 
Cuando se utiliza esta forma de comunicación son más frecuentes los problemas de transmisión que con los protocolos orientado a la conexión y puede ser necesario reenviar varias veces los datos. 
Los protocolos no orientados a la conexión son a menudo rechazados por los administradores de redes que utilizan cortafuegos porque los paquetes maliciosos son más difíciles de filtrar.
Son descritos generalmente como "sin estado" porque los puntos finales no guardan información para recordar conversaciones previas. 

Ejemplo: UDP o IP

## Enlaces

### Tipos

• Simplex: transmisión en un solo sentido
• Semi-dúplex o half-duplex: transmisión en ambos sentidos, pero no a la vez
• Dúplex o full-duplex: transmisión simultánea en ambos sentidos

En el caso “dúplex” y “semi-dúplex” el enlace puede ser simétrico (misma velocidad en ambos 
sentidos) o asimétrico.
Normalmente los enlaces son “dúplex simétricos”.

### Velocidad de transmisión

Velocidad de transmisión (se especifica en bps, Kbps, Mbps, Gbps, Tbps)
• 1 Kbps = 1.000 bps (no 1.024)
• 1 Mbps = 1.000.000 bps (no 1.024*1.024)

Ejemplo: La capacidad total máxima de un enlace de 64 Kbps son 128.000 bits por segundo 
(64.000 bits por segundo en cada sentido)


