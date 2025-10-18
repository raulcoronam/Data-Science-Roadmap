# Módulo 2: What Do Data Scientists Do?

Este es mi diario de apuntes para el segundo módulo del curso. Continuaré aplicando mi **Método de Deconstrucción Aplicada (v2.0)** para conectar la teoría con la práctica.

## 🎯 Mi Objetivo con este Módulo

* **¿Qué sé ya sobre esto?** (Ej: "Sé que los Data Scientists usan algoritmos y ven datos, pero no tengo claro cómo es su día a día, ni qué herramientas (software) usan además de Python").
* **¿Cuál es mi meta de aprendizaje?** (Ej: "Quiero entender las diferentes tareas que realiza un DS, qué significa 'Big Data' en un sentido práctico y qué tipos de archivos de datos existen").
* **¿Qué estrategia utilizaré?** El Método de Deconstrucción Aplicada 2.0.

---

## Paso 1: Vistazo al Resultado Final - El Caso de Uber/Didi

Para entender qué hacen los Data Scientists, he analizado un producto que los utiliza intensamente: Uber (o Didi). Este caso me permite ver diferentes roles, algoritmos y, crucialmente, diferentes tipos de datos.

### Análisis Guiado

* **El Problema de Negocio:** No es solo "pedir un taxi". Es un problema de logística complejo que incluye:
    1.  **Matching:** Conectar eficientemente a conductores (oferta) con pasajeros (demanda).
    2.  **Pricing (Tarifa Dinámica):** Calcular un precio que balancee la oferta y la demanda en tiempo real (ej. si llueve o es hora pico).
    3.  **Logística (ETA):** Calcular el tiempo estimado de llegada y la ruta óptima.

* **Los Datos Utilizados (La Materia Prima):** Este sistema es un gran ejemplo de **Big Data** porque usa muchos tipos de datos diferentes, generados muy rápido.
    * **Datos Estructurados (Tablas):** Perfiles de usuario, historial de viajes (costo, fecha), calificaciones. Probablemente se verían como un **CSV** o tabla de Excel.
    * **Datos de Streaming (Tiempo Real):** La ubicación GPS de millones de conductores y pasajeros. Estos datos se envían en pequeños paquetes, probablemente en formato **JSON**.
    * **Datos Externos:** Mapas, datos del clima, tráfico en vivo y eventos (conciertos, partidos) para predecir la demanda.

* **El Resultado Observable (El Producto de Datos):** La app de Uber es una interfaz que nos muestra los resultados de múltiples algoritmos:
    1.  **El Precio:** Es el resultado de un algoritmo de "tarifa dinámica".
    2.  **El Tiempo de Llegada (ETA):** Es el resultado de un algoritmo de ruteo y predicción.
    3.  **El "Match":** La asignación del conductor es un algoritmo de optimización.
    4.  **Detección de Fraude:** Algoritmos que vigilan patrones extraños en los viajes.

**Conclusión del Paso 1:** Ahora entiendo que los Data Scientists en un lugar como Uber no solo hacen un modelo. Trabajan en problemas muy específicos (precios, rutas, fraude) y deben manejar una gran variedad de tipos de datos (tablas, JSONs, GPS) que llegan a una velocidad inmensa (Big Data).

## Paso 2: Fundamentos Conectados a la Realidad

Aquí documentaré mis notas de cada lección, conectándolas siempre con el caso de Uber o Netflix.

### 🎥 "A Day in the Life of a Data Scientist"
* (Tus notas aquí... ¿Qué tareas hacen? ¿Pasan más tiempo limpiando datos o creando modelos? ¿Con quién hablan?)
* **Conexión con el Caso Práctico:**

### 🎥 "Data Science Skills and Big Data"
* **Habilidades Clave:**
    * Habilidad 1: (Ej: Programación en Python/R)
    * Habilidad 2: (Ej: Estadística)
    * Habilidad 3: (Ej: Comunicación)
* **¿Qué es Big Data?** (Mi definición simple)
* **Conexión con el Caso Práctico:** (Ej: "Uber es un ejemplo perfecto de Big Data porque genera millones de puntos de GPS por segundo (Velocidad, Volumen y Variedad).")

### 🎥 "Working on Different File Formats"
* (Tus notas aquí... ¿Qué es un CSV? ¿Qué es un JSON? ¿Qué es un XML?)
* **Conexión con el Caso Práctico:** (Ej: "El perfil de un usuario de Uber (nombre, email, foto) probablemente se guarda como un **JSON**. El historial de todos sus viajes (fecha, costo, inicio, fin) seguro es una tabla en una base de datos que se podría exportar como un **CSV**.")

### 🎥 "Data Science Topics and Algorithms"
* (Tus notas aquí... ¿Qué es regresión? ¿Qué es un árbol de decisión?)
* **Conexión con el Caso Práctico:** (Ej: "El algoritmo que usa Uber para calcular el 'precio dinámico' (surge pricing) es un algoritmo de **regresión** o similar, que predice la demanda y la oferta en tiempo real.")

### 📖 "What Makes Someone a Data Scientist?"
* (Reflexiones de la lectura. ¿Hay una sola definición?)
* (Mi propia definición de lo que es un Data Scientist).

---

## 🚀 Conclusión del Módulo

(Escribe tu reflexión final aquí cuando termines el módulo).
* **¿Qué funcionó bien?**
* **¿Qué me costó más trabajo?**
* **¿Cómo cambió mi entendimiento del rol?**
