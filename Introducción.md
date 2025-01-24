# **Introducción**
<p align="center">
  <img src="/imagenes/monitorización-de-sistemas-informaticos.jpg" alt="Descripción de la imagen" width="500"/>
</p>
La Monitorización de Sistemas es una práctica esencial para garantizar el correcto funcionamiento de los sistemas informáticos y prevenir problemas antes de que afecten a los usuarios finales, que básicamente consiste en la instalación de una serie de sensores en los diferentes elementos hardware y software de forma que, 24h al día y 7 días a la semana, estos sensores registran la situación en que están cada uno de los aspectos que controlamos.
En un mundo cada vez más digitalizado, donde las organizaciones dependen de sus sistemas para garantizar la continuidad de sus operaciones, es crucial contar con herramientas y técnicas que permitan supervisar de manera continua el estado de los componentes que integran estas infraestructuras. Desde servidores y bases de datos hasta redes y aplicaciones, la monitorización proporciona información en tiempo real sobre el rendimiento, la disponibilidad y posibles incidencias que puedan comprometer el funcionamiento del entorno.
La monitorización de sistemas se ha convertido en una tarea fundamental en la gestión de infraestructuras tecnológicas, permitiendo supervisar el estado de los recursos y garantizar un rendimiento óptimo.

## Beneficios de la Monitorización de Sistemas
- **Optimización del rendimiento**: Al monitorizar los sistemas de manera constante, podemos identificar cuellos de botella y cuellos de rendimiento. Esto permite optimizar la configuración de los servidores y aplicaciones para obtener un rendimiento máximo.
- **Mejora de la disponibilidad**: La monitorización de sistemas nos ayuda a detectar problemas de disponibilidad, como caídas de servidores o redes. Al recibir alertas inmediatas, podemos tomar medidas para restablecer el servicio rápidamente y minimizar el impacto en los usuarios finales.
- **Prevención de problemas**: La monitorización de sistemas nos permite anticiparnos a los problemas y tomar medidas correctivas antes de que afecten a los usuarios. Al detectar patrones de comportamiento anormales o tendencias negativas, podremos abordarlos antes de que se conviertan en un problema mayor.
- **Reducción del tiempo de inactividad**: Gracias a la monitorización de sistemas, podremos identificar y resolver problemas de manera proactiva, lo que reduce significativamente el tiempo de inactividad de los sistemas. Esto se traduce en una mayor productividad y satisfacción de los usuarios finales.
- **Tranquilidad**: La monitorización de sistemas es una práctica esencial para garantizar el correcto funcionamiento de una infraestructura IT. Al pasar de un enfoque reactivo a uno proactivo, podremos anticiparnos a los problemas, optimizar el rendimiento, mejorar la disponibilidad y reducir el tiempo de inactividad.
- **Prevención de situaciones graves**: Cuando los problemas no se abordan de manera proactiva, pueden convertirse en situaciones graves que afectan la eficiencia operativa y la satisfacción del cliente.

## Situaciones de Gravedad
- **Tiempo de inactividad no planificada**: Cuando los sistemas informáticos, las aplicaciones y las redes no se monitorizan de manera proactiva, es más probable que se den tiempos de inactividad no planificados. Este tiempo de inactividad puede resultar en una pérdida de productividad, ingresos y clientes.
- **Lentitud del sistema**: Las infraestructuras que no se monitorizan de manera proactiva pueden experimentar problemas de rendimiento que afectan la velocidad y la eficiencia del sistema. La lentitud del sistema puede provocar una disminución en la productividad y generar insatisfacción entre los clientes.
- **Problemas de seguridad**: Las infraestructuras que no se monitorizan de manera proactiva corren el riesgo de enfrentar problemas de seguridad, como virus, malware y ataques cibernéticos. La gestión reactiva de las infraestructuras dificulta la detección y solución de problemas de seguridad antes de que afecten a los sistemas informáticos y las redes.

## Objetivos de la Monitorización de Sistemas
- Aprovechar al máximo los recursos HW de una empresa.
- Prevención de incidencias y detección de problemas.
- Notificación de posibles problemas.
- Ahorro de costes.
- Ahorro de tiempo.
- Mejorar la satisfacción en atención al cliente.

Para conseguir estos objetivos lo primero es contar con un sistema de monitorización, lo siguiente sería establecer un protocolo de resolución de incidencias, esto va a marcar la diferencia a la hora de resolver problemas.

## Razones para Monitorizar Sistemas
- Acceso al estado de los sistemas informáticos en tiempo real.
- Detección del origen de los incidentes.
- Acceso a información ejecutiva del estado de las instalaciones y chequear cómo están los activos informáticos más críticos.
- Mejorar la eficacia y la eficiencia de las labores de mantenimiento del sistema.
- Configuración de eventos y alarmas. Por ejemplo, alarmas cuando un disco duro esté lleno, la memoria esté ocupada por encima del 80%, en caso de que haya demasiados accesos a disco en modo escritura, demasiados hilos abiertos corriendo en el mismo sistema, etc.
- Inventariar sistemas (mapas, listados).
- Planificar el crecimiento en base al uso real de los sistemas. Mediante informes de uso, se pueden detectar tendencias y saber cuándo hace falta más disco, poner otro servidor o aumentar la memoria.
- Reducir costes.

## Herramientas de Monitorización
A través de diversas herramientas, es posible analizar los procesos, el almacenamiento y las redes en tiempo real, o a través de análisis históricos, adaptándose a diferentes necesidades y entornos. Podemos diferenciar entre dos tipos:

### Herramientas de Línea de Comandos
- Una interfaz de línea de comandos (**CLI**) es un mecanismo de software que se utiliza para interactuar con el sistema operativo mediante el teclado.
- La línea de comandos permite automatizar fácilmente tareas como crear, copiar y convertir archivos, configurar el entorno de programación, ejecutar lo que programamos, acceder a los programas y utilidades que no tienen equivalentes gráficos, o controlar otras computadoras de forma remota.
- Entre las herramientas más destacadas en entornos de línea de comandos, se encuentran:
  - **htop**: Ideal para la monitorización de procesos en tiempo real, con una interfaz interactiva y amigable. Aunque es muy útil para obtener información rápida sobre el uso de CPU y memoria, no permite un análisis histórico detallado.
  - **df y du**: Herramientas básicas para la monitorización del almacenamiento. Mientras df proporciona datos globales del uso del disco, du detalla el consumo de espacio por directorios. Son ligeras y simples, pero carecen de capacidades avanzadas.
 capacidades avanzadas.
  - **tcpdump e iptraf**: En el ámbito de la red, estas herramientas permiten monitorear el tráfico en tiempo real. `tcpdump` captura y analiza paquetes de red, mientras que `iptraf` ofrece estadísticas detalladas del tráfico de red. Sin embargo, no son adecuadas para análisis complejos o históricos.

### Herramientas de Interfaz Gráfica
- Otro mecanismo disponible es la interfaz de usuario gráfica (**GUI**), la cual se utiliza en la actualidad en casi todas las aplicaciones y sistemas de software.
- Entre las herramientas más avanzadas para entornos gráficos y de análisis en profundidad, destacan:

  - **Grafana**: Una plataforma de visualización potente que se integra con numerosas fuentes de datos como Prometheus. Su capacidad para crear paneles personalizados lo hace ideal para análisis históricos y tendencias, aunque requiere cierta curva de aprendizaje.
    <p align="center">
      <img src="/imagenes/grafana-2.jpg" alt="Descripción de la imagen" width="200"/>
    </p>

  - **Prometheus**: Especializada en la monitorización de métricas, es perfecta para la recopilación y análisis de datos en tiempo real. Su principal ventaja es su integración nativa con Grafana, pero puede ser más compleja de configurar en comparación con herramientas más sencillas.
    <p align="center">
      <img src="/imagenes/prometheus.png" alt="Descripción de la imagen" width="300"/>
    </p>   

  - **Zabbix**: Una solución integral para monitorización en tiempo real y alertas. Es adecuada para grandes infraestructuras, pero puede ser excesiva para entornos pequeños debido a su nivel de configuración.
    <p align="center">
      <img src="/imagenes/zabbix-logo.png" alt="Descripción de la imagen" width="200"/>
    </p>

  - **Nagios**: Una herramienta sólida para la monitorización de redes, sistemas y aplicaciones. Ofrece flexibilidad mediante plugins, aunque su interfaz puede resultar menos intuitiva comparada con Grafana o Zabbix.
    <p align="center">
      <img src="/imagenes/nagios.jpg" alt="Descripción de la imagen" width="300"/>
    </p>

Este trabajo se organiza en tres apartados: la monitorización de procesos, de almacenamiento y de red. Cada sección detallará los comandos esenciales y sus opciones clave, así como ejemplos gráficos (Capturas de Pantalla) de las respuestas de estos al ser ejecutados.

