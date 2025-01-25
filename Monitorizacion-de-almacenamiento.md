
---
# **Monitorizacion de almacenamiento**

***La monitorización de almacenamiento es esencial para garantizar que los sistemas tengan suficiente espacio disponible y funcionen de manera eficiente. Al supervisar el uso del disco, podemos identificar problemas como la saturación del espacio o la presencia de archivos innecesarios que podrían afectar el rendimiento. En sistemas Linux, existen varias herramientas que permiten ver el estado de las particiones, el espacio libre y ocupado, y otros detalles importantes sobre el almacenamiento. En esta presentación, exploraremos algunos de los comandos más útiles para monitorizar el almacenamiento y gestionar de manera adecuada los recursos del disco.***

---
## **Comando DF**

*Se utiliza para mostrar el uso del espacio en disco en los sistemas de archivos montados. Proporciona información detallada sobre la cantidad de espacio total, usado y disponible en cada sistema de archivos, así como el porcentaje de uso. Esto nos permite conocer el estado y la capacidad de almacenamiento en tiempo real.*

---
### **Opciones:**

---
- **df**

Si ejecutamos el comando df sin opciones extra, nos mostrará un resumen del uso del espacio en disco para todos los sistemas de archivos montados en tu sistema. Nos proporcionará información detallada sobre la cantidad de espacio total, usado y disponible en cada sistema de archivos, así como el punto de montaje correspondiente. Esto permite a los administradores de sistemas conocer el estado y la capacidad de almacenamiento de todos los sistemas de archivos en tiempo real.

<p align="center">
  <img src="/imagenes/df.png" alt="Descripción de la imagen" width="500"/>
</p>

- **df --help**

Nos muestra una lista de todas las opciones disponibles para el comando df, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando y cómo se pueden utilizar las diferentes opciones para obtener información específica el estado y la capacidad de almacenamiento de todos los sistemas de archivos.
  
<p align="center">
  <img src="/imagenes/df help.png" alt="Descripción de la imagen" width="500"/>
</p>

- **df -h**

Se utiliza para mostrar el uso del espacio en disco en un formato legible para humanos. Nos proporciona información detallada sobre la cantidad de espacio total, usado y disponible en cada sistema de archivos, así como el porcentaje de uso, utilizando unidades como KB, MB o GB. Esto nos permite conocer el estado y la capacidad de almacenamiento en tiempo real de una manera más comprensible.

<p align="center">
  <img src="/imagenes/df -h.png" alt="Descripción de la imagen" width="400"/>
</p>

- **df -l**

Se utiliza para mostrar solo los sistemas de archivos locales. Nos proporcionará información detallada sobre la cantidad de espacio total, usado y disponible en cada sistema de archivos local, así como el porcentaje de uso. Esto nos permite conocer el estado y la capacidad de almacenamiento de los sistemas de archivos locales en tiempo real.

<p align="center">
  <img src="/imagenes/df -l.png" alt="Descripción de la imagen" width="500"/>
</p>

- **df -T**

Se utiliza para mostrar solo los sistemas de archivos de un tipo específico. Proporciona información detallada sobre la cantidad de espacio total, usado y disponible en cada sistema de archivos del tipo especificado, así como el porcentaje de uso. Esto permite a los administradores de sistemas conocer el estado y la capacidad de almacenamiento de los sistemas de archivos de un tipo específico en tiempo real.

<p align="center">
  <img src="/imagenes/df -T.png" alt="Descripción de la imagen" width="500"/>
</p>

- **df -x**

La opción -x se utiliza para excluir sistemas de archivos de un tipo específico. Proporciona información detallada sobre la cantidad de espacio total, usado y disponible en cada sistema de archivos, excluyendo aquellos del tipo especificado, así como el porcentaje de uso. Esto permite a los administradores de sistemas conocer el estado y la capacidad de almacenamiento de los sistemas de archivos, excluyendo los tipos especificados, en tiempo real. Requiere que especifiquemos el tipo de sistema de archivos que deseas excluir

<p align="center">
  <img src="/imagenes/df -x listen.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando DU**

*Se utiliza para estimar y mostrar el uso del espacio en disco de archivos y directorios. Proporcionará información detallada sobre la cantidad de espacio en disco utilizado por cada archivo y directorio especificado, permite conocer el estado y la capacidad de almacenamiento en tiempo real.*

---
### **Opciones**

---
- **du**

Ejecutanado el comando du sin opciones, nos mostrará el uso del espacio en disco de todos los archivos y directorios en el directorio actual y sus subdirectorios. Nos proporciona información detallada sobre la cantidad de espacio en disco utilizado por cada archivo y directorio especificado, permitiendo a los administradores de sistemas conocer el estado y la capacidad de almacenamiento en tiempo real.

<p align="center">
  <img src="/imagenes/du.png" alt="Descripción de la imagen" width="200"/>
</p>

- **du --help**

Nos muestra una lista de todas las opciones disponibles para el comando du, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando y cómo se pueden utilizar las diferentes opciones para obtener información específica sobre el estado y la capacidad de almacenamiento en el sistema.

<p align="center">
  <img src="/imagenes/du help.png" alt="Descripción de la imagen" width="200"/>
</p>

- **du -h**

Se utiliza para mostrar el uso del espacio en disco en un formato legible para humanos. Proporcionará información detallada sobre la cantidad de espacio en disco utilizado por cada archivo y directorio especificado, utilizando unidades como KB, MB o GB. Esto nos permite conocer el estado y la capacidad de almacenamiento de una manera más comprensible.

<p align="center">
  <img src="/imagenes/du -h.png" alt="Descripción de la imagen" width="200"/>
</p>

- **du -s**

Se utiliza para mostrar el uso del espacio en disco de un directorio especificado y sus subdirectorios, proporcionando un resumen total. Esto nos permite conocer el estado y la capacidad de almacenamiento de un directorio específico en tiempo real.

<p align="center">
  <img src="/imagenes/du -s.png" alt="Descripción de la imagen" width="300"/>
</p>

- **du -c**

Se utiliza para mostrar un total general al final de la salida. Esto significa que, además de mostrar el uso del espacio en disco para cada archivo y directorio especificado, también proporcionará un resumen total del uso del espacio en disco al final de la lista. Esto es útil para obtener una visión general del uso total del espacio en disco en un directorio y sus subdirectorios.

<p align="center">
  <img src="/imagenes/du-c.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando FREE**

*Se utiliza para mostrar la cantidad de memoria libre y usada en el sistema, incluyendo la memoria física (RAM) y el espacio de intercambio (swap). Proporcionará un resumen del uso de la memoria en tiempo real, permitiendo a los administradores de sistemas conocer el estado y el rendimiento de la memoria.*

---
### **Opciones**

---
- **free**

Nos mostrará un resumen del uso de la memoria en el sistema. Proporcionará información detallada sobre la cantidad de memoria total, usada, libre, compartida, en búferes y en caché, tanto para la memoria física (RAM) como para el espacio de intercambio (swap). Esto permitirá conocer el estado y el rendimiento de la memoria en tiempo real.

<p align="center">
  <img src="/imagenes/free.png" alt="Descripción de la imagen" width="500"/>
</p>

- **free --help**

Nos muestra una lista de todas las opciones disponibles para el comando free, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando y cómo se pueden utilizar las diferentes opciones para obtener información específica sobre el uso de la memoria en el sistema.
 
<p align="center">
  <img src="/imagenes/free2.png" alt="Descripción de la imagen" width="300"/>
</p>

- **free -v**

Esta opción muestra una vista extendida de la información sobre la memoria. En lugar de mostrar únicamente los valores básicos (como memoria total, usada, libre, etc.), incluye detalles adicionales dependiendo del sistema operativo o distribución. Por ejemplo, en algunas versiones de Debian, puede incluir información sobre Huge Pages (páginas de memoria grandes usadas en sistemas avanzados para optimizar el rendimiento).


<p align="center">
  <img src="/imagenes/free-v.png" alt="Descripción de la imagen" width="500"/>
</p>

- **free -l**

Se utiliza para mostrar información adicional sobre la memoria baja y la memoria alta del sistema. Nos muestra una salida similar a la del comando free normal, pero incluye columnas adicionales para estas dos categorías de memoria

<p align="center">
  <img src="/imagenes/free-l.png" alt="Descripción de la imagen" width="500"/>
</p>

- **free -t**

Se utiliza para mostrar un resumen del uso de la memoria, incluyendo la memoria física (RAM) y el espacio de intercambio (swap), con un total general al final de la salida. Esto nos permite obtener una visión general del uso total de la memoria en el sistema.
 
<p align="center">
  <img src="/imagenes/free-t.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando IOSTAT**

*Se utiliza para monitorear el rendimiento del sistema, específicamente el uso de la CPU y las estadísticas de entrada/salida de los dispositivos de almacenamiento. Proporcionará información detallada sobre la carga de trabajo del sistema y el rendimiento de los dispositivos de almacenamiento, permitiendo a los administradores de sistemas identificar posibles cuellos de botella y optimizar el rendimiento.*

---
### **Opciones**

---
- **iostat**

Nos mostrará un resumen del uso de la CPU y las estadísticas de entrada/salida de los dispositivos de almacenamiento. Proporciona información detallada sobre la carga de trabajo del sistema y el rendimiento de los dispositivos de almacenamiento, permitiendo identificar posibles cuellos de botella y optimizar el rendimiento.

<p align="center">
  <img src="/imagenes/iiostat.png" alt="Descripción de la imagen" width="500"/>
</p>

- **iostat --help**

Nos muestra una lista de todas las opciones disponibles para el comando iostat, junto con una breve descripción de cada una. Esto es útil para obtener una visión general de las capacidades del comando y cómo se pueden utilizar las diferentes opciones para obtener información específica sobre el rendimiento del sistema y los dispositivos de almacenamiento.

<p align="center">
  <img src="/imagenes/iostat2.png" alt="Descripción de la imagen" width="500"/>
</p>

- **iostat -x**

Se utiliza para mostrar estadísticas detalladas de entrada/salida por dispositivo. Proporciona información más granular sobre el rendimiento de cada dispositivo de almacenamiento, incluyendo métricas como el tiempo de espera promedio, el tiempo de servicio promedio, el porcentaje de tiempo de utilización del dispositivo, entre otros. Esto nos permite identificar posibles cuellos de botella y optimizar el rendimiento de los dispositivos de almacenamiento de manera más efectiva.

<p align="center">
  <img src="/imagenes/iostat -x.png" alt="Descripción de la imagen" width="500"/>
</p>

- **iostat -p**

Se utiliza para mostrar estadísticas de entrada/salida por partición. Proporciona información detallada sobre el rendimiento de cada partición de los dispositivos de almacenamiento, incluyendo métricas como el tiempo de espera promedio, el tiempo de servicio promedio, el porcentaje de tiempo de utilización de la partición, entre otros. Esto permitirá identificar posibles cuellos de botella y optimizar el rendimiento de las particiones de almacenamiento de manera más efectiva.

<p align="center">
  <img src="/imagenes/ios -p.png" alt="Descripción de la imagen" width="500"/>
</p>

- **iostat -d**

Se utiliza para mostrar estadísticas de entrada/salida por dispositivo. Proporciona información detallada sobre el rendimiento de cada dispositivo de almacenamiento, incluyendo métricas como el tiempo de espera promedio, el tiempo de servicio promedio, el porcentaje de tiempo de utilización del dispositivo, entre otros. Nos permite identificar posibles cuellos de botella y optimizar el rendimiento de los dispositivos de almacenamiento de manera más efectiva.

<p align="center">
  <img src="/imagenes/ios-d.png" alt="Descripción de la imagen" width="500"/>
</p>

- **iostat -N**

Sirve para mostrar el nombre completo de los dispositivos gestionados por el sistema, incluyendo la información de los volúmenes lógicos si estos están configurados en el sistema (por ejemplo, con LVM).

Cuando no se usa -N, es posible que el comando solo muestre nombres de dispositivos más cortos o abreviados, como /dev/sda, en lugar de los nombres completos o los asociados a LVM, como /dev/mapper/volumen-logico. Es útil en escenarios donde estás trabajando con sistemas que usan LVM (Logical Volume Manager) o si necesitas identificar dispositivos en volúmenes complejos o RAID.

<p align="center">
  <img src="/imagenes/IOS -n.png" alt="Descripción de la imagen" width="500"/>
</p>

- **iostat -c**

Se utiliza para mostrar estadísticas de la CPU. Proporcionará información detallada sobre el uso de la CPU, incluyendo métricas como el porcentaje de tiempo que la CPU está inactiva, el porcentaje de tiempo que la CPU está ocupada en modo de usuario, el porcentaje de tiempo que la CPU está ocupada en modo de sistema, entre otros. Esto nos permite identificar posibles cuellos de botella y optimizar el rendimiento de la CPU de manera más efectiva.

<p align="center">
  <img src="/imagenes/ios-c.png" alt="Descripción de la imagen" width="500"/>
</p>

---
