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

---

## Paso 2: Fundamentos Conectados a la Realidad

Aquí documentaré mis notas de cada lección, conectándolas siempre con el caso de Uber.

### 🎥 "A Day in the Life of a Data Scientist"

* (Tus notas aquí... ¿Qué tareas hacen? ¿Pasan más tiempo limpiando datos o creando modelos? ¿Con quién hablan?)
* **Conexión con el Caso Práctico:**

### 🎥 "Data Science Skills and Big Data"

* **Habilidades Clave:**
    * Habilidad 1: Python (pandas)
    * Habilidad 2: Linux
    * Habilidad 3: Databases
    * Habilidad 4: Math (calculus, algebra, statistics, probability)

* **¿Cuál es la importancia de Big Data para un Data Scientist?**
    El concepto de Big Data se refiere a conjuntos de datos que son tan grandes y complejos que requieren herramientas y técnicas especiales para su procesamiento y análisis. En el video, se menciona que lo que antes se consideraba Big Data está en constante evolución debido a la innovación tecnológica. Esto implica que las herramientas y software, como Hadoop, han ampliado las capacidades de manejo de datos, permitiendo a los científicos de datos trabajar con volúmenes de información que antes eran impensables.

* **Conexión con el Caso Práctico:**
    Uber es un ejemplo perfecto de Big Data porque genera millones de puntos de GPS por segundo (Velocidad, Volumen y Variedad).

### 🎥 "Working on Different File Formats"

* **¿Con cuáles tipos de formatos de archivos trabaja un Data Scientist?**
    Es importante saber cuáles son los tipos de formatos de archivos que existen para un Data Scientist, ya que cada tipo tendrá sus respectivos beneficios y limitaciones. Los formatos Standard son:
    1.  **Delimited text file formats (p.e. .CSV o .TSV):** Son usados para almacenar datos como texto, donde cada valor es separado mediante un delimitador (ej. comas o tabs). La primera fila suele ser la cabecera.
    2.  **Microsoft Excel Open .XML Spreadsheet (.XLSX):** Formato basado en XML para hojas de cálculo. Puede tener múltiples hojas y es un formato abierto accesible para la mayoría de las aplicaciones.
    3.  **Extensible Markup Language (.XML):** Lenguaje de marcado con reglas para codificar datos, legible tanto para máquinas como para humanos. Diseñado para enviar informes a través de internet, es independiente de la plataforma.
    4.  **Portable Document Format (.PDF):** Formato de archivo de Adobe para presentar documentos independientes de la aplicación, software o hardware.
    5.  **JavaScript Object Notation (.JSON):** Formato basado en texto diseñado para transmitir datos estructurados en la web. Puede leerse en cualquier lenguaje, es fácil de usar y es ideal para compartir datos, por lo que muchas APIs y Servicios Web devuelven datos en JSON.

* **Datos estructurados y no estructurados**
    Una manera sencilla de verlo es:
    * **Datos estructurados:** Aquellos que están organizados en filas y columnas, como en un archivo de excel.
    * **Datos no estructurados:** Aquellos que no están organizados en filas y columnas, como texto plano, audio o video.
    * *Nota:* Para poder trabajar con los datos, deben estar estructurados. En ocasiones, se pasa mucho tiempo limpiando y estructurando datos no estructurados para poder trabajar con ellos.

* **Conexión con el Caso Práctico:**
    El perfil de un usuario de Uber (nombre, email, foto) probablemente se guarda como un **JSON**. El historial de todos sus viajes (fecha, costo, inicio, fin) seguro es una tabla en una base de datos que se podría exportar como un **CSV**.

### 🎥 "Data Science Topics and Algorithms"

Algunos de los temas y algoritmos más importantes para un Data Scientist son:

* **Regresión:**
    Vamos a desglosar el concepto de regresión utilizando el ejemplo del taxi. Imagina que tomas un taxi. Hay un costo fijo de $2.50 solo por subirte (la "constante"). A medida que el taxi se mueve, la tarifa aumenta por cada 100 metros (relación entre distancia y costo). Si el taxi se detiene, cada minuto también incrementa la tarifa (relación entre tiempo y costo). La regresión es la herramienta que nos ayuda a entender y calcular estas relaciones (tarifa base, costo por distancia, costo por tiempo) para predecir el costo total.

* **Algoritmo k-Nearest Neighbor (k-NN):**
    Using complicated machine learning algorithms does not always guarantee achievin a better performance. Occasionally, a simple algorithm such as k-nearest neighbor can yield a satisfactory performance.
    El k-NN es una técnica de clasificación que agrupa datos buscando los "k" puntos de datos más cercanos a un nuevo dato y determina a qué categoría pertenece basándose en la mayoría de esos vecinos. Por ejemplo, para saber si un email es "spam", el algoritmo mira los 'k' correos más similares y lo clasifica en la categoría que más se repita entre ellos.

* **Otros temas mencionados:** Data Visualization, Redes Neuronales Artificiales, R, Python.

* **Conexión con el Caso Práctico:**
    El algoritmo que usa Uber para calcular el 'precio dinámico' (surge pricing) es un algoritmo de **regresión** o similar, que predice la demanda y la oferta en tiempo real.

### 📖 "What Makes Someone a Data Scientist?"

* **Reflexiones de la lectura:**
    I define a data scientist as someone who finds solutions to problems by analyzing Big or small data using appropriate tools and then tells stories to communicate her findings to the relevant stakeholders. I do not use the data size as a restrictive clause.

    It is important to realize that one who tries to set arbitrary thresholds to exclude others is likely to run into inconsistencies.

    Data scientist is that unique blend of skills that can both unlock the insights of data and tell a fantastic story via the data.

    The other key ingredient for a successful data scientist is a behavioral trait: **curiosity**. The best data scientist tend to be really curious people, thinkers who ask good questions and are O.K. dealing with unstructured situations and trying to find structure in them.

    Data Science is a journey of exploration, innovation and storytelling.

---

## Glosario (Continuación)

| Term | Definition | Video where the term is introduced |
| --- | --- | --- |
| Comma-separated values (CSV) / Tab-separated values (TSV) | Commonly used format for storing tabular data as plain text where either the comma or the tab separates each value. | Working on Different File Formats |
| Data file types | A computer file configuration is designed to store data in a specific way. | Working on Different File Formats |
| Data format | How data is encoded so it can be stored within a data file type. | Working on Different File Formats |
| Data visualization | A visual way, such as a graph, of representing data in a readily understandable way makes it easier to see trends in the data. | Data Science Topics and Algorithms |
| Delimited text file | A plain text file where a specific character separates the data values. | Working on Different File Formats |
| Extensible Markup Language (XML) | A language designed to structure, store, and enable data exchange between various technologies. | Working on Different File Formats |
| Hadoop | An open-source framework designed to store and process large datasets across clusters of computers. | What Makes Someone a Data Scientist |
| JavaScript Object Notation (JSON) | A data format compatible with various programming languages for two applications to exchange structured data. | Working on Different File Formats |
| Jupyter notebooks | A computational environment that allows users to create and share documents containing code, equations, visualizations, and explanatory text. See Python notebooks. | Data Science Skills & Big Data |
| Nearest neighbor | A machine learning algorithm that predicts a target variable based on its similarity to other values in the dataset. | Working on Different FileS Formats |
| Neural networks | A computational model used in deep learning that mimics the structure and functioning of the human brain's neural pathways. It takes an input, processes it using previous learning, and produces an output. | A Day in the Life of a Data Scientist |
| Pandas | An open-source Python library that provides tools for working with structured data is often used for data manipulation and analysis. | Data Science Skills & Big Data |
| Python notebooks | Also known as a “Jupyter” notebook, this computational environment allows users to create and share documents containing code, equations, visualizations, and explanatory text. | Data Science Skills & Big Data |
| R | An open-source programming language used for statistical computing, data analysis, and data visualization. | Data Science Skills & Big Data |
| Recommendation engine | A computer program that analyzes user input, such as behaviors or preferences, and makes personalized recommendations based on that analysis. | A Day in the Life of a Data Scientist |
| Regression | A statistical model that shows a relationship between one or more predictor variables with a response variable. | Data Science Topics and Algorithms |
| Tabular data | Data that is organized into rows and columns. | A Day in theLife of a Data Scientist |
| XLSX | The Microsoft Excel spreadsheet file format. | Working on Different File Formats |

---

## 🚀 Conclusión del Módulo

(Escribe tu reflexión final aquí cuando termines el módulo).

* **¿Qué funcionó bien?**
* **¿Qué me costó más trabajo?**
* **¿Cómo cambió mi entendimiento del rol?**
