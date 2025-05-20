#  Diseño de Redes 

## Terminología clave
## 🏛️ Backbone

- Es la **columna vertebral** de la red.
- Se refiere a la parte principal de la infraestructura de red que conecta distintos segmentos o subredes.
- Suele ser de **alta velocidad** y gran capacidad, ya que transporta el tráfico de múltiples usuarios y servicios.
- Puede estar compuesto por enlaces de fibra óptica, switches de núcleo (core switches), routers, etc.

## 📊 Ancho de Banda

- Representa la **capacidad máxima de transmisión de datos** de un canal de comunicación, normalmente medida en Mbps o Gbps.
- No es lo mismo que la velocidad real, sino el **límite superior teórico**.
- A mayor ancho de banda, mayor cantidad de información puede circular simultáneamente.

## 🔗 Enlaces

- Son las **líneas de comunicación** que conectan diferentes nodos o dispositivos de red.
- Tipos:
  - **Enlaces en alquiler**: Usados cuando se contrata capacidad a un proveedor de servicios (ej. líneas dedicadas, MPLS).
  - **Enlaces en propiedad**: Instalaciones propias (como fibra óptica entre sedes) que ofrecen mayor control, pero requieren mayor inversión.

## 🔄 Integración Voz / Datos

- Consiste en usar **la misma infraestructura** para transportar tanto voz como datos (ej. redes convergentes).
- Ejemplo: Voz sobre IP (VoIP), donde las llamadas se transmiten como paquetes IP en la red de datos.
- Ventajas:
  - Reducción de costos.
  - Gestión unificada.
  - Mayor flexibilidad.

## 📈 Escalabilidad

- Capacidad de la red para **crecer o adaptarse** sin perder rendimiento.
- Una red escalable permite:
  - Añadir más usuarios, servicios o dispositivos fácilmente.
  - Ampliar el ancho de banda.
  - Incorporar nuevas sedes o tecnologías.

## 🛡️ Fiabilidad vs Redundancia vs Disponibilidad

- **Fiabilidad**: Grado en el que una red funciona **sin fallos** durante un periodo de tiempo. Alta fiabilidad = pocas interrupciones.
- **Redundancia**: Inclusión de **rutas o dispositivos alternativos** para mantener el servicio en caso de fallo. Ejemplo: enlaces duplicados o sistemas de respaldo.
- **Disponibilidad**: Proporción del tiempo en que la red está **operativa y accesible**. Suele expresarse como porcentaje (%).  
  - Ejemplo: “cinco nueves” = 99.999% de disponibilidad (~5 min de caída al año).

## 🔐 Seguridad

- Conjunto de **medidas y tecnologías** para proteger la red contra amenazas internas y externas.
- Incluye:
  - **Autenticación** (verificar identidad).
  - **Autorización** (control de acceso).
  - **Cifrado** (proteger datos en tránsito).
  - **Firewalls**, **IDS/IPS**, **VPNs**.
- Es esencial para garantizar:
  - Integridad, confidencialidad y disponibilidad de los datos.
 
## Diseño de Red Centralizado vs Distribuido

## 🏢 Diseño de Red Centralizado

### ✅ Ventajas:
- **Gestión simplificada**: Control centralizado de usuarios, configuraciones, políticas y servicios.
- **Coste más bajo en infraestructura**: Menos dispositivos de procesamiento distribuidos.
- **Seguridad más controlada**: Al concentrar los datos y accesos, es más fácil aplicar políticas de seguridad.
- **Fácil mantenimiento**: Solo se necesita actualizar o mantener la infraestructura del centro de control.

### ❌ Inconvenientes:
- **Punto único de fallo**: Si cae el servidor central, toda la red puede quedar inutilizada.
- **Mayor latencia**: Especialmente si los clientes están geográficamente dispersos.
- **Escalabilidad limitada**: Puede volverse ineficiente al aumentar el número de usuarios o servicios.
- **Cuello de botella**: Alta carga en el nodo central puede degradar el rendimiento.

---

## 🧩 Diseño de Red Distribuido

### ✅ Ventajas:
- **Alta disponibilidad y fiabilidad**: No depende de un único punto; si un nodo falla, otros pueden asumir el control.
- **Mejor escalabilidad**: Se pueden añadir nodos o servicios sin afectar el rendimiento global.
- **Rendimiento optimizado**: Reducción de la latencia al estar los servicios más cerca de los usuarios.
- **Distribución de carga**: El tráfico se reparte entre múltiples servidores/nodos.

### ❌ Inconvenientes:
- **Mayor complejidad de gestión**: Requiere herramientas avanzadas para la monitorización y sincronización entre nodos.
- **Coste inicial más alto**: Mayor inversión en hardware, software y personal técnico.
- **Seguridad más difícil de controlar**: Superficie de ataque mayor, ya que hay más puntos de entrada posibles.
- **Sincronización de datos**: Riesgo de inconsistencias si no se diseña correctamente.

---

## 📌 Conclusión

- Un **diseño centralizado** es útil para entornos pequeños, homogéneos o con recursos limitados.
- Un **diseño distribuido** es ideal para organizaciones grandes, con múltiples ubicaciones o que requieran alta disponibilidad y escalabilidad.


# Redes corporativas

https://www.redirisnova.es/antecedentes.html

