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

* * **What Do Data Scientists Do?**
¿Cuál es la importancia de Big Data para un Data Scientist?

¿Con cuáles tipos de formatos de archivos trabaja un Data Scientist? 
Es importante saber cuáles son los tipos de formatos de archivos que existen para un Data Scientist, ya que cada tipo tendrá sus respectivos beneficios y limitaciones. Al conocer esto, el profesional tomara mejores decisiones dependiendo de sus necesidades de datos y rendimiento. Los formatos Standard son: 
1. Delimited text file formats (p.e. .CSV o .TSV) -> Son usados para almacenar datos como texto, donde cada valor es separado mediante un delimitador, el cuál es una secuencia de uno o más caracteres para especificar el límite entre valores independientes. Los delimitadores más usuales son comas, tab, espacio, barra vertical, entre otros. .CSV = comma-separated values y .TSV = tab-separated-values son los más usuales. La primera fila de datos es la cabecera de la columna, donde cada columna puede tener tipos de datos distintos. Los archivos delimitados permiten valores de campo de cualquier magnitud y pueden ser procesados por casi todas las aplicaciones existentes. 
2. Microsoft Excel Open .XML Spreadsheet (.XLSX) -> Es un formato basado en XML que entra dentro del formato de archivo de hoja de cálculo. En él puede haber múltiples hojas de trabajo. Cada una de las hojas de trabajo está organizada en filas y columnas y la intersección entre cada una es una celda. Cada celda contiene datos. .XLSX es un formato de archivo abierto, lo que significa que generalmente es accesible para la mayoría de las otras aplicaciones. Este formato puede utilizar y guardar todas las funciones dosponibles en Excel y también es conocido por ser uno de los formatos de archivo más seguros ya que no puede guardar código malicioso. 
3. Extensible Markup Language (.XML) -> Es un lenguaje markup con reglas establecidas para codificar datos. Este formato es legible tanto para máquinas como para humanos. Es un lenguajr auto descriptivo diseñado para enviar informes a través de internet. Tiene algunas similitudes con .HTML pero también tiene diferencias, como que .XML no utiliza etiquetas predefinidas como sí lo hace .HTML. .XML es independiente de la plataforma y lenguaje de programación, por lo que simplifica el intercambio de datos entre varios sistemas. 
4. Portable Document Format (.PDF) -> Es un tipo de formato de archivo desarrollado por Adobe para presentar documentos independientes a la aplicación, software, hardware y sistemas operativos, lo que significa que puede ser visto de la misma manera en cualquier dispositivo. Puede utilizarse para completar datos tales como para formularios. 
5. JavaScript Object Notation (.JSON) ->  Es un tipo de formato de archivo basado en texto diseñado para transmitir datos estructurados en la web. Puede leerse en cualquier lenguaje de programación, es fácil de usar, es compatible con una amplia gama de navegadores y es considerada como una de las mejores herramientas para compartir datos de cualquier tamaño y tipo, incluso audio y video. Esta es una razón por la que muchas API y Servicios Web devuelven datos como JSON.

¿Cuáles son los principales algoritmos usados por un Data Scientist?

¿Cuándo se le puede llamar a alguien Data Scientist? 

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
### Glosario (Continuación)

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
| Nearest neighbor | A machine learning algorithm that predicts a target variable based on its similarity to other values in the dataset. | Working on Different File FormS Formats |
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
