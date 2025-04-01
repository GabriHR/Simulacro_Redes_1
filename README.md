## Pregunta 1: Modelos OSI y TCP/IP

### a) Describe las principales diferencias entre el modelo OSI y el modelo TCP/IP, considerando aspectos como el número de capas, la orientación (teórica vs. práctica) y el manejo de la capa de aplicación.

**Diferencias principales entre el modelo OSI y el modelo TCP/IP:**

- **Número de capas:**
    - **Modelo OSI:** Tiene 7 capas (Física, Enlace de Datos, Red, Transporte, Sesión, Presentación y Aplicación).
    - **Modelo TCP/IP:** Tiene 4 capas (Acceso a la Red, Internet, Transporte y Aplicación).

- **Orientación:**
    - **Modelo OSI:** Es un modelo teórico y conceptual que no está directamente vinculado a un protocolo específico. Se utiliza principalmente como una guía para entender y diseñar redes.
    - **Modelo TCP/IP:** Es un modelo práctico y basado en protocolos reales utilizados en Internet. Está diseñado para ser implementado y utilizado en redes reales.

- **Manejo de la capa de aplicación:**
    - **Modelo OSI:** La capa de Aplicación está separada en tres capas distintas: Aplicación, Presentación y Sesión.
    - **Modelo TCP/IP:** La capa de Aplicación combina las funciones de las capas de Aplicación, Presentación y Sesión del modelo OSI.

### b) Explica brevemente las ventajas y limitaciones de cada uno de estos modelos.

**Ventajas y limitaciones de cada modelo:**

- **Modelo OSI:**
    - **Ventajas:**
        - Proporciona una guía clara y detallada para la implementación de redes.
        - Facilita la interoperabilidad y la estandarización de los protocolos de red.
        - Ayuda a los desarrolladores y administradores de red a entender y solucionar problemas de red.
    - **Limitaciones:**
        - Es un modelo teórico y no está directamente vinculado a protocolos específicos.
        - Puede ser más complejo y menos intuitivo para la implementación práctica.

- **Modelo TCP/IP:**
    - **Ventajas:**
        - Es un modelo práctico y ampliamente utilizado en redes reales, especialmente en Internet.
        - Está basado en protocolos específicos y probados, lo que facilita su implementación.
        - Es más simple y directo en comparación con el modelo OSI.
    - **Limitaciones:**
        - No proporciona una guía tan detallada y estructurada como el modelo OSI.
        - Puede ser menos flexible en términos de estandarización y desarrollo de nuevos protocolos.
---

## Pregunta 2: Función de la Capa de Transporte

Explica el papel de la capa de transporte en ambos modelos (OSI y TCP/IP). En tu respuesta, menciona cómo se garantiza la entrega de datos y da ejemplos de protocolos asociados a esta capa.

## Solución:
**Función de la Capa de Transporte**

La capa de transporte es crucial tanto en el modelo OSI como en el modelo TCP/IP, ya que se encarga de proporcionar una transferencia de datos confiable y eficiente entre sistemas finales.

**Modelo OSI**

En el modelo OSI, la capa de transporte es la cuarta capa. Su función principal es garantizar que los datos se transfieran de manera confiable y sin errores entre los nodos de la red. Esto se logra mediante:

- **Control de flujo:** Regula la cantidad de datos que se envían para evitar la congestión de la red.
- **Control de errores:** Detecta y corrige errores que puedan ocurrir durante la transmisión de datos.
- **Segmentación y reensamblaje:** Divide los datos en segmentos más pequeños para su transmisión y los reensambla en el destino.
- **Establecimiento de conexión:** Establece, mantiene y termina conexiones lógicas entre los nodos.

Ejemplos de protocolos en la capa de transporte del modelo OSI incluyen:

- **TCP (Transmission Control Protocol):** Protocolo orientado a la conexión que garantiza la entrega confiable de datos.
- **UDP (User Datagram Protocol):** Protocolo no orientado a la conexión que permite la transmisión rápida de datos sin garantía de entrega.

**Modelo TCP/IP**

En el modelo TCP/IP, la capa de transporte es la tercera capa. Sus funciones son similares a las del modelo OSI, enfocándose en la entrega confiable de datos entre aplicaciones. Las principales responsabilidades incluyen:

- **Multiplexación:** Permite que múltiples aplicaciones utilicen la red simultáneamente.
- **Control de flujo y errores:** Similar al modelo OSI, regula la transmisión de datos y corrige errores.
- **Establecimiento de conexión:** Gestiona la creación y terminación de conexiones entre aplicaciones.

Ejemplos de protocolos en la capa de transporte del modelo TCP/IP incluyen:

- **TCP (Transmission Control Protocol):** Protocolo orientado a la conexión que asegura la entrega ordenada y confiable de datos.
- **UDP (User Datagram Protocol):** Protocolo no orientado a la conexión que permite la transmisión rápida y sin garantía de entrega.

En resumen, la capa de transporte en ambos modelos es esencial para garantizar la entrega confiable y eficiente de datos entre sistemas finales, utilizando protocolos como TCP y UDP para cumplir con sus funciones.

---

## Pregunta 3: TCP vs. UDP

### Compara y contrasta TCP y UDP en términos de:

#### Orientación a conexión

- **TCP (Transmission Control Protocol):** Es un protocolo orientado a la conexión. Esto significa que antes de que los datos puedan ser transferidos, se debe establecer una conexión entre el emisor y el receptor mediante un proceso de "handshake" de tres vías.
- **UDP (User Datagram Protocol):** Es un protocolo no orientado a la conexión. No requiere establecer una conexión antes de enviar datos, lo que permite una comunicación más rápida pero menos confiable.

#### Fiabilidad y control de errores

- **TCP:** Proporciona fiabilidad y control de errores. Utiliza técnicas como la retransmisión de paquetes perdidos, el control de flujo y el control de congestión para asegurar que los datos lleguen correctamente y en orden.
- **UDP:** No proporciona fiabilidad ni control de errores. Los paquetes pueden perderse, duplicarse o llegar fuera de orden sin que el protocolo intente corregir estos problemas. Es responsabilidad de la aplicación manejar estos aspectos si es necesario.

#### Velocidad y orden de entrega

- **TCP:** Debido a su naturaleza orientada a la conexión y sus mecanismos de control de errores, TCP tiende a ser más lento que UDP. Sin embargo, garantiza que los datos lleguen en el orden correcto.
- **UDP:** Es más rápido que TCP porque no tiene el overhead de establecer una conexión y no realiza control de errores. Sin embargo, no garantiza el orden de entrega de los datos.

#### Ejemplos de aplicaciones en las que se emplea cada uno

- **TCP:**
    - **HTTP/HTTPS:** Utilizado para la navegación web.
    - **FTP:** Protocolo de transferencia de archivos.
    - **SMTP:** Protocolo para el envío de correos electrónicos.
    - **SSH:** Protocolo para acceso remoto seguro.

- **UDP:**
    - **DNS:** Sistema de nombres de dominio.
    - **VoIP:** Protocolo de voz sobre IP.
    - **Streaming de video y audio:** Aplicaciones que requieren transmisión continua de datos.
    - **TFTP:** Protocolo de transferencia de archivos trivial.

En resumen, TCP y UDP son protocolos de transporte con diferentes características y usos. TCP es adecuado para aplicaciones que requieren fiabilidad y orden, mientras que UDP es ideal para aplicaciones que priorizan la velocidad y pueden tolerar la pérdida de datos.

---

## Pregunta 4: Protocolo para Transferencia de Archivos
### a) ¿Qué protocolo de la capa de aplicación se utiliza tradicionalmente para la transferencia de archivos en redes TCP/IP?

### Solución:
El protocolo tradicionalmente utilizado para la transferencia de archivos en redes TCP/IP es el FTP (File Transfer Protocol).

### b) Menciona al menos dos alternativas a este protocolo, resaltando sus diferencias principales en cuanto a seguridad o funcionalidad.

### Solución:
SFTP (SSH File Transfer Protocol):

Seguridad: SFTP proporciona una transferencia de archivos segura utilizando el protocolo SSH (Secure Shell) para cifrar tanto los datos como las credenciales de usuario.
Funcionalidad: Además de la transferencia de archivos, SFTP permite operaciones de gestión de archivos como la creación, eliminación y modificación de archivos y directorios en el servidor remoto.
FTPS (FTP Secure):

Seguridad: FTPS añade soporte para SSL/TLS (Secure Sockets Layer/Transport Layer Security) a FTP, proporcionando cifrado para la transferencia de datos y las credenciales de usuario.
Funcionalidad: FTPS mantiene la misma funcionalidad que FTP, pero con la adición de seguridad mediante cifrado. Puede operar en modo explícito (requiere una conexión segura) o implícito (usa un puerto seguro predeterminado).
En resumen, mientras que FTP es el protocolo tradicional para la transferencia de archivos, SFTP y FTPS ofrecen mejoras significativas en términos de seguridad mediante el uso de cifrado.

---

## Pregunta 5: Resolución de Nombres en DNS
Describe detalladamente el proceso de resolución de nombres en DNS, desde que un usuario ingresa una URL en el navegador 
hasta que se establece la conexión con el servidor web. Incluye en tu respuesta el rol de la caché y de los servidores raíz.

## Solución:

El proceso de resolución de nombres en DNS (Domain Name System) es el mecanismo mediante el cual se traduce un nombre de dominio legible por humanos (como `www.ejemplo.com`) en una dirección IP (como `192.0.2.1`) que las computadoras utilizan para identificar y comunicarse con los servidores en la red. A continuación se describe detalladamente este proceso:

1. **Ingreso de la URL:**
    - El usuario ingresa una URL en el navegador web.

2. **Consulta a la Caché del Navegador:**
    - El navegador primero verifica si la dirección IP correspondiente al nombre de dominio ya está almacenada en su caché local. Si la encuentra, utiliza esa dirección IP para establecer la conexión.

3. **Consulta a la Caché del Sistema Operativo:**
    - Si la dirección IP no está en la caché del navegador, el sistema operativo verifica su propia caché DNS para ver si tiene la dirección IP correspondiente.

4. **Consulta al Servidor DNS Recursivo:**
    - Si la dirección IP no se encuentra en la caché del sistema operativo, se envía una consulta a un servidor DNS recursivo (generalmente proporcionado por el ISP o configurado manualmente).

5. **Consulta a la Caché del Servidor DNS Recursivo:**
    - El servidor DNS recursivo verifica su propia caché para ver si tiene la dirección IP correspondiente al nombre de dominio.

6. **Consulta a los Servidores Raíz:**
    - Si la dirección IP no está en la caché del servidor DNS recursivo, este envía una consulta a uno de los servidores raíz del DNS. Los servidores raíz no contienen la dirección IP del dominio, pero pueden dirigir la consulta a los servidores de dominio de nivel superior (TLD).

7. **Consulta a los Servidores TLD:**
    - Los servidores raíz responden con la dirección de los servidores TLD (por ejemplo, los servidores responsables de `.com`, `.org`, etc.). El servidor DNS recursivo entonces consulta a los servidores TLD correspondientes.

8. **Consulta a los Servidores Autoritativos:**
    - Los servidores TLD responden con la dirección de los servidores DNS autoritativos para el dominio específico (por ejemplo, `ejemplo.com`). El servidor DNS recursivo consulta a estos servidores autoritativos.

9. **Respuesta del Servidor Autoritativo:**
    - Los servidores autoritativos responden con la dirección IP correspondiente al nombre de dominio solicitado.

10. **Almacenamiento en Caché:**
    - El servidor DNS recursivo almacena la dirección IP en su caché para futuras consultas y la envía de vuelta al sistema operativo del usuario.

11. **Establecimiento de la Conexión:**
    - El sistema operativo pasa la dirección IP al navegador, que luego establece una conexión con el servidor web utilizando la dirección IP obtenida.

12. **Carga del Sitio Web:**
    - El navegador envía una solicitud HTTP al servidor web y comienza a cargar el sitio web solicitado.

---

## Pregunta 6: Comunicación en el Modelo TCP/IP
Explica el proceso de comunicación entre dos dispositivos en una red utilizando el modelo TCP/IP. Describe el rol y la función de cada capa (Aplicación, Transporte, Internet y Acceso a Red) durante el envío y recepción de datos.

## Solución:
El proceso de comunicación entre dos dispositivos en una red utilizando el modelo TCP/IP implica varias capas, cada una con roles y funciones específicas. A continuación se describe el proceso de envío y recepción de datos a través de las capas del modelo TCP/IP:


- Capa de Aplicación:


    - Rol: Proporciona servicios de red a las aplicaciones del usuario.
    - Función: Las aplicaciones generan datos que necesitan ser enviados a través de la red. Ejemplos de protocolos en esta capa incluyen HTTP, FTP, SMTP y DNS.
    - Proceso: La aplicación (por ejemplo, un navegador web) crea un mensaje (por ejemplo, una solicitud HTTP) y lo pasa a la capa de transporte.
- Capa de Transporte:


    - Rol: Proporciona comunicación de extremo a extremo y control de flujo de datos.
    - Función: Divide los datos en segmentos, asegura la entrega confiable (en el caso de TCP) y gestiona el control de errores y el reensamblaje de datos.
    - Proceso: La capa de transporte (por ejemplo, utilizando TCP) encapsula el mensaje de la capa de aplicación en segmentos, añade encabezados con información de control (como números de puerto y secuencia) y lo pasa a la capa de Internet.
- Capa de Internet:


    - Rol: Encargada de la dirección y el encaminamiento de los paquetes a través de la red.
    - Función: Encapsula los segmentos en paquetes, añade encabezados con direcciones IP de origen y destino, y determina la ruta que los paquetes deben seguir para llegar al destino.
    - Proceso: La capa de Internet (utilizando el protocolo IP) encapsula los segmentos en paquetes IP, añade las direcciones IP y pasa los paquetes a la capa de acceso a red.
- Capa de Acceso a Red:


    - Rol: Maneja la transmisión física de los datos a través de la red.
    - Función: Encapsula los paquetes IP en tramas, añade encabezados y trailers con direcciones MAC y otra información de control, y transmite las tramas a través del medio físico (cableado, inalámbrico, etc.).
    - Proceso: La capa de acceso a red (utilizando protocolos como Ethernet o Wi-Fi) encapsula los paquetes en tramas, añade las direcciones MAC y transmite las tramas a través del medio físico hacia el dispositivo de destino.

### Recepción de Datos

El proceso de recepción de datos es el inverso del proceso de envío:


- Capa de Acceso a Red:


    - Proceso: El dispositivo receptor recibe las tramas a través del medio físico, verifica las direcciones MAC y pasa las tramas a la capa de Internet.
- Capa de Internet:


    - Proceso: La capa de Internet verifica las direcciones IP, desencapsula los paquetes IP y pasa los segmentos a la capa de transporte.
- Capa de Transporte:


    -Proceso: La capa de transporte verifica los números de puerto, reensambla los segmentos en el mensaje original, maneja el control de errores y pasa el mensaje a la capa de aplicación.
- Capa de Aplicación:


    - Proceso: La capa de aplicación recibe el mensaje y lo entrega a la aplicación correspondiente (por ejemplo, el navegador web muestra la página web solicitada).
En resumen, cada capa del modelo TCP/IP tiene un rol específico en el proceso de comunicación, desde la generación de datos por la aplicación hasta la transmisión física y la recepción de los datos en el dispositivo de destino.