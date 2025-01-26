# **Monitorización del Rendimiento**

---
***La monitorización del rendimiento es fundamental para garantizar la eficiencia y estabilidad de los sistemas informáticos. Esta práctica permite identificar el uso de recursos como la CPU, la memoria, el disco y la red, ayudando a detectar cuellos de botella y optimizar procesos. En sistemas Linux, existen herramientas de línea de comandos que proporcionan datos en tiempo real sobre el rendimiento general del sistema. En esta presentación, exploraremos algunos de los comandos más utilizados para analizar y mejorar el rendimiento, asegurando un funcionamiento óptimo del sistema.***

<p align="center">
  <img src="/imagenes/ojo.jpg" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando SAR**
 
Se utiliza para monitorizar el rendimiento del sistema. Proporciona información detallada sobre el uso de la CPU, la memoria, las estadísticas de E/S de bloques, las estadísticas de red, la cola de carga, los dispositivos y el intercambio de memoria. Esto nos permite conocer el estado y el rendimiento del sistema en tiempo real.

---
- **sar**

Nos mostrará un resumen de las estadísticas del sistema desde el inicio del día hasta el momento actual. Esto incluye información sobre el uso de la CPU, la memoria, las estadísticas de E/S de bloques, las estadísticas de red, la cola de carga, los dispositivos y el intercambio de memoria. Esto nos permitirá conocer el estado y el rendimiento del sistema en tiempo real.

<p align="center">
  <img src="/imagenes/sar.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **sar-help**

Nos muestra una lista de todas las opciones disponibles para el comando sar, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando y cómo se pueden utilizar las diferentes opciones para monitorizar distintos aspectos del sistema. Entre las opciones más comunes se encuentran el análisis del uso de la CPU, memoria, disco, red, y otros recursos, tanto en tiempo real como a partir de registros históricos. De esta forma, podemos seleccionar las opciones adecuadas para obtener información detallada sobre el rendimiento y actividad del sistema.

<p align="center">
  <img src="/imagenes/sar-help.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando GLANCES**

Es una herramienta de monitoreo del sistema que proporciona una visión general del rendimiento del sistema en tiempo real. Muestra información sobre el uso de la CPU, la memoria, el disco, la red y otros recursos del sistema. Es una herramienta muy útil para los administradores de sistemas que necesitan monitorear el rendimiento del sistema de manera eficiente.

---
- **glances**

Sin opciones, obtendremos una visión general del rendimiento del sistema en tiempo real. Nos mostrará información sobre el uso de la CPU, la memoria, el disco, la red y otros recursos del sistema. Es una herramienta muy útil para los administradores de sistemas que necesitan monitorear el rendimiento del sistema de manera eficiente.

<p align="center">
  <img src="/imagenes/glances.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **glances --help**

Mostrará una lista de todas las opciones disponibles para el comando glances, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando y cómo se pueden utilizar las diferentes opciones para monitorear el rendimiento del sistema de manera eficiente.

## **Comando SMEM**

Es una herramienta de monitoreo de memoria que proporciona un desglose detallado del uso de la memoria en el sistema. A diferencia de otras herramientas de monitoreo de memoria, smem puede mostrar el uso de la memoria física y virtual por proceso, lo que permite a los administradores de sistemas identificar qué procesos están consumiendo más memoria.

---
- **smem**

Obtendremos un desglose detallado del uso de la memoria en el sistema. Nos mostrará información sobre la memoria física y virtual utilizada por cada proceso, lo que permite identificar qué procesos están consumiendo más memoria. Esto es útil para los sistemas que necesitan monitorear y optimizar el uso de la memoria en el sistema.  

- **smem --help**

Nos muestra una lista de todas las opciones disponibles para el comando smem, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando, que se centra en mostrar el uso de memoria por procesos en el sistema. Entre las opciones, se incluyen formas de personalizar la salida, como ordenar los resultados, seleccionar columnas específicas, cambiar la unidad de medida (kilobytes, megabytes, etc.) y mostrar gráficos de uso. Esto permite analizar de manera precisa cómo se distribuye y utiliza la memoria en el sistema.

---
## **Comando BMON**

Es una herramienta de monitoreo y depuración de red basada en texto para sistemas tipo Unix. Captura estadísticas relacionadas con la red y las muestra visualmente en un formato amigable en tiempo real2. Es útil para controlar el ancho de banda y detectar posibles problemas en la red.

---
- **bmon**

Sin opciones, obtendremos una visualización en tiempo real del rendimiento de la red. Nos muestra información sobre el tráfico de red, el ancho de banda utilizado, las tasas de transferencia y otros datos relevantes para cada interfaz de red. Es una herramienta muy útil para quienes necesitan monitorear y depurar problemas de red de manera eficiente.

- **bmon --help**

Nos muestra una lista de todas las opciones disponibles para el comando, junto con una breve descripción de cada una. Se utiliza para monitorizar en tiempo real el tráfico de red en el sistema, proporcionando información detallada sobre las interfaces de red y el uso del ancho de banda. Las opciones disponibles permiten personalizar la visualización, como elegir entre diferentes salidas (texto o gráficos), filtrar interfaces específicas, ajustar los intervalos de actualización, y definir las unidades de medida. Esta ayuda es ideal para configurar bmon según las necesidades de monitorización de red del usuario.

---
## **  Comando MPSTAT**

se utiliza para informar sobre las estadísticas de la CPU. Proporciona información detallada sobre el uso de la CPU, incluyendo métricas como el porcentaje de tiempo que la CPU está inactiva, el porcentaje de tiempo que la CPU está ocupada en modo de usuario, el porcentaje de tiempo que la CPU está ocupada en modo de sistema, entre otros. Esto permite a los administradores de sistemas identificar posibles cuellos de botella y optimizar el rendimiento de la CPU de manera más efectiva.

---
- **mpstat**

Obtendremos estadísticas de la CPU para todos los procesadores en tu sistema. Nos proporcionará información detallada sobre el uso de la CPU, incluyendo métricas como el porcentaje de tiempo que la CPU está inactiva, el porcentaje de tiempo que la CPU está ocupada en modo de usuario, el porcentaje de tiempo que la CPU está ocupada en modo de sistema, entre otros. Esto permite identificar posibles cuellos de botella y optimizar el rendimiento de la CPU de manera más efectiva.

- **mpstat --help**

Nos muestra una lista de todas las opciones disponibles para el comando, junto con una breve descripción de cada una. Este comando es útil para monitorizar el uso de la CPU, tanto globalmente como por núcleo, y proporciona estadísticas detalladas como el porcentaje de tiempo dedicado a tareas de usuario, sistema, inactividad, y más. Entre sus opciones se incluyen la capacidad de especificar intervalos de tiempo, filtrar la salida para CPU específicas y ajustar el formato de los datos. Esta ayuda permite al usuario configurar mpstat para analizar de manera precisa el rendimiento de los procesadores en el sistema.

---
## **Comando VMSTAT**

Se utiliza para informar sobre las estadísticas de la memoria virtual del sistema. Nos proporciona información detallada sobre el uso de la memoria, la paginación, los procesos, el intercambio y la actividad de la CPU. Esto nos permite identificar posibles cuellos de botella y optimizar el rendimiento del sistema de manera más efectiva.

---
- **vmstat**

obtendremos un resumen del rendimiento del sistema en tiempo real. Nos mostrará información sobre la memoria, la paginación, los procesos, el intercambio y la actividad de la CPU. Esto nos permite identificar posibles cuellos de botella y optimizar el rendimiento del sistema de manera más efectiva.

- **vmstat --help**

Muestra una lista de todas las opciones disponibles para el comando vmstat, junto con una breve descripción de cada una. Este comando es útil para obtener estadísticas sobre el rendimiento general del sistema, como el uso de la CPU, memoria, intercambio (swap), entrada/salida de disco y carga del sistema. Entre sus opciones, permite especificar intervalos de tiempo para actualizaciones, personalizar columnas en la salida, y habilitar información más detallada para diagnósticos específicos. Esta ayuda sirve para adaptar el uso de vmstat a necesidades concretas de monitorización del sistema.

---
## **Comando PIDSTAT**

Se utiliza para monitorear las estadísticas de los procesos en el sistema. Proporcionará información detallada sobre el uso de la CPU, la memoria y otros recursos por cada proceso en ejecución. Esto nos permite identificar qué procesos están consumiendo más recursos y optimizar el rendimiento del sistema de manera más efectiva.

- **pidstat**

Obtendremos estadísticas detalladas sobre el uso de la CPU por cada proceso en ejecución en el sistema. Esto incluye información sobre el porcentaje de tiempo que cada proceso está utilizando la CPU, lo que permite identificar qué procesos están consumiendo más recursos y optimizar el rendimiento del sistema de manera más efectiva.

- **pidstat --help**

Nos mostrará una lista de todas las opciones disponibles, junto con una breve descripción de cada una. Este comando es útil para monitorizar el uso de recursos por proceso, proporcionando estadísticas detalladas como el uso de CPU, memoria, disco y más, clasificadas por PID. Las opciones permiten personalizar la salida, como mostrar métricas específicas (I/O, memoria, hilos), definir intervalos y repeticiones, o incluir información de procesos inactivos. Esta ayuda permite configurar pidstat de manera flexible para analizar el rendimiento de procesos individuales o del sistema en su conjunto.

---
## **Comando DSTAT**

Es una herramienta versátil de monitoreo del sistema que combina la funcionalidad de varias herramientas de monitoreo en una sola. Proporciona información en tiempo real sobre el uso de la CPU, la memoria, el disco, la red y otros recursos del sistema. Es especialmente útil para los administradores de sistemas que necesitan una visión completa del rendimiento del sistema en un solo lugar.

---
- **dstat**

Obtendremos una visualización en tiempo real del rendimiento del sistema. Nos mostrará información sobre el uso de la CPU, la memoria, el disco, la red y otros recursos del sistema.

- **dstat --help**

Las opciones permiten personalizar qué módulos o métricas se desean mostrar, como estadísticas de entrada/salida de disco, tráfico de red, consumo energético, entre otros. Además, ofrece configuraciones para ajustar el intervalo de actualización y exportar los datos a formatos compatibles con hojas de cálculo. Esta ayuda es ideal para adaptar dstat a necesidades específicas de monitorización del sistema.

---

<p align="center">
  <img src="/imagenes/rendi.jpg" alt="Descripción de la imagen" width="500"/>
</p> 

