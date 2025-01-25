
---
# **Monitorización de Procesos**

***La monitorización de procesos es crucial para gestionar de manera eficiente los recursos del sistema y garantizar que las aplicaciones se ejecuten correctamente. A través de esta práctica, podemos identificar qué procesos están consumiendo más recursos, como la CPU o la memoria, y tomar decisiones para optimizar el rendimiento.
En sistemas Linux, existen diversos comandos que permiten ver, controlar y analizar los procesos en ejecución. En esta presentación, exploraremos algunos de los comandos más utilizados para monitorizar y gestionar procesos de manera efectiva.***

<p align="center">
  <img src="/imagenes/integracion_datos_monitorizacion_pic01_20240228_blog_equimed.jpg" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando PS**

El comando ps en Linux tiene muchas opciones útiles para mostrar información sobre los procesos en ejecución. Muestra una lista que incluye información básica sobre cada proceso, como el ID del proceso (PID), el terminal asociado (TTY), el tiempo de CPU utilizado (TIME) y el comando que inició el proceso (CMD).Algunas de las opciones más comunes son:

---
### **Opciones:**

---
- **ps**

El comando ps ejecutado sin ninguna opción extra muestra una lista de los procesos que están actualmente en ejecución en la terminal desde la cual se ejecutó el comando. 
  
<p align="center">
  <img src="/imagenes/1.jpg" alt="Descripción de la imagen" width="200"/>
</p>

- **ps a** 

Muestra una lista de todos los procesos que están actualmente en ejecución en el sistema, incluyendo aquellos que no están asociados a un terminal específico. 
  
<p align="center">
  <img src="/imagenes/2.png" alt="Descripción de la imagen" width="500"/>
</p>

- **ps aux**

Muestra una lista detallada de todos los procesos que están actualmente en ejecución en el sistema. Esta lista incluye información más completa sobre cada proceso, como el ID del proceso (PID), el usuario que inició el proceso (USER), el porcentaje de uso de la CPU (%CPU), el porcentaje de uso de la memoria (%MEM), el tamaño de la memoria virtual utilizada (VSZ), el tamaño de la memoria residente (RSS), el estado del proceso (STAT), el tiempo de CPU utilizado (TIME) y el comando que inició el proceso (COMMAND).

<p align="center">
  <img src="/imagenes/3.png" alt="Descripción de la imagen" width="500"/>
</p>

- **ps -C**

Se utiliza para mostrar información sobre los procesos que coinciden con un nombre de comando específico. Debemos proporcionar el nombre del comando como argumento.

<p align="center">
  <img src="/imagenes/4.png" alt="Descripción de la imagen" width="500"/>
</p>

- **ps -u**

Muestra una lista de los procesos que están actualmente en ejecución en el sistema, filtrados por el usuario especificado. Debemoss proporcionar el nombre del usuario como argumento.

<p align="center">
  <img src="/imagenes/5.png" alt="Descripción de la imagen" width="500"/>
</p>

- **ps -p**

Se utiliza para mostrar información sobre procesos específicos, filtrados por el ID del proceso (PID) que especifiquemoss. Debemos proporcionar el PID como argumento.

<p align="center">
  <img src="/imagenes/6.png" alt="Descripción de la imagen" width="500"/>
</p>

- **ps -x**

Muestra una lista de todos los procesos que están actualmente en ejecución en el sistema, incluyendo aquellos que no están asociados a un terminal específico.

<p align="center">
  <img src="/imagenes/7.png" alt="Descripción de la imagen" width="400"/>
</p>

- **ps -a**

Muestra una lista de todos los procesos que están actualmente en ejecución en el sistema, no solo los asociados a la terminal desde la cual se ejecutó el comando. 
  
<p align="center">
  <img src="/imagenes/8.png" alt="Descripción de la imagen" width="300"/>
</p>

- **ps -e** o **ps -A**

Muestra una lista de todos los procesos que están actualmente en ejecución en el sistema, no solo los asociados a la terminal desde la cual se ejecutó el comando.

<p align="center">
  <img src="/imagenes/9.png" alt="Descripción de la imagen" width="300"/>
</p>

- **ps -o**

se utiliza para personalizar la salida del comando ps, permitiéndonos especificar qué columnas de información deseamos ver sobre los procesos en ejecución. Debemos proporcionar una lista de columnas como argumento.

<p align="center">
  <img src="/imagenes/10.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando TOP** 

*El comando top se utiliza para mostrar una lista dinámica y en tiempo real de los procesos que están actualmente en ejecución en el sistema. Proporciona una visión general del uso de la CPU, la memoria y otros recursos del sistema, permitiendo a los administradores de sistemas monitorear el rendimiento y la actividad del sistema en tiempo real.*

---
### **Opciones:**

---
- **top**

Cuando ejecutamos el comando top sin ninguna opción extra, obtenemos una interfaz interactiva que se actualiza periódicamente y nos muestra información detallada sobre los procesos en ejecución.

<p align="center">
  <img src="/imagenes/11.png" alt="Descripción de la imagen" width="500"/>
</p>

- **top -d**

Se utiliza para especificar el intervalo de actualización en segundos para la salida del comando top. Esto nos permite controlar con qué frecuencia se actualiza la información mostrada en la interfaz interactiva de top.

<p align="center">
  <img src="/imagenes/12.png" alt="Descripción de la imagen" width="500"/>
</p>

- **top -p**

Se utiliza para mostrar información sobre procesos específicos, filtrados por el ID del proceso (PID) que especifiquemoss. Debemoss proporcionar el PID como argumento. Esto nos permite monitorear en tiempo real solo los procesos que coinciden con el PID que especificamos.

<p align="center">
  <img src="/imagenes/13.png" alt="Descripción de la imagen" width="500"/>
</p>

- **top -u**

Se utiliza para mostrar información sobre los procesos que están actualmente en ejecución en el sistema, filtrados por el usuario especificado. Debemos proporcionar el nombre del usuario como argumento. Esto nos permite monitorear en tiempo real solo los procesos que pertenecen al usuario especificado.

<p align="center">
  <img src="/imagenes/14.png" alt="Descripción de la imagen" width="500"/>
</p>

- **top -b**

top -b
El comando top -b se utiliza para ejecutar top en modo batch, lo que significa que la salida se genera en un formato adecuado para ser guardada en un archivo o procesada por otros programas. Este modo es útil para capturar la salida de top en un archivo para su análisis posterior.

<p align="center">
  <img src="/imagenes/15.png" alt="Descripción de la imagen" width="400"/>
</p>

- **top -r**

Se utiliza para invertir el orden de clasificación de la salida del comando top. Esto significa que si la salida de top está ordenada de manera ascendente por una columna específica, el uso de top -r la ordenará de manera descendente, y viceversa.


<p align="center">
  <img src="/imagenes/17 -r.png" alt="Descripción de la imagen" width="400"/>
</p>

- **top -k**

Se utiliza para enviar una señal a un proceso específico, lo que generalmente se usa para finalizar un proceso. Debemoss proporcionar el ID del proceso (PID) como argumento y la señal que deseamos enviar. Por defecto, la señal es SIGTERM, que solicita al proceso que termine de manera ordenada.

<p align="center">
  <img src="/imagenes/17kill.png" alt="Descripción de la imagen" width="400"/>
</p>

---
## **Comando ATOP**

*El comando atop es una herramienta avanzada de monitorización de sistemas que proporciona una visión detallada y en tiempo real del uso de recursos del sistema, como la CPU, la memoria, el disco y la red. A diferencia de otras herramientas de monitorización, atop puede registrar la actividad del sistema en intervalos regulares y guardar estos registros para su análisis posterior.*

---
### **Opciones:**

---
- **atop**

Sin ninguna opción extra, obtenemos una interfaz interactiva que se actualiza periódicamente y nos muestra información detallada sobre los procesos en ejecución y el uso de recursos del sistema.

<p align="center">
  <img src="/imagenes/15.png" alt="Descripción de la imagen" width="400"/>
</p>

- **atop -a**

Se utiliza para mostrar información detallada sobre todos los procesos y recursos del sistema, incluyendo aquellos que han terminado durante el intervalo de muestreo. Esto proporciona una visión más completa del uso de recursos y de los procesos que han estado activos en el sistema.

Obtenemos una interfaz interactiva que se actualiza periódicamente y nos muestra información detallada sobre los procesos en ejecución, los procesos que han terminado y el uso de recursos del sistema.

<p align="center">
  <img src="/imagenes/atop -a.png" alt="Descripción de la imagen" width="400"/>
</p>

- **atop c**

Se utiliza para mostrar la línea de comando completa con la que se inició cada proceso en la salida de atop. Esto proporciona una visión más detallada de los procesos en ejecución, incluyendo los argumentos de la línea de comando que se utilizaron para iniciarlos.

Obtenemos una interfaz interactiva que se actualiza periódicamente y nos muestra información detallada sobre los procesos en ejecución, incluyendo la línea de comando completa.

<p align="center">
  <img src="/imagenes/atop c.png" alt="Descripción de la imagen" width="400"/>
</p>

- **atop -d**

Se utiliza para especificar el intervalo de actualización en segundos para la salida del comando atop. Esto nos permite controlar con qué frecuencia se actualiza la información mostrada en la interfaz interactiva de atop.

<p align="center">
  <img src="/imagenes/atop -d.png" alt="Descripción de la imagen" width="400"/>
</p>

- **atop m**

Se utiliza para mostrar información detallada sobre el uso de memoria de los procesos en ejecución. Esto nos proporciona una visión más profunda de cómo se está utilizando la memoria en el sistema, incluyendo la memoria virtual, la memoria residente y la memoria compartida.

Obtenemoss una interfaz interactiva que se actualiza periódicamente y nos muestra información detallada sobre el uso de memoria de los procesos en ejecución.

<p align="center">
  <img src="/imagenes/atop m.png" alt="Descripción de la imagen" width="400"/>
</p>

- **atop -m**

Se utiliza para mostrar información aún más detallada sobre el uso de memoria de los procesos en ejecución. Esto nos proporciona una visión más profunda de cómo se está utilizando la memoria en el sistema, incluyendo la memoria virtual, la memoria residente y la memoria compartida.

Obtenemos una interfaz interactiva que se actualiza periódicamente y nos  muestra información detallada sobre el uso de memoria de los procesos en ejecución.

<p align="center">
  <img src="/imagenes/atop -m.png" alt="Descripción de la imagen" width="400"/>
</p>

- **atop -n**

Se utiliza para especificar el número de actualizaciones que deseamoss ver antes de que atop termine automáticamente. Esto es útil si deseamos ejecutar atop durante un número específico de intervalos de actualización y luego salir automáticamente.

<p align="center">
  <img src="/imagenes/atop -n.png" alt="Descripción de la imagen" width="400"/>
</p>

- **atop -p**

Se utiliza para mostrar información detallada sobre procesos específicos, filtrados por el ID del proceso (PID) que especifiquemos. Debemos proporcionar el PID como argumento. Esto nos permite monitorear en tiempo real solo los procesos que coinciden con el PID que especificamos.

<p align="center">
  <img src="/imagenes/atop -p 2829.png" alt="Descripción de la imagen" width="400"/>
</p>

- **atop -u**

Se utiliza para mostrar información detallada sobre el uso de CPU de los procesos en ejecución, ordenados por el porcentaje de uso de la CPU. Esto nos proporciona una visión más profunda de cómo se está utilizando la CPU en el sistema, permitiéndonos identificar los procesos que están consumiendo más recursos de CPU.

Obtenemos una interfaz interactiva que se actualiza periódicamente y nos muestra información detallada sobre el uso de CPU de los procesos en ejecución.

<p align="center">
  <img src="/imagenes/atop -u.png" alt="Descripción de la imagen" width="400"/>
</p>

---
## **Comando HTOP**

*El comando htop es una herramienta interactiva de monitorización de procesos que proporciona una visión en tiempo real del uso de recursos del sistema, como la CPU, la memoria y el disco. A diferencia de top, htop ofrece una interfaz más amigable y colorida, con opciones de navegación y filtrado más avanzadas.
Cuando instalamoss el comando htop, se instalará junto al comando, una aplicación que podremos ejecutar desde la interfaz grágica.*

<p align="center">
  <img src="/imagenes/htop icono.png" alt="Descripción de la imagen" width="400"/>
</p>

---
### **Opciones:**

---
- **htop**
 
Sin ninguna opción extra, obtemneos una interfaz interactiva que se actualiza periódicamente y nos muestra información detallada sobre los procesos en ejecución. 

<p align="center">
  <img src="/imagenes/htop.png" alt="Descripción de la imagen" width="400"/>
</p>

- **htop -u**

Se utiliza para filtrar y mostrar solo los procesos que pertenecen a un usuario específico. Debemos proporcionar el nombre del usuario como argumento. Esto nos permite monitorear en tiempo real solo los procesos que pertenecen al usuario especificado.

<p align="center">
  <img src="/imagenes/htop -u.png" alt="Descripción de la imagen" width="400"/>
</p>

- **htop -p**

Se utiliza para mostrar información detallada sobre procesos específicos, filtrados por el ID del proceso (PID) que especifiquemos. Debes proporcionar el PID como argumento. Esto nos permite monitorear en tiempo real solo los procesos que coinciden con el PID que especificamos.

<p align="center">
  <img src="/imagenes/htop -p 2928.png" alt="Descripción de la imagen" width="400"/>
</p>

- **htop -t**

Se utiliza para mostrar la salida de htop en modo árbol, lo que significa que los procesos se organizan jerárquicamente según su relación padre-hijo. Esto nos permite ver la estructura de los procesos y cómo están relacionados entre sí.

<p align="center">
  <img src="/imagenes/htop -t.png" alt="Descripción de la imagen" width="400"/>
</p>
