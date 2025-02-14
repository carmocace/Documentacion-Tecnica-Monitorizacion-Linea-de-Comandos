# **Monitorización de Rendimiento del Sistema**

---
***La monitorización del rendimiento es fundamental para garantizar la eficiencia y estabilidad de los sistemas informáticos. Esta práctica permite identificar el uso de recursos como la CPU, la memoria, el disco y la red, ayudando a detectar cuellos de botella y optimizar procesos. En sistemas Linux, existen herramientas de línea de comandos que proporcionan datos en tiempo real sobre el rendimiento general del sistema. En esta presentación, exploraremos algunos de los comandos más utilizados para analizar y mejorar el rendimiento, asegurando un funcionamiento óptimo del sistema.***

<p align="center">
  <img src="/imagenes/image.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando SAR**
 
Se utiliza para monitorizar el rendimiento del sistema. Proporciona información detallada sobre el uso de la CPU, la memoria, las estadísticas de E/S de bloques, las estadísticas de red, la cola de carga, los dispositivos y el intercambio de memoria. Esto nos permite conocer el estado y el rendimiento del sistema en tiempo real.

---
## **OPCIONES:**

---
- **sar**

Nos mostrará un resumen de las estadísticas del sistema desde el inicio del día hasta el momento actual. Esto incluye información sobre el uso de la CPU, la memoria, las estadísticas de E/S de bloques, las estadísticas de red, la cola de carga, los dispositivos y el intercambio de memoria. Esto nos permitirá conocer el estado y el rendimiento del sistema en tiempo real.

<p align="center">
  <img src="/imagenes/sar.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **sar --help**

Nos muestra una lista de todas las opciones disponibles para el comando sar, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando y cómo se pueden utilizar las diferentes opciones para monitorizar distintos aspectos del sistema. Entre las opciones más comunes se encuentran el análisis del uso de la CPU, memoria, disco, red, y otros recursos, tanto en tiempo real como a partir de registros históricos. De esta forma, podemos seleccionar las opciones adecuadas para obtener información detallada sobre el rendimiento y actividad del sistema.

<p align="center">
  <img src="/imagenes/sar-help.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando GLANCES**

Es una herramienta de monitoreo del sistema que proporciona una visión general del rendimiento del sistema en tiempo real. Muestra información sobre el uso de la CPU, la memoria, el disco, la red y otros recursos del sistema. Es una herramienta muy útil para los administradores de sistemas que necesitan monitorear el rendimiento del sistema de manera eficiente.

---
## **OPCIONES:**

---
- **glances**

Sin opciones, obtendremos una visión general del rendimiento del sistema en tiempo real. Nos mostrará información sobre el uso de la CPU, la memoria, el disco, la red y otros recursos del sistema. Es una herramienta muy útil para los administradores de sistemas que necesitan monitorear el rendimiento del sistema de manera eficiente.

<p align="center">
  <img src="/imagenes/glances.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **glances --help**

Mostrará una lista de todas las opciones disponibles para el comando glances, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando y cómo se pueden utilizar las diferentes opciones para monitorear el rendimiento del sistema de manera eficiente.

<p align="center">
  <img src="/imagenes/glances-help.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando SMEM**

Es una herramienta de monitoreo de memoria que proporciona un desglose detallado del uso de la memoria en el sistema. A diferencia de otras herramientas de monitoreo de memoria, smem puede mostrar el uso de la memoria física y virtual por proceso, lo que permite a los administradores de sistemas identificar qué procesos están consumiendo más memoria. Se utiliza para analizar y reportar el uso de memoria en un sistema Linux. Proporciona información detallada sobre cómo se está utilizando la memoria por cada proceso, incluyendo memoria física y memoria compartida, con un enfoque visual y comprensible. Esto permite identificar procesos que consumen demasiados recursos y optimizar el rendimiento del sistema.

---
## **OPCIONES:**

---
- **smem**

Obtendremos un desglose detallado del uso de la memoria en el sistema. Nos mostrará información sobre la memoria física y virtual utilizada por cada proceso, lo que permite identificar qué procesos están consumiendo más memoria. Esto es útil para los sistemas que necesitan monitorear y optimizar el uso de la memoria en el sistema.

<p align="center">
  <img src="/imagenes/smem.png" alt="Descripción de la imagen" width="500"/>
</p>

- **smem --help**

Nos muestra una lista de todas las opciones disponibles para el comando smem, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando, que se centra en mostrar el uso de memoria por procesos en el sistema. Entre las opciones, se incluyen formas de personalizar la salida, como ordenar los resultados, seleccionar columnas específicas, cambiar la unidad de medida (kilobytes, megabytes, etc.) y mostrar gráficos de uso. Esto permite analizar de manera precisa cómo se distribuye y utiliza la memoria en el sistema.

<p align="center">
  <img src="/imagenes/smem-help.png" alt="Descripción de la imagen" width="500"/>
</p>

- **smem -u**

Nos muestra un desglose del uso de memoria por usuario en lugar de por proceso. Esto es particularmente útil cuando se quiere identificar qué usuarios están utilizando más recursos en el sistema. Presenta información como el total de memoria utilizada y cómo está distribuida entre los usuarios activos.

<p align="center">
  <img src="/imagenes/smem-u.png" alt="Descripción de la imagen" width="500"/>
</p>

- **smem -m**

Obtendremos un resumen de la memoria del sistema, incluyendo detalles de la memoria física total, usada y libre, así como la memoria compartida, de intercambio (swap) y buffers. Esta vista global es útil para evaluar rápidamente la disponibilidad de memoria del sistema.


<p align="center">
  <img src="/imagenes/smem-m.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **  Comando MPSTAT**

se utiliza para informar sobre las estadísticas de la CPU. Proporciona información detallada sobre el uso de la CPU, incluyendo métricas como el porcentaje de tiempo que la CPU está inactiva, el porcentaje de tiempo que la CPU está ocupada en modo de usuario, el porcentaje de tiempo que la CPU está ocupada en modo de sistema, entre otros. Esto permite a los administradores de sistemas identificar posibles cuellos de botella y optimizar el rendimiento de la CPU de manera más efectiva.

---
## **OPCIONES:**

---
- **mpstat**

Obtendremos estadísticas de la CPU para todos los procesadores en tu sistema. Nos proporcionará información detallada sobre el uso de la CPU, incluyendo métricas como el porcentaje de tiempo que la CPU está inactiva, el porcentaje de tiempo que la CPU está ocupada en modo de usuario, el porcentaje de tiempo que la CPU está ocupada en modo de sistema, entre otros. Esto permite identificar posibles cuellos de botella y optimizar el rendimiento de la CPU de manera más efectiva.

<p align="center">
  <img src="/imagenes/mpstat.png" alt="Descripción de la imagen" width="500"/>
</p>

- **mpstat --help**

Nos muestra una lista de todas las opciones disponibles para el comando, junto con una breve descripción de cada una. Este comando es útil para monitorizar el uso de la CPU, tanto globalmente como por núcleo, y proporciona estadísticas detalladas como el porcentaje de tiempo dedicado a tareas de usuario, sistema, inactividad, y más. Entre sus opciones se incluyen la capacidad de especificar intervalos de tiempo, filtrar la salida para CPU específicas y ajustar el formato de los datos. Esta ayuda permite al usuario configurar mpstat para analizar de manera precisa el rendimiento de los procesadores en el sistema.

<p align="center">
  <img src="/imagenes/mpstat-help.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando VMSTAT**

Se utiliza para informar sobre las estadísticas de la memoria virtual del sistema. Nos proporciona información detallada sobre el uso de la memoria, la paginación, los procesos, el intercambio y la actividad de la CPU. Esto nos permite identificar posibles cuellos de botella y optimizar el rendimiento del sistema de manera más efectiva.

---
## **OPCIONES:**

---
- **vmstat**

obtendremos un resumen del rendimiento del sistema en tiempo real. Nos mostrará información sobre la memoria, la paginación, los procesos, el intercambio y la actividad de la CPU. Esto nos permite identificar posibles cuellos de botella y optimizar el rendimiento del sistema de manera más efectiva.

<p align="center">
  <img src="/imagenes/vmstat.png" alt="Descripción de la imagen" width="500"/>
</p>

- **vmstat --help**

Muestra una lista de todas las opciones disponibles para el comando vmstat, junto con una breve descripción de cada una. Este comando es útil para obtener estadísticas sobre el rendimiento general del sistema, como el uso de la CPU, memoria, intercambio (swap), entrada/salida de disco y carga del sistema. Entre sus opciones, permite especificar intervalos de tiempo para actualizaciones, personalizar columnas en la salida, y habilitar información más detallada para diagnósticos específicos. Esta ayuda sirve para adaptar el uso de vmstat a necesidades concretas de monitorización del sistema.

<p align="center">
  <img src="/imagenes/vmstat-help.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando PIDSTAT**

Se utiliza para monitorear las estadísticas de los procesos en el sistema. Proporcionará información detallada sobre el uso de la CPU, la memoria y otros recursos por cada proceso en ejecución. Esto nos permite identificar qué procesos están consumiendo más recursos y optimizar el rendimiento del sistema de manera más efectiva.

---
## **OPCIONES:**

---
- **pidstat**

Obtendremos estadísticas detalladas sobre el uso de la CPU por cada proceso en ejecución en el sistema. Esto incluye información sobre el porcentaje de tiempo que cada proceso está utilizando la CPU, lo que permite identificar qué procesos están consumiendo más recursos y optimizar el rendimiento del sistema de manera más efectiva.

<p align="center">
  <img src="/imagenes/pidstat.png" alt="Descripción de la imagen" width="500"/>
</p>

- **pidstat --help**

Nos mostrará una lista de todas las opciones disponibles, junto con una breve descripción de cada una. Este comando es útil para monitorizar el uso de recursos por proceso, proporcionando estadísticas detalladas como el uso de CPU, memoria, disco y más, clasificadas por PID. Las opciones permiten personalizar la salida, como mostrar métricas específicas (I/O, memoria, hilos), definir intervalos y repeticiones, o incluir información de procesos inactivos. Esta ayuda permite configurar pidstat de manera flexible para analizar el rendimiento de procesos individuales o del sistema en su conjunto.

<p align="center">
  <img src="/imagenes/pidstat-help.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando DSTAT**

Es una herramienta versátil de monitoreo del sistema que combina la funcionalidad de varias herramientas de monitoreo en una sola. Proporciona información en tiempo real sobre el uso de la CPU, la memoria, el disco, la red y otros recursos del sistema. Es especialmente útil para los administradores de sistemas que necesitan una visión completa del rendimiento del sistema en un solo lugar.

---
## **OPCIONES:**

---
- **dstat**

Obtendremos una visualización en tiempo real del rendimiento del sistema. Nos mostrará información sobre el uso de la CPU, la memoria, el disco, la red y otros recursos del sistema.

<p align="center">
  <img src="/imagenes/dstat.png" alt="Descripción de la imagen" width="500"/>
</p>

- **dstat --help**

Las opciones permiten personalizar qué módulos o métricas se desean mostrar, como estadísticas de entrada/salida de disco, tráfico de red, consumo energético, entre otros. Además, ofrece configuraciones para ajustar el intervalo de actualización y exportar los datos a formatos compatibles con hojas de cálculo. Esta ayuda es ideal para adaptar dstat a necesidades específicas de monitorización del sistema.

<p align="center">
  <img src="/imagenes/dstat-help.png" alt="Descripción de la imagen" width="500"/>
</p>

---
<p align="center">
  <img src="/imagenes/ren.jpg" alt="Descripción de la imagen" width="500"/>
</p> 

