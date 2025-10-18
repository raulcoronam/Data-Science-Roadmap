# Curso 1: What's Data Science?

- Define data science and its importance in today’s data driven world.
- List some paths that can lead to a career in data science.
- Summarize advice given by seasoned data science professionals to data scientists who are just starting out.
- Articulate why data science is considered the most in-demand job in the 21st century.
- Describe what a typical day in the life of a data scientist looks like.
- Define some of the commonly used terms in data science.
- Identify some of the key qualities of a successful data scientist.

- ## 🎯 Mi Objetivo con el Módulo: What is Data Science? 

* **¿Qué sé ya sobre esto?** He oído que Data Science es ahora fundamental para las empresas, especialmente las grandes, ya que utilizan datos para entender mejor al cliente, entender mejor sus números y entender a la empresa en general y así, crecer. He oído que se usa para recomendaciones como las de Netflix, pero no sé exactamente cómo funciona. La ciencia de datos utiliza los datos para comprender el mundo que nos rodea. 
* **¿Cuál es mi meta de aprendizaje?** Mi objetivo es entender a ciencia cierta, qué es Data Science, cómo es el dá a día de un Data Scientist, quiero conocer si es el campo laboral al que me quiero dedicar y cómo sería mi vida si me dedico a ello. 
* **¿Qué estrategia utilizaré?** El Método de Deconstrucción Aplicada 2.0.

## Paso 1: Vistazo al Resultado Final - El Caso de Netflix

Mi método de aprendizaje inicia deconstruyendo un caso real para entender el "para qué" antes de estudiar la teoría (el "como"). He elegido el sistema de recomendación de Netflix.

### Análisis Guiado

* **El Problema de Negocio:** El objetivo principal no es solo recomendar, sino **reducir la tasa de cancelación de usuarios**. El sistema busca maximizar el valor de la suscripción mostrándome contenido relevante de forma rápida para mantenerme enganchado.

* **Los Datos Utilizados (La Materia Prima):** El sistema se alimenta de mis acciones:
    * **Datos Explícitos:** Calificaciones que doy (👍), mi idioma, lo que añado a "Mi Lista".
    * **Datos Implícitos:** Mi historial de visualización, si termino o abandono una película, la hora en que veo contenido, el dispositivo que uso, e incluso lo que busco.

* **El Resultado Observable:** La experiencia de Netflix está completamente personalizada por los datos:
    * Las **filas de categorías** que veo ("Porque viste...").
    * El **orden** en que se presentan las películas y series.
    * Incluso la **imagen de portada** que me muestran para un mismo título.
    * El **porcentaje de coincidencia** que me anima a probar algo nuevo.

### Preguntas que me Surgen

Este primer análisis me deja con preguntas que espero resolver a medida que aprendo los fundamentos:
* ¿Cómo funciona con un usuario completamente nuevo que no tiene historial?
* ¿Cómo mide el sistema si una recomendación fue realmente "exitosa"?
* ¿Cómo equilibra mostrarme cosas que sabe que me gustan con sugerirme géneros nuevos que podría descubrir?

**Conclusión del Paso 1:** He confirmado que la Ciencia de Datos no es un ejercicio abstracto. Es una disciplina para construir "productos" que resuelven problemas de negocio utilizando datos. Este contexto me da un ancla mental para entender los conceptos que estudiaré a continuación.

## 🧠 ¿Qué aprendí aquí?

Este es el espacio para mis notas y reflexiones clave. Mi objetivo es explicar en mis propias palabras los conceptos más importantes.

* **¿Qué es realmente la Ciencia de Datos?**
Ciencia de datos es el proceso para entender diferentes cosas, para responder preguntas a aquello que se está explorando. La ciencia de datos es el campo de exploración, manipulación y análisis de datosm con el fin de responder a preguntas o hacer recomendaciones. La Ciencia de datos puede ayudar a las empresas a entender sus entornos, analizar problemas existentes y revelar oportunidades ocultas. Los científicos de datos buscan utilizar de la mejor manera los datos para proporcionar valor a la empresa. La Ciencia de Datos es esencial para aclarar la pregunta que la empresa quiere responder. Las mejores preguntas iniciales pueden ser: ¿Qué datos necesitamos para resolver el problema? ¿De dónde vendrán esos datos?. A veces se confirma lo que la empresa sospecha pero en otras ocasiones, puede llevar a conocimiento nuevo que lleva a la empresa a un nuevo enfoque.

Los datos te pueden hacer aprender: "Yo pensaba esto pero ahora con los datos, sé esto". 

* **El Rol de un Científico de Datos:**
Los científicos de datos requieren una combinación de habilidades, incluyendo conocimiento especializado en la materia, programación y habilidades de comunicación. Las 3 softskills principales de un científico de datos son la curiosidad (ayuda a plantear preguntas significativas), la argumentación (argumentos sólidos ayudan a explicar los hallazgos después de aprender de los datos) y el juicio (guía para empezar en la dirección correcta), aunque un cientifico de datos debe sentirse cómodo con las matemáticas y los algoritmos. 
Se encarga no solo de manipular, explofar y encontrar conclusiones sobre los datos, sino que también de hacer que la organización entienda dichos datos.
Una de las mayores características de un científico de datos es la curiosidad (para saber qué hacer con los datos) y la comunicación (para poder contar una historia). Si no logras contar una gran historia, tus hallazgos permanecerán ocultos. Los científicos de datos no provienen de un campo en particular, sino que usualmente vienen de varios campos como ingeniería, estadística e incluso psicología. Lo que tienen en común es el interés en entender los datos y aprender nuevas herramientas para trabajar con ellos. La ventaja competitiva de un científico de datos es ser especialista en un campo en específico. Es decir, tu ventaja competitiva es tu comprensión de algún aspecto de la vida donde tus habilidades exceden las de los demás. Después, tu ventaja competitiva debe concatenarse con tus habilidades analíticas y aquí es importante aprender platafomas/herramientas que sean específicas para el sector que te interesa. Por último, después de aprender las herramientas/plataformas, lo siguiente debe ser aplicar tus habilidades a problemas reales y mostrarle al mundo lo que puedes hacer.
Data -> Stories -> Insights or Clarify the problem -> Data collection -> Analysis -> Recognition -> Storytelling -> Visualization

* **What Do Data Scientists Do?**
¿Cuál es la importancia de Big Data para un Data Scientist?

¿Con cuáles tipos de formatos de archivos trabaja un Data Scientist? 

¿Cuáles son los principales algoritmos usados por un Data Scientist?

¿Cuándo se le puede llamar a alguien Data Scientist? 

* **El Ciclo de Vida de un Proyecto de Data Science:**

* **Diferencias entre Data Science, Data Analytics e IA:**
    * (Tus notas aquí... ¡un punto clave para no confundir términos!)
 
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
 
* **Dudas**
* **¿Qué son los datos estructurados y no estructurados?**

### Glosario de Data Science

| Term | Definition | Video where the term is introduced |
| --- | --- | --- |
| Algorithms | A set of step-by-step instructions to solve a problem or complete a task. | What is Data Science? |
| Model | A representation of the relationships and patterns found in data to make predictions or analyze complex systems retaining essential elements needed for analysis. | What is Data Science? |
| Outliers | When a data point or points occur significantly outside of most of the other data in a data set, potentially indicating anomalies, errors, or unique phenomena that could impact statistical analysis or modeling. | What is Data Science? |
| Quantitative analysis | A systematic approach using mathematical and statistical analysis is used to interpret numerical data. | Many Paths to Data Science |
| Structured data | Data is organized and formatted into a predictable schema, usually related tables with rows and columns. | What is Data Science? |
| Unstructured data | Unorganized data that lacks a predefined data model or organization makes it harder to analyze using traditional methods. This data type often includes text, images, videos, and other content that doesn't fit neatly into rows and columns like structured data. | What is Data Science? |

## 💻 ¿Cómo se usa este directorio?

* En esta carpeta guardaré mis apuntes principales en este `README.md`.
* Si hay algún script o notebook de Jupyter con código de ejemplo, lo añadiré aquí.
* Cualquier recurso externo (links a artículos, videos) que me haya sido útil, lo listaré en una sección de "Recursos".

## 🚀 Conclusión del Módulo

(Cuando termines el curso, escribe una pequeña reflexión aquí: ¿Qué fue lo que más te sorprendió? ¿Qué concepto te costó más trabajo? ¿Qué te gustaría explorar a continuación?)
