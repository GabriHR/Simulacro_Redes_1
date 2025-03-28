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
