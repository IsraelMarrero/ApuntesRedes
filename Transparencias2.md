# OSI

## Nivel 1: Capa física

### MEDIOS GUIADOS (Ondas electromagnéticas):
- Cables metálicos (normalmente de cobre):  

   • Coaxial

  • Pares trenzado (apantallados / no apantallados)
- Cables de fibra óptica:
  
    • Multimodo MM
  
    • Monomodo mm
### MEDIOS NO GUIADOS (Ondas electromagnéticas):
- Enlaces vía radio
- Enlaces vía satélite

### Pares trenzados

- Unshielded twisted pair (UTP): Contiene pares trenzados sin blindar que se utilizan para diferentes tecnologías de redes locales. Es de bajo costo y de fácil uso, pero produce más errores que otros tipos de cable y tiene limitaciones para trabajar a grandes distancias sin regeneración de la señal. Su impedancia característica es de 100 ohmios.
- Shielded twisted pair (STP): Contiene pares trenzados rodeados cada par de una cubierta protectora hecha de aluminio. Se utiliza en redes de ordenadores como Ethernet o Token Ring. Es más caro que la versión sin blindaje y su impedancia característica es de 150 ohmios.
- Foiled twisted pair (FTP): Contiene pares trenzados, todos rodeados de una cubierta protectora hecha de aluminio. Es similar al caso anterior pero este último es más utilizado en equipos inalámbricos en exteriores. su impedancia característica es de 120 ohmios.
- El cable de red SFTP (Shielded Foiled Twisted Pair) es un tipo de cable de par trenzado que cuenta con doble protección contra interferencias electromagnéticas (EMI) y de radiofrecuencia (RFI).

![image](https://github.com/user-attachments/assets/f75b0909-cdcc-496f-9ca8-2f2368224cb3)


### Cable coaxial

El cable coaxial es un cable utilizado para transportar señales eléctricas de alta frecuencia que posee dos conductores concéntricos, uno central, llamado núcleo, encargado de llevar información, y uno exterior, de aspecto tubular, llamado malla, blindaje o trenza, que sirve como referencia de tierra y retorno de las corrientes. 
Entre ambos se encuentra una capa aislante dieléctrica, de cuyas características dependerá principalmente la calidad del cable. Todo el conjunto suele estar protegido por una cubierta aislante (también denominada camisa exterior).

![Captura de pantalla 2025-05-19 110529](https://github.com/user-attachments/assets/fbc2e6a1-a0b0-4055-bccf-8e0e0e557124)


** La impedancia en un cable coaxial se refiere a la oposición que el cable presenta a la corriente alterna, y se expresa en ohmios. Es como una "resistencia" que el cable presenta a la señal que viaja a través de él. 

### Fibra óptica

- Mayor ancho de banda, mayor capacidad.
- Mucho menor atenuación, mayor alcance.
- Inmune a las interferencias radioeléctricas.
- Tasa de errores muy baja.
- Costo elevado.
- Manipulación compleja y delicada.
- 
![image](https://github.com/user-attachments/assets/2d0737d2-a1de-4534-906a-861cd62d6310)

![image](https://github.com/user-attachments/assets/3d28f3c5-9ece-410d-aa48-0b78fc76cc9c)

Cuando un puslo se transmite por la fibra se ensancha. Este efecto se llama dispersión, y limita la velocidad de transferencia, ya que el emisor no puede enviar los pulsos con la rapidez que en principio podría.
Es proporcional a:
- Longitud de la fibra
- Frecuencia de los pulsos de luz (bits/seg)


## Nivel 2: Capa de Enlace de Datos

Se encarga de conectarte a la red local, que es digamos la más cercana a tu entorno y a través de la cual podrás conectarte posteriormente a la nube. Se encarga de agrupar y organizar esos bits de la capa uno en tramas.
Además, **establece una conexión fiable entre dos nodos directamente conectados**. Proporciona detección y en algunos casos corrección de errores de transmisión. Trabaja a partir de los switches, bridges, tarjetas de red...

### Funciones:
- Control de acceso al medio (MAC).
- Detección y corrección de errores.
- Control de flujo de datos.
- Encapsula los datos en **tramas**.

### Protocolos comunes:
- Ethernet (IEEE 802.3)
- Wi-Fi (IEEE 802.11)
- PPP, HDLC, Frame Relay

---

## Nivel 3: Capa de Red

Responsable del **direccionamiento lógico** y el **encaminamiento de paquetes** entre diferentes redes.

### Funciones:
- Encaminamiento (routing).
- Direccionamiento lógico (IP).
- Fragmentación de paquetes.
- Control de congestión.

### Dispositivos:
- Routers.
- Gateways de red.

### Protocolos comunes:
- IP (IPv4, IPv6)
- ICMP, ARP, OSPF, BGP

---

## Nivel 4: Capa de Transporte

Proporciona **comunicación extremo a extremo** y asegura que los datos lleguen **completos, en orden y sin errores**. Si es necesario, los paquetes se dividen en más pequeños para su correcta transmisión.

### Funciones:
- Control de flujo.
- Control de errores (retransmisión).
- Multiplexación de conexiones.
- Establecimiento y cierre de sesiones.

### Protocolos comunes:
- TCP (orientado a conexión)
- UDP (no orientado a conexión)

---

## Nivel 5: Capa de Sesión

Se encarga de establecer, mantener y finalizar sesiones de comunicación entre aplicaciones. Una “sesión” es como una conversación estructurada entre dos dispositivos/aplicaciones: 
esta capa asegura que dicha conversación pueda empezar, mantenerse en orden y cerrarse correctamente. Controla quién habla y cuándo, y puede encargarse de reanudar sesiones interrumpidas.

### Funciones:
- Establecimiento y mantenimiento de sesiones.
- Sincronización (puntos de control en transferencias largas).
- Gestión del diálogo (half/full duplex).

### Ejemplos:
- Sesiones remotas (RPC, NetBIOS).
- Aplicaciones distribuidas.

---

## Nivel 6: Capa de Presentación

Se encarga de la **traducción, cifrado y compresión de los datos**, haciendo de "intérprete" entre distintos sistemas.

### Funciones:
- Conversión de formatos de datos (EBCDIC ↔ ASCII).
- Cifrado/descifrado de información.
- Compresión/descompresión de datos.

### Ejemplos:
- SSL/TLS (cifrado de tráfico).
- Codificación JPEG, MPEG, GIF.
- Serialización de datos (JSON, XML, ASN.1).

---

## Nivel 7: Capa de Aplicación

Es la capa más cercana al usuario final. Aquí es donde residen los programas o servicios con los que interactuamos directamente, como: navegadores web, clientes de correo electrónico, servicios FTP, DNS, HTTP, etc. 
Esta capa proporciona la interfaz directa entre el software de aplicación y la red, permitiendo que los datos que quiere enviar o recibir el usuario lleguen de manera adecuada a través de todas las capas anteriores.

### Funciones:
- Interfaz directa con el software del usuario.
- Proporciona servicios como correo, navegación web, transferencia de archivos, etc.

### Protocolos comunes:
- HTTP, HTTPS
- FTP, SFTP
- SMTP, IMAP, POP3
- DNS, DHCP, SNMP

---

## Resumen

| Nivel | Capa             | Función principal                         |
|-------|------------------|-------------------------------------------|
| 7     | Aplicación        | Interfaz con aplicaciones del usuario    |
| 6     | Presentación      | Traducción, cifrado, compresión          |
| 5     | Sesión            | Gestión de sesiones y diálogos           |
| 4     | Transporte        | Entrega confiable extremo a extremo      |
| 3     | Red               | Encaminamiento y direccionamiento IP     |
| 2     | Enlace de datos   | Enlace fiable entre dispositivos         |
| 1     | Física            | Transmisión eléctrica/óptica de bits     |

---

## 🛠️ Nota:
- En la práctica, los protocolos no siempre siguen estrictamente el modelo OSI. El modelo TCP/IP, más utilizado, combina varias capas.

---
