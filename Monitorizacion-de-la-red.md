
---
# **Monitorizacion de la Red**

***La monitorización de la red es vital para asegurar una comunicación eficiente y detectar posibles problemas de conectividad o de rendimiento en el sistema. Al controlar el tráfico de red, podemos identificar cuellos de botella, conexiones no deseadas o problemas de latencia. En sistemas Linux, existen diversos comandos que permiten observar el estado de la red, el uso del ancho de banda y la actividad de las interfaces de red. En esta presentación, exploraremos algunos de los comandos más utilizados para monitorizar el tráfico de red y mantener una red saludable y eficiente.***

<p align="center">
  <img src="/imagenes/red.jpg" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando NETSTAT**

---
### **Opciones**

---
- **netstat**

<p align="center">
  <img src="/imagenes/netstat.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat --help**

<p align="center">
  <img src="/imagenes/nestat help.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat -a**

<p align="center">
  <img src="/imagenes/nestat -a.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat -p**

<p align="center">
  <img src="/imagenes/nestat -p.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat -tp**

<p align="center">
  <img src="/imagenes/nestat -tp.png" alt="Descripción de la imagen" width="500"/>
</p>

- **netstat -r**

<p align="center">
  <img src="/imagenes/netsatat2.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando TCPDUMP**


---
### **Opciones**

---
- **tcpdump**

 <p align="center">
  <img src="/imagenes/tcpdump.png" alt="Descripción de la imagen" width="500"/>
</p>

- **tcpdump --help**

<p align="center">
  <img src="/imagenes/tcpdump help.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **tcpdump -i**

<p align="center">
  <img src="/imagenes/tcpdump -i.png" alt="Descripción de la imagen" width="500"/>
</p>

- **tcpdump -Z**

<p align="center">
  <img src="/imagenes/tcpdump -Z.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando TCPTRACK**


---
### **Opciones**

---
- **tcptrack**

 <p align="center">
  <img src="/imagenes/tcptrack.png" alt="Descripción de la imagen" width="500"/>
</p>

- **tcptrack -i**
  
 <p align="center">
  <img src="/imagenes/tcptrack -i enp0s3.png" alt="Descripción de la imagen" width="500"/>
</p>

 <p align="center">
  <img src="/imagenes/tcptrack.png" alt="Descripción de la imagen" width="500"/>
</p>

---
## **Comando IPTRAF**

---
### **Opciones**

---
- **iptraf --help**

<p align="center">
  <img src="/imagenes/iptraf 2.png" alt="Descripción de la imagen" width="500"/>
</p> 

- **iptraf -ng**

<p align="center">
  <img src="/imagenes/iptraf-ng.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando Bandwithd**

---
### **Opciones**

---
- **bandwithd**

<p align="center">
  <img src="/imagenes/bandwithd.png" alt="Descripción de la imagen" width="500"/>
</p> 

<p align="center">
  <img src="/imagenes/band2.png" alt="Descripción de la imagen" width="500"/>
</p> 

---
## **Comando NLOAD**

Es una herramienta que se utiliza para monitorear el tráfico de red y el uso del ancho de banda en tiempo real. Visualiza el tráfico entrante y saliente utilizando gráficos y proporciona información adicional como la cantidad total de datos transferidos y el uso mínimo/máximo de la red

---
- **nload**

Obtendremos una visualización en tiempo real del tráfico de red y el uso del ancho de banda.Nos muestra gráficos del tráfico entrante y saliente, así como información adicional como la cantidad total de datos transferidos y el uso mínimo/máximo de la red. Es una herramienta muy útil para quienes necesitan monitorear el rendimiento de la red de manera eficiente.

- **nload --help**

Nos muestra una lista de todas las opciones disponibles, junto con una breve descripción de cada una. Se utiliza para monitorizar en tiempo real el tráfico de red, mostrando gráficos interactivos del ancho de banda utilizado para descarga (inbound) y subida (outbound). Las opciones permiten configurar aspectos como la interfaz de red que se desea monitorizar, el intervalo de actualización, las unidades de medida (bits o bytes), y ajustes visuales como los colores o el escalado automático. Esta ayuda facilita personalizar nload para realizar un seguimiento eficiente del tráfico de red según las necesidades del usuario.

<p align="center">
  <img src="/imagenes/nload-help.jpg" alt="Descripción de la imagen" width="500"/>
</p> 

---
<p align="center">
  <img src="/imagenes/redes2.jpg" alt="Descripción de la imagen" width="500"/>
</p> 

---
