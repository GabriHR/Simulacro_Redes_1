Link con acceso al respositorio --> https://github.com/GabriHR/Simulacro_Redes_1.git

---

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

### Explica el papel de la capa de transporte en ambos modelos (OSI y TCP/IP). En tu respuesta, menciona cómo se garantiza la entrega de datos y da ejemplos de protocolos asociados a esta capa.

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
