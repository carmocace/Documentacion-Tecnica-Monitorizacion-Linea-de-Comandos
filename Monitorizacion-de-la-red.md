
---
# **Monitorizacion de la Red**

***La monitorización de la red es vital para asegurar una comunicación eficiente y detectar posibles problemas de conectividad o de rendimiento en el sistema. Al controlar el tráfico de red, podemos identificar cuellos de botella, conexiones no deseadas o problemas de latencia. En sistemas Linux, existen diversos comandos que permiten observar el estado de la red, el uso del ancho de banda y la actividad de las interfaces de red. En esta presentación, exploraremos algunos de los comandos más utilizados para monitorizar el tráfico de red y mantener una red saludable y eficiente.***

<p align="center">
  <img src="/imagenes/red.jpg" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando NETSTAT**

Se utiliza para mostrar estadísticas de red y conexiones de red en el sistema. Proporciona información detallada sobre las conexiones de red activas, las tablas de enrutamiento, las interfaces de red y las estadísticas de protocolo. Es una herramienta muy útil para los administradores de sistemas que necesitan monitorear y depurar problemas de red de manera eficiente.

---
### **OPCIONES:**

---
- **netstat**

Obtendremos una lista de todas las conexiones de red activas en nuestro sistema. Esto incluye información sobre las conexiones TCP y UDP, las direcciones IP de origen y destino, los puertos y el estado de la conexión.

<p align="center">
  <img src="/imagenes/netstat.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat --help**

Obtenemos una lista completa de las opciones disponibles para el comando junto con una breve descripción de cada una. Esto ayuda a explorar sus funcionalidades, como listar conexiones activas, estadísticas de protocolos, tablas de enrutamiento, entre otros. Es una referencia esencial para aprovechar al máximo el comando y personalizar su uso.

<p align="center">
  <img src="/imagenes/nestat help.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat -a**

Nos muestra todas las conexiones activas y puertos en escucha del sistema. Esto incluye tanto las conexiones TCP y UDP activas como los puertos que están esperando nuevas conexiones. Es especialmente útil para identificar servicios en ejecución o detectar puertos abiertos.

<p align="center">
  <img src="/imagenes/nestat -a.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat -p**

Añade información sobre el proceso asociado a cada conexión activa o puerto en escucha. Muestra el identificador del proceso (PID) y el nombre del programa que está utilizando el socket. Esta información es útil para identificar qué aplicaciones están utilizando la red.

<p align="center">
  <img src="/imagenes/nestat -p.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat -tp**

La combinación -tp muestra las conexiones activas en el protocolo TCP junto con el proceso asociado a cada conexión. Es ideal para depurar problemas relacionados específicamente con conexiones TCP, como servicios que utilizan este protocolo o conexiones no autorizadas.

<p align="center">
  <img src="/imagenes/nestat -tp.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat -r**

Nos muestra la tabla de enrutamiento del sistema. Incluye detalles como destinos, puertas de enlace, interfaces de red y métricas asociadas. Esto es útil para verificar y gestionar las rutas que utiliza el sistema para enviar y recibir paquetes en la red.

<p align="center">
  <img src="/imagenes/netsatat2.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando TCPDUMP**

Es una herramienta de captura de paquetes que se utiliza para analizar el tráfico de red. Nos permite capturar y mostrar los paquetes que se transmiten o reciben a través de una red, proporcionando información detallada sobre el contenido de los paquetes, las direcciones IP de origen y destino, los puertos y otros datos relevantes. Es una herramienta muy útil para los administradores de sistemas y los profesionales de seguridad que necesitan monitorear y analizar el tráfico de red para detectar problemas o posibles amenazas.

---
### **OPCIONES:**

---
- **tcpdump**

Ejecutandolo sin opciones, obtendremos una captura de todos los paquetes que se transmiten o reciben a través de la red en el sistema. Esto incluye información detallada sobre el contenido de los paquetes, las direcciones IP de origen y destino, los puertos y otros datos relevantes.

 <p align="center">
  <img src="/imagenes/tcpdump.png" alt="Descripción de la imagen" width="500"/>
</p>

- **tcpdump --help**

Se muestra una lista completa de las opciones disponibles junto con una breve descripción de cada una. Esto es útil para conocer las funcionalidades del comando, como seleccionar interfaces, aplicar filtros, personalizar la captura o modificar el formato de salida. Es el primer paso para aprender y explorar el uso avanzado de la herramienta.

<p align="center">
  <img src="/imagenes/tcpdump help.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **tcpdump -i**

Permite especificar la interfaz de red en la que se realizará la captura de paquetes, como eth0, wlan0, o cualquier otra interfaz activa en el sistema. Si no se utiliza esta opción, tcpdump seleccionará la interfaz predeterminada. Esto es fundamental cuando se quiere limitar la captura a una red específica.

<p align="center">
  <img src="/imagenes/tcpdump -i.png" alt="Descripción de la imagen" width="500"/>
</p>

- **tcpdump -Z**

 Nos permite ejecutar un comando específico sobre cada archivo de captura cuando se rota (por ejemplo, mediante la opción -C o -G para rotación de archivos). Esto se usa comúnmente para comprimir automáticamente los archivos rotados o procesarlos de alguna manera.

<p align="center">
  <img src="/imagenes/tcpdump -Z.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando TCPTRACK**

Es una herramienta de monitoreo de conexiones TCP en tiempo real. Muestra información sobre las conexiones TCP activas en el sistema, incluyendo el estado de la conexión, la dirección IP de origen y destino, y la cantidad de datos transferidos. Es útil para monitorear y depurar problemas de red de manera eficiente.

---
### **OPCIONES:**

---
- **tcptrack**

Ejecutado sin opciones, obtendremos una visualización en tiempo real de las conexiones TCP activas en nuestro sistema. Nos mostrará información sobre el estado de la conexión, la dirección IP de origen y destino, y la cantidad de datos transferidos.

 <p align="center">
  <img src="/imagenes/tcptrack.png" alt="Descripción de la imagen" width="500"/>
</p>

- **tcptrack -i**

Nos permite especificar la interfaz de red en la que tcptrack observará las conexiones TCP. Esto es necesario para que el comando sepa en qué interfaz monitorear el tráfico. Si no se proporciona una interfaz, tcptrack no podrá funcionar y mostrará un mensaje de error.
  
 <p align="center">
  <img src="/imagenes/tcptrack -i enp0s3.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando IPTRAF**

Es una herramienta de monitoreo de red en tiempo real que proporciona estadísticas detalladas sobre el tráfico de red. Muestra información sobre las conexiones TCP, UDP, ICMP y otros protocolos, así como estadísticas de tráfico por interfaz de red. Es especialmente útil para los administradores de sistemas que necesitan monitorear y analizar el tráfico de red para detectar problemas o posibles amenazas.

---
### **OPCIONES:**

---
- **iptraf --help**

Nos muestra un resumen de las opciones disponibles para el comando iptraf, junto con una breve descripción de su funcionalidad. Es útil para obtener una visión general de las capacidades de la herramienta y aprender cómo utilizar sus características.

<p align="center">
  <img src="/imagenes/iptraf 2.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **iptraf -ng**

IPTraf-NG (Next Generation), es una versión mejorada de la herramienta IPTraf, que proporciona estadísticas detalladas sobre el tráfico de red en tiempo real. Esta herramienta basada en la consola permite monitorear y analizar el tráfico de red de manera eficiente. Algunas de las características de IPTraf-NG incluyen:

1.- Monitor de tráfico IP que muestra información detallada sobre el tráfico que circula por la red.

2.- Estadísticas detalladas sobre los paquetes IP, TCP, UDP, ICMP y otros protocolos.

3.- Monitor de paquetes entrantes y salientes en los puertos comunes de ciertas aplicaciones.

4.- Módulo de estadísticas para la red local que muestra los hosts activos y la actividad de los datos.

5.- Filtros para mostrar solo conexiones por TCP, UDP y otros protocolos.

6.- Soporte para interfaces Ethernet, SLIP, PPP y otras

<p align="center">
  <img src="/imagenes/iptraf-ng.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando Bandwithd**


---
- **bandwithd**

Es una herramienta que monitoriza el uso de ancho de banda en redes, generando informes detallados y gráficos. A diferencia de herramientas en tiempo real como tcpdump o tcptrack, bandwidthd registra estadísticas a lo largo del tiempo y las presenta en una interfaz web. Permite a los administradores de red rastrear el consumo de ancho de banda por IP, protocolo o puerto.

**Características principales de bandwidthd:**
- **Monitoreo por IP:** Registra el tráfico entrante y saliente por dirección IP.
- **Reportes web:** Genera páginas HTML y gráficos que detallan el uso del ancho de banda.
- **Soporte de filtros:** Permite aplicar filtros basados en direcciones IP, subredes, protocolos, etc.
- **Base de datos:** Los datos pueden almacenarse en bases de datos como PostgreSQL o MySQL para análisis avanzado.

<p align="center">
  <img src="/imagenes/bandwithd.png" alt="Descripción de la imagen" width="500"/>
</p> 

<p align="center">
  <img src="/imagenes/band2.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando NLOAD**

Es una herramienta que se utiliza para monitorear el tráfico de red y el uso del ancho de banda en tiempo real. Visualiza el tráfico entrante y saliente utilizando gráficos y proporciona información adicional como la cantidad total de datos transferidos y el uso mínimo/máximo de la red

- **OPCIONES:**

---
- **nload**

Obtendremos una visualización en tiempo real del tráfico de red y el uso del ancho de banda.Nos muestra gráficos del tráfico entrante y saliente, así como información adicional como la cantidad total de datos transferidos y el uso mínimo/máximo de la red. Es una herramienta muy útil para quienes necesitan monitorear el rendimiento de la red de manera eficiente.

<p align="center">
  <img src="/imagenes/nload.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **nload --help**

Nos muestra una lista de todas las opciones disponibles, junto con una breve descripción de cada una. Se utiliza para monitorizar en tiempo real el tráfico de red, mostrando gráficos interactivos del ancho de banda utilizado para descarga (inbound) y subida (outbound). Las opciones permiten configurar aspectos como la interfaz de red que se desea monitorizar, el intervalo de actualización, las unidades de medida (bits o bytes), y ajustes visuales como los colores o el escalado automático. Esta ayuda facilita personalizar nload para realizar un seguimiento eficiente del tráfico de red según las necesidades del usuario.

<p align="center">
  <img src="/imagenes/nload-help.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando BMON**

Es una herramienta de monitoreo y depuración de red basada en texto para sistemas tipo Unix. Captura estadísticas relacionadas con la red y las muestra visualmente en un formato amigable en tiempo real2. Es útil para controlar el ancho de banda y detectar posibles problemas en la red.

---
- **OPCIONES:**

---
- **bmon**

Sin opciones, obtendremos una visualización en tiempo real del rendimiento de la red. Nos muestra información sobre el tráfico de red, el ancho de banda utilizado, las tasas de transferencia y otros datos relevantes para cada interfaz de red. Es una herramienta muy útil para quienes necesitan monitorear y depurar problemas de red de manera eficiente.

<p align="center">
  <img src="/imagenes/bmon.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **bmon --help**

Nos muestra una lista de todas las opciones disponibles para el comando, junto con una breve descripción de cada una. Se utiliza para monitorizar en tiempo real el tráfico de red en el sistema, proporcionando información detallada sobre las interfaces de red y el uso del ancho de banda. Las opciones disponibles permiten personalizar la visualización, como elegir entre diferentes salidas (texto o gráficos), filtrar interfaces específicas, ajustar los intervalos de actualización, y definir las unidades de medida. Esta ayuda es ideal para configurar bmon según las necesidades de monitorización de red del usuario.

<p align="center">
  <img src="/imagenes/bmon-help.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando PING**

se utiliza para verificar la conectividad de red entre dos dispositivos. Envía paquetes de solicitud de eco ICMP a un host específico y espera una respuesta. Esto nos permite determinar si un dispositivo está accesible en la red y medir el tiempo de respuesta.

---
- **OPCIONES:**

---
- **ping --help**

se muestra una lista completa de las opciones disponibles para el comando, junto con una breve descripción de su propósito. Esto permite explorar las funcionalidades del comando y personalizar su uso según las necesidades.

<p align="center">
  <img src="/imagenes/ping-help.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
- **ping -c**

La opción -c permite especificar el número de paquetes de solicitud de eco que se enviarán. Por ejemplo, si deseas enviar 4 paquetes de solicitud de eco, puedes usar el comando ping -c 4 <dirección IP o nombre de host>.

<p align="center">
  <img src="/imagenes/ping.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
<p align="center">
  <img src="/imagenes/redes2.jpg" alt="Descripción de la imagen" width="500"/>
</p> 

---
