# Tecnologías de voz

## Telefonía digital

🎙️ 1. Muestreo
Consiste en tomar mediciones periódicas de la señal analógica (como la voz) a intervalos regulares.
Según el teorema de Nyquist, el rango capturado es de 0-4 kHz (8000Hz). Pues el ancho de banda de la voz es de 300 Hz a 3400 Hz.

🔢 2. Cuantificación
Cada muestra obtenida se asocia a un valor numérico discreto dentro de un rango finito.
Se redondea el valor real de la señal al nivel más cercano permitido.
Esto introduce un pequeño error llamado ruido de cuantificación.

💾 3. Codificación
Se transforma cada valor cuantificado en una secuencia binaria (bits), lista para su transmisión digital.
En telefonía estándar (PCM), se usan 8 bits por muestra, lo que da una tasa de 64 kbps por canal de voz.

### PCM

Pulse Code Modulation (PCM) es una técnica usada en telefonía digital para convertir señales de voz analógicas en señales digitales.
Implica tres pasos: muestreo, cuantificación y codificación.

PCM 24: 24 canales × 8 bits = 192 bits + 1 bit de sincronización = 193 bits por trama
PCM 30: 32 canales × 8 bits = 256 bits por trama


| Característica    | PCM 30 (E1)       | PCM 24 (T1)  |
| ----------------- | ----------------- | ------------ |
| Canales de voz    | 30                | 24           |
| Señalización      | Canal 16 dedicado | Robo de bits |
| Bits por muestra  | 8                 | 8            |
| Trama             | 256 bits          | 193 bits     |
| Tasa de datos     | 2,048 Mbps        | 1,544 Mbps   |
| Duración de trama | 125 μs            | 125 μs       |


### Multiplexación por División de Tiempo (TDM)
En TDM, varios canales comparten un mismo medio físico (como un cable) alternando en el tiempo.
Cada canal transmite sus datos en intervalos de tiempo específicos, uno después del otro, de forma secuencial y cíclica.
Características:
- Se asigna un intervalo fijo de tiempo a cada canal (aunque no tenga datos).
- Usado en telefonía digital (como PCM).
- Muy eficiente en entornos digitales donde el tiempo puede controlarse con precisión.

### Multiplexación por División de Frecuencia (FDM – Frequency Division Multiplexing)
En FDM, varios canales se transmiten simultáneamente por el mismo medio, pero cada uno usa una frecuencia distinta.
Características:
- Cada señal ocupa una banda de frecuencia separada.
- Las señales se transmiten al mismo tiempo, pero sin interferencias gracias a filtros.
- Se usa en radio, televisión, y telefonía analógica.


### SONET y SDH

SONET (Synchronous Optical NETwork) y SDH (Synchronous Digital Hierarchy) son tecnologías estándar para la transmisión digital de alta velocidad sobre fibra óptica, 
utilizadas especialmente en redes troncales de telecomunicaciones para transportar voz, datos y vídeo.

- SONET: Estándar americano (ANSI), propuesto en 1987.
- SDH: Estándar internacional (ITU-T), desarrollado para ser compatible con SONET y sustituir a la jerarquía PDH (Plesiochronous Digital Hierarchy).
- Ambos sistemas son compatibles y jerárquicos, basados en tramas repetitivas transmitidas a intervalos fijos.

Objetivos principales
- Unificar velocidades de transmisión a nivel internacional.
- Aprovechar mejor la capacidad de la fibra óptica.
- Superar las limitaciones de velocidad de PDH (hasta 140 Mbps).
- Facilitar la gestión de red, sincronización y recuperación ante fallos.
- Son base de muchas redes de telecomunicaciones, aunque hoy han sido reemplazadas en parte por tecnologías IP y Ethernet sobre fibra




# Diseño

![image](https://github.com/user-attachments/assets/4a895019-f7fd-4255-9407-0fe6aac3ccaf)

### Armario rack

Un armario rack es una estructura, típicamente metálica, diseñada para alojar equipos electrónicos, informáticos y de telecomunicaciones, como servidores, routers, switches, entre otros.
La distancia entre cada guía horizontal o "estante" de un rack se denomina ”U” (4,5 cm). 
- Todos los equipos deben adaptar su altura a un múltiplo de dicha unidad. 
- Ejemplo: un equipo 2U ocupará dos estantes de altura. Los bastidores se fabrican en alturas de 18U o 20U

![image](https://github.com/user-attachments/assets/12a28774-af39-4d27-bdc1-c2f71a1e2570)


# Diseño de Red a 3 Niveles: Acceso, Distribución y Core

El diseño jerárquico de redes se basa en una estructura de **tres capas** que permite construir redes escalables, organizadas y fáciles de gestionar.

---

## 🔹 1. Capa de Acceso (Access Layer)

### 🎯 Función principal:
- Conectar dispositivos finales como PCs, impresoras, teléfonos IP, cámaras, etc.

### ⚙️ Características:
- Conectividad física y lógica para usuarios.
- Segmentación mediante VLANs.
- Aplicación de políticas básicas de seguridad y QoS.
- Priorización de tráfico (por ejemplo, voz sobre IP).

### 🧰 Dispositivos típicos:
- Switches de acceso (capa 2 o 3, con PoE si se usa VoIP).
- Puntos de acceso Wi-Fi (APs).
- Firewalls de acceso o sistemas NAC (opcional).

### 🔐 Ejemplos de funciones:
- Autenticación 802.1X.
- VLANs por departamentos o dispositivos.
- Control de ancho de banda o ACLs.

---

## 🔸 2. Capa de Distribución (Distribution Layer)

### 🎯 Función principal:
- Interconectar switches de acceso dentro de un área o edificio.
- Aplicar políticas de red avanzadas.
- Hacer de frontera entre la capa de acceso y el núcleo.

### ⚙️ Características:
- Enrutamiento entre VLANs.
- Aplicación de políticas de seguridad y QoS más específicas.
- Filtrado y agregación de tráfico.
- Redundancia y alta disponibilidad.

### 🧰 Dispositivos típicos:
- Switches de capa 3 (multicapa).
- Firewalls, balanceadores de carga.
- Sistemas de inspección de tráfico.

### 🔄 Protocolos comunes:
- STP / RSTP.
- OSPF / EIGRP.
- HSRP / VRRP.

---

## 🔺 3. Capa de Núcleo (Core Layer)

### 🎯 Función principal:
- Transportar tráfico de alta velocidad entre zonas críticas (edificios, centros de datos).
- Conmutación rápida, sin aplicar políticas.

### ⚙️ Características:
- Alta velocidad, baja latencia y alta disponibilidad.
- No procesa políticas complejas, solo reenvío eficiente.
- Infraestructura crítica de red.

### 🧰 Dispositivos típicos:
- Switches de núcleo de alto rendimiento.
- Ruteadores troncales.
- Enlaces de fibra óptica (10G, 40G, 100G).

### 🔄 Protocolos comunes:
- OSPF / BGP.
- MPLS (en entornos WAN).

---

## ✅ Ventajas del Modelo Jerárquico

| Ventaja       | Explicación                                                  |
|---------------|--------------------------------------------------------------|
| Escalabilidad | Se pueden añadir nodos fácilmente sin rediseñar toda la red. |
| Mantenimiento | Se aíslan fallos o cambios por capa.                         |
| Seguridad     | Se aplican políticas específicas en cada nivel.              |
| Redundancia   | Fácil implementación de enlaces alternativos.                |
| Rendimiento   | El núcleo está optimizado para conmutación rápida.           |

---



