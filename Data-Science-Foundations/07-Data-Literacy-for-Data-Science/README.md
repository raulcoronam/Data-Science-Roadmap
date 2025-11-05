# Módulo 7: Data Literacy for Data Science (Understanding Data)

Este módulo es la base de todo: la alfabetización de datos. Antes de poder analizar o modelar, debo entender qué es el dato en su forma más pura: sus tipos, sus fuentes y, lo más importante, sus "datos sobre los datos" (metadata).

## 🎯 Mi Objetivo con este Módulo

* **¿Qué sé ya sobre esto?** (Ej: "Sé que hay 'datos' en todas partes. Entiendo la diferencia básica entre un archivo de texto y una tabla de Excel. Pero no tengo claro por qué un mismo dato puede venir de tantas fuentes diferentes.")
* **¿Cuál es mi meta de aprendizaje?** (Ej: "Quiero entender sólidamente la diferencia entre datos estructurados y no estructurados. Mi objetivo principal es dominar el concepto de 'Metadata', ya que parece ser la 'llave' que le da contexto y valor a los datos.")
* **¿Qué estrategia utilizaré?** El Método de Deconstrucción Aplicada 2.0.

---

## Paso 1: Vistazo al Resultado Final - El Caso de un "Smart Home" (IoT)

Para entender "Data Literacy", he deconstruido un ecosistema donde la variedad y el contexto de los datos es todo: un Hogar Inteligente (como Google Home o Alexa).

### Análisis Guiado

* **El Problema de Negocio:** La meta de un Smart Home es la **automatización y la asistencia proactiva**. El desafío es: ¿cómo un sistema "entiende" los comandos y el estado de una casa?

* **Los Conceptos del Módulo en Acción:**
    1.  **Fuentes de Datos (Data Sources):** El sistema recolecta datos de múltiples fuentes simultáneamente: **Sensores** (termostato, cámaras), **Entrada del Usuario** (voz, app) y **APIs Externas** (el servicio del clima).
    2.  **Tipos de Datos (Understanding Data):** Estas fuentes generan una gran variedad de tipos:
        * **Datos Estructurados:** `21.5°C` (numérico del termostato), `true/false` (booleano del sensor de la puerta).
        * **Datos No Estructurados:** El archivo de audio de mi voz, el stream de video de la cámara.
    3.  **Metadata (¡El Concepto Clave!):** Los datos crudos no sirven de nada. El valor está en sus "datos sobre los datos".
        * El dato **`21.5`** es inútil.
        * La **Metadata** es lo que lo hace accionable:
            * **Metadata de Proceso:** `timestamp: '2025-11-05T14:10:00Z'` (cuándo se midió).
            * **Metadata Técnica:** `unit: 'celsius'` (qué significa el número).
            * **Metadata de Negocio:** `location: 'Sala de Estar'` (dónde está el sensor).

* **El Resultado Observable (La "Magia"):**
    Cuando le digo a Alexa "tengo frío", el sistema funciona gracias a la metadata:
    1.  Recibe un dato de **audio (no estructurado)**.
    2.  La **metadata** de la bocina le dice que estoy en la "Sala de Estar".
    3.  Busca el sensor que también tenga la **metadata** `location: 'Sala de Estar'`.
    4.  Compara la temperatura de ese sensor con una regla de negocio ("frío" < 22°C) y envía un comando.

**Conclusión del Paso 1:** Este caso me demuestra que la "alfabetización de datos" no es solo saber qué es un CSV. Es entender que los datos crudos no tienen valor sin un contexto. La **Metadata** es el sistema de contexto que permite que los algoritmos tomen decisiones inteligentes.

## Paso 2: Fundamentos Conectados a la Realidad

Aquí documentaré mis notas de cada lección, conectándolas siempre con nuestro caso de estudio del "Smart Home".

### 🎥 "Understanding Data"
* (Tus notas aquí... ¿Cuáles son los tipos de datos? Ej: Estructurados vs. No Estructurados vs. Semi-Estructurados. ¿Numéricos, categóricos, texto, video?)
* **Conexión con el Caso Práctico:** (Ej: "El termostato genera datos **estructurados numéricos** (21°C). Mi voz pidiendo una canción es un dato **no estructurado de audio**.")

### 🎥 "Data Sources"
* (Tus notas aquí... ¿De dónde vienen los datos? Ej: Bases de datos internas, APIs externas, sensores (IoT), entrada manual del usuario.)
* **Conexión con el Caso Práctico:** (Ej: "Las fuentes de datos en el Smart Home son: **Sensores** (termostato, cámara), **Entrada del Usuario** (mi voz, la app del celular), y **APIs Externas** (el servicio del clima para decidir la temperatura).")

### 🎥 "Working on Varied Data Sources and Types"
* (Tus notas aquí... ¿Cuáles son los retos? ¿Cómo se combina un JSON de una API con una tabla de SQL? ¿Cómo se "limpia" un dato de texto?)
* **Conexión con el Caso Práctico:** (Ej: "El reto es combinar todas estas fuentes. El sistema tiene que tomar mi voz (audio no estructurado), convertirla a texto, entender que 'tengo frío' (análisis de texto), y luego enviar un comando numérico (estructurado) al termostato.")

### 📖 "Metadata"
* (Tus notas aquí... ¿Qué es Metadata?
    * **Metadata Técnica:** (Ej: tipo de dato, tamaño del archivo).
    * **Metadata de Proceso:** (Ej: cuándo se capturó el dato).
    * **Metadata de Negocio:** (Ej: a qué habitación pertenece el sensor).
* **Conexión con el Caso Práctico:** (¡Esta es la clave de todo!) (Ej: "El dato '21°C' no significa nada. La **Metadata** es lo que le da valor: {`sensor_id: 'termo_sala'`, `unit: 'celsius'`, `timestamp: '2025-11-05T14:00:00Z'`, `location: 'Sala de Estar'`}. Sin metadata, la casa no 'entiende' nada.")

---

## 🚀 Conclusión del Módulo

(Escribe tu reflexión final aquí cuando termines el módulo).
* **¿Qué funcionó bien?**
* **¿Cuál es el concepto de 'Metadata' más importante que aprendí?**
* **¿Por qué es tan difícil trabajar con datos no estructurados?**

---

## Glosario del Módulo
(Aquí puedes pegar la tabla del glosario cuando la tengas).
