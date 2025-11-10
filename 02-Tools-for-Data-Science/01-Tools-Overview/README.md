# Curso 2: Tools for Data Science
## Módulo 1: Visión General de las Herramientas

Este módulo es mi primera inmersión en la "caja de herramientas" del Científico de Datos. El objetivo es entender el ecosistema de software que existe, por qué hay tantas herramientas y en qué categoría cae cada una.

## 🎯 Mi Objetivo con este Módulo

* **¿Qué sé ya sobre esto?** (Ej: "He oído hablar de Python y R. Supongo que hay herramientas para 'Big Data' (como vi en el curso anterior) y herramientas para 'visualizar'. No tengo clara la diferencia entre 'Open Source', 'Cloud' y 'Comercial'.")
* **¿Cuál es mi meta de aprendizaje?** (Basado en los objetivos del módulo) "Quiero poder describir el toolkit de un Data Scientist, listar las categorías de herramientas y dar ejemplos de Open Source (gratuitas), Comerciales (de paga) y Basadas en la Nube (Cloud)."
* **¿Qué estrategia utilizaré?** El Método de Deconstrucción Aplicada 2.0.

---
## Paso 1: Vistazo al Resultado Final - El Caso de un E-commerce (Amazon/MercadoLibre)

Para entender por qué existen tantas herramientas de Data Science, he deconstruido un proyecto común: un **sistema de recomendación** ("Los clientes que compraron esto también compraron...").

### Análisis Guiado: El Viaje del Proyecto y su "Toolkit"

Un solo proyecto de datos pasa por múltiples etapas, y cada una usa un tipo de herramienta diferente. No existe "una herramienta para todo".

* **El Problema de Negocio:** Aumentar el valor promedio del carrito de compras sugiriendo productos relevantes.

* **Las Herramientas (El "Toolkit" en Acción):**
    1.  **La "Cantera" (Almacenamiento):** Primero, todos los datos de las compras se guardan en una base de datos.
        * **Herramienta:** **SQL**.
    2.  **El "Taller" (Análisis):** Un Data Scientist explora y limpia millones de transacciones para entender los patrones de compra.
        * **Herramienta (Open Source):** **Jupyter Notebooks** y **Python** (con Pandas).
    3.  **El "Motor" (Modelado):** Se construye el algoritmo de ML que aprende los patrones y genera las recomendaciones.
        * **Herramienta (Open Source):** **Python** (con Scikit-learn).
    4.  **El "Dashboard" (Visualización):** El gerente de marketing necesita ver el impacto en las ventas en un gráfico.
        * **Herramienta (Comercial):** **Tableau** o **Power BI**.
    5.  **La "Fábrica" (Despliegue):** El modelo debe funcionar para millones de usuarios en tiempo real en el sitio web, 24/7. No puede correr en una laptop.
        * **Herramienta (Cloud-based):** **IBM Watson Studio** o **AWS SageMaker**.

**Conclusión del Paso 1:** Este caso me demuestra por qué el curso divide las herramientas en categorías. Un Data Scientist exitoso no es un experto en *una* herramienta, sino que sabe *qué tipo* de herramienta (Open Source, Comercial o Cloud) usar en *cada etapa* del proyecto, desde el "Taller" hasta la "Fábrica".

## Paso 2: Fundamentos Conectados a la Realidad

## OpenSource tools: 

### Data management tools
  - MySQL: Is a open source RDBMS that uses Structured Query Language (SQL) para manipular y almacenar datos. Su uso común es en web applications e e-commerce. 
  - PostgreSQL: Is a RDBMS que enfatiza en cumplimuento de extensibilidad y SQL, ofrece características avanzadas como soporte a JSON, búsqueda full text y spacial data. 
  - (apache) cassandra: Base de datos NoSQL altamente escalable y distribuida que puede lidiar con grandes cantidades de data estructurada y no estructurada. 
  - elasticsearch: REASTful search y motor de análisis altamente escalable y fácil de usar con capacidades de consulta potentes. 
  - ceph: Is a open source storage platform diseñado para data centers modernos.
  - CouchDB: Es un NoSQL orientado a documentos que usa JSON para almacenar datos. 
  - mongoDB: Es como CouchDB a modo para aplicaciones de web modernas que lidian con grandes volúmenes de data no estructurada. 
  - Hadoop HDFS: Sistema de archivos que proporciona un alto rendimiento de acceso a datos de aplicación.

### Operating system tools
  - Jupyter: Es un IDE que soporta desarrollo en Julia, Python y R con Jupyter Notebook, Jupyter Lab y Jupyter Hub. Jupyter Lab incluye notebooks personalizados para organizaciones y JupyterHub extiende esas capacidades para empresas. 
  - RStudio: Es un IDE construida para gestionar y ejecutar código en R. 
  - Microsoft Visual Studio: IDE que soporta varios lenguajes como C, C++, C++/CLI, Visual Basic, .NET, C#, F#, JavaScript, TypeScript, XML, XSLT, HTML y CSS, así como Python, Ruby, Node.js y M. 
  - Pycharm: IDE de suscripción que ofrece más de 16 herramientas adicionales para codificar, asistencia, testeo y desarrollo. 
  - Spyder: IDE diseñada para científicos, ingenieros y analistas de datos, incluye una combinación de herramientas de desarrollo integral para editado avanzado, analisis, depuración, etc. 
  - Anaconda Navigator: Is an GUI-based Navigator that supports Python development.

### Data integration and transformation tools
  - Apache Spark SQL: Es un módulo del ecosistema Spark que proporciona una interfaz de programación para trabajar con structured data usando SQL, data frames y datasets.
  - Kubeflow: Es una caja de herramientas de machine learning construida sobre Kubernetes que proporciona una plataforma para construir, implementar y gestionar flujos de trabajo de machine learning end to end.
  - Node-RED: Es una herramienta de programación visual para conectar juntos hardware, APIs y servicios online.
  - Apache Airflow: Es una plataforma para programáticamente crear, calendarizar y monitorear flujos de trabajo.
  - Apache Nifi: Es una platafora de integración que permite a los usuarios automatiar el flujo de datos entre sistemas.
  - Apache Kafka: Es una plataforma de flujos que permite a aplicaciones publicar, procesar y suscribir a flujos de registros en tiempo real.

### Data visualization tools
  -   Tableau and PowerBI are used for dara visualization, but data scientist use other tools.
  -   PixieDust: Es una librería para crear visualizaciones exploratorias de datos en Python y Jupyter Notebooks.
  -   Kibana: Herramienta de visualización que permite a los usuarios interactuar con su propia data a través de una interfaz basada en la web.
  -   Hue: Es una interfaz web para analizar y visualizar conjuntos de datos grandes en Apache Hadoop.
  -   Apache Superset: Es una aplicación web moderna para empresas que buscan inteligencia empresarial que hace fácil de visualizar y explorar grandes datasets. 

### Model deployment tools
  - Apache PredictionIO: Es un servidor de machine learning construido sobre una infraestructura distribuida y escalable. 
  - Kubernetes: Plataforma de orquestración de contenedores que automáicamente lanza, escala y gestiona aplicaciones contenidas. 
  - MLeap: Librería para serialización y deserialización de modelos de aprendizaje en una en un archivo multipropósito. Le da a los usuarios la habilidad de exportar modelos desde diferentes librerías y frameworks tales como Spark, scikit-learn y TensorFlow.
  - TensorFlow Lite: Es una herramienta para correr modelos de ML en dispositivos móviles y embebidos. 
  - Apache Seldon: Plataforma para implementar y gestionar ML models sobre Kubernetes. 
  - OpenShift: Container application framework basado en Kubernets con características como automatización ,escalabilidad y seguridad, ofrece un método para crear, implementar y gestionar containerized applications. 
  - TensorFlow Serving: Es una utilidad que sirve ML models en configuraciones del mundo real. 
  - TensorFlow.js: Librería que sirve para construir e implementar ML models en JavaScript. 

### Model monitoring and assessment tools
  - IBM AI Fairness 360: Conjunto de herramientas para detectar y mitigar sesgo en modelos de ML.  
  - IBM AI Explainability 360: Conjunto de herramientas para explicar el comportamiento y decisiones de modelos de ML.
  - IBM Adversarial Robustness 360 Toolbox: Librería para proteger ML models de ataques adversarios.  
  - Prometheus: Sistema de monitoreo que colecta y almacena métricas en tiempo real desde distintas fuentes. 
  - ModelDB: Plataforma de gestion de ML models y experimentos.

### Code asset tools
  - Git: VCS para rastrear cambios en código y colaboración entre desarrolladores. 
  - GitLab: Es un repositorio web basado en Git que proporciona una completa plataforma de Operaciones de desarrollo.
  - GitHub: Repositorio web basado en Git que proporciona una plataforma para desarrolladores para colaborar en código y gestionar proyectos de software. 
  - Bitbucket: Es un VCS que proporciona a los desarrolladores una paltaforma para colaborar en código y gestionar proyectos de software.

### Data asset tools
  - ODPi Egeria es un framework de gestionamiento de metadata que proporciona una manera estándar de gestionar y compartir metadatos a través de diferentes plataformas y herramientas.
  - Kylo: Es una plataforma diseñada para simplificar los procesos de datos.
  - Apache Atlas: Framework de gestionamiento y gobernanza de metadatos para ecosistemas Hadoop. 

## Comercial tools: 
Data Management Tools

Key players include Oracle Database, Microsoft SQL Server, and IBM Db2, which are considered industry standards.
Commercial support from vendors is crucial for effective data management.
Data Integration Tools

Leaders in this category are Informatica PowerCenter and IBM InfoSphere DataStage, along with SAP, Oracle, and Microsoft products.
These tools facilitate the design and deployment of ETL (Extract, Transform, Load) processes through graphical interfaces.
Data Visualization and Model Building Tools

Prominent visualization tools include Tableau, Microsoft Power BI, and IBM Cognos Analytics, aimed at creating reports and dashboards.
For model building, SPSS Modeler and SAS Enterprise Miner are highlighted, with SPSS Modeler also available in Watson Studio Desktop for cloud-based applications.
---

# 🧰 Caja de Herramientas del Científico de Datos

A continuación se presenta un desglose de las categorías de herramientas esenciales y ejemplos populares dentro de cada una.

---

## 1. Herramientas de Gestión de Datos (Data Management)
*Facilita el almacenamiento, la organización y la recuperación de datos. Incluye bases de datos relacionales, NoSQL y plataformas de Big Data.*

### MySQL
* Popular sistema de gestión de bases de datos relacionales (RDBMS) de código abierto.
* Utiliza SQL (Structured Query Language) para gestionar y almacenar datos.
* **Usos comunes:** Aplicaciones web, Data Warehousing, E-commerce.

### PostgreSQL
* Potente sistema de gestión de bases de datos relacionales (RDBMS) de código abierto.
* Enfatiza la extensibilidad y el cumplimiento de SQL.
* **Ofrece características avanzadas como:** Soporte para JSON, búsqueda de texto completo, datos espaciales.

### Apache CouchDB
* Base de datos NoSQL orientada a documentos.
* Utiliza JSON para almacenar datos.
* Altamente escalable, tolerante a fallos y fácil de usar.

### MongoDB
* Base de datos NoSQL orientada a documentos.
* Almacena datos en un formato JSON flexible.
* **Proporciona:** Escalabilidad, alta disponibilidad y distribución de datos.
* **Adecuado para:** Aplicaciones web modernas que manejan grandes volúmenes de datos no estructurados.

### Apache Cassandra
* Base de datos NoSQL orientada a documentos, distribuida y altamente escalable.
* Puede manejar grandes cantidades de datos estructurados y no estructurados a través de muchos servidores básicos.
* **Ofrece:** Alta disponibilidad, tolerancia a fallos y niveles de consistencia ajustables.
* **Adecuado para:** Aplicaciones de misión crítica.

### Hadoop Distributed File System (HDFS)
* Diseñado para trabajar con grandes conjuntos de datos (como Apache Hadoop) en un entorno de computación distribuida.
* Procesamiento de datos de alto rendimiento al dividir archivos en bloques (default 128MB), distribuidos en múltiples DataNodes.
* Los datos se replican en diferentes DataNodes, asegurando alta disponibilidad y tolerancia a fallos.
* Escalable y eficiente.

### Ceph
* Plataforma de almacenamiento definida por software, gratuita y de código abierto, adecuada para entornos de nube híbrida.
* Diseñada para centros de datos modernos.
* Proporciona un sistema de almacenamiento unificado y altamente escalable para: almacenamiento de objetos (como AWS S3), almacenamiento en bloques (discos virtuales) y almacenamiento de archivos (como NFS).
* Alto rendimiento, disponibilidad y fiabilidad.

### Elasticsearch
* Principalmente un motor de búsqueda y herramienta de análisis RESTful distribuido.
* Basado en la biblioteca Lucene.
* **Ofrece:** Búsqueda de texto completo, análisis de datos en tiempo real, alta escalabilidad.
* Fácil de usar, potentes capacidades de consulta e indexación de datos en tiempo real.

---

## 2. Herramientas de Integración y Transformación de Datos (ETL)
*Agiliza las canalizaciones de datos (data pipelines) y automatiza los flujos de trabajo de procesamiento. La tarea clásica es Extraer, Transformar y Cargar (ETL).*

### Apache Airflow
* Plataforma de código abierto para crear, programar y monitorear flujos de trabajo de forma programática.
* Creada originalmente por Airbnb.
* Permite a los usuarios definir y ejecutar flujos de trabajo complejos con soporte para dependencias, paralelismo y manejo de errores.

### Kubeflow
* Un conjunto de herramientas de machine learning de código abierto que permite la ejecución de pipelines de ciencia de datos sobre Kubernetes.
* Proporciona una plataforma para construir, desplegar y gestionar flujos de trabajo de ML de extremo a extremo a escala.
* **Soporte para:** Entrenamiento distribuido, servicio de modelos, ajuste de hiperparámetros.

### Apache Kafka
* Plataforma de streaming distribuida que permite a las aplicaciones publicar, procesar y suscribirse a flujos de récords en tiempo real.
* Creada originalmente por LinkedIn.
* Es escalable, tolerante a fallos y de alto rendimiento (high-throughput).
* **Adecuado para:** Construir aplicaciones de misión crítica e intensivas en datos.

### Apache NiFi
* Plataforma de integración de datos de código abierto que permite a los usuarios automatizar el flujo de datos entre sistemas.
* Proporciona una interfaz de usuario web para diseñar y gestionar flujos de datos.
* **Soporte para:** Enrutamiento de datos, transformación, enriquecimiento y otras capacidades.

### Apache Spark SQL
* Un módulo en el ecosistema de Spark que proporciona una interfaz de programación para trabajar con datos estructurados usando SQL, DataFrames y Datasets.
* Soporta una amplia gama de fuentes de datos y proporciona un rendimiento optimizado.

### Node-RED
* Herramienta de programación visual de código abierto para conectar dispositivos de hardware, APIs y servicios en línea.
* Permite a los usuarios crear flujos de mensajes controlados por eventos.
* Su consumo de recursos es tan bajo que incluso funciona en dispositivos pequeños como una Raspberry Pi.
* **Soporte para:** Transformación, filtrado y agregación de datos.

---

## 3. Herramientas de Visualización de Datos
*Proporciona una representación gráfica de los datos y ayuda a comunicar los "insights" (hallazgos clave).*

### PixieDust
* Biblioteca de código abierto para crear visualizaciones de datos interactivas y exploratorias en Python y Jupyter notebooks.
* Proporciona visualizaciones integradas y conectores de datos.
* Soporta personalización y extensibilidad.

### Hue
* Interfaz web de código abierto para analizar y visualizar grandes conjuntos de datos en Apache Hadoop.
* Ofrece una experiencia amigable para explorar datos y crear visualizaciones sin necesidad de habilidades de programación; puede crear visualizaciones desde consultas SQL.

### Kibana
* Herramienta de visualización de datos de código abierto que permite a los usuarios interactuar con sus datos a través de una interfaz web.
* Comúnmente usada con Elasticsearch para analizar y visualizar grandes conjuntos de datos.

### Apache Superset
* Una aplicación web de inteligencia de negocios (BI) moderna y lista para empresas que facilita la visualización y exploración de grandes conjuntos de datos.
* Ofrece un rico conjunto de opciones de visualización, incluyendo gráficos, tablas, mapas, análisis geoespacial y procesamiento de datos en tiempo real.

---

## 4. Herramientas de Despliegue de Modelos (Model Deployment)
*Soporta la construcción y despliegue (puesta en producción) de modelos de datos y machine learning.*

### Apache PredictionIO
* Servidor de machine learning de código abierto construido sobre una infraestructura escalable y distribuida.
* Permite a los desarrolladores construir, evaluar y desplegar rápidamente motores predictivos para recomendación, clasificación,

## 🚀 Conclusión del Módulo

(Escribe tu reflexión final aquí cuando termines el módulo).
* **¿Qué funcionó bien?**
* **¿Cuál es la diferencia más clara que entendí entre herramientas Open Source, Cloud y Comerciales?**
* **¿Por qué un Data Scientist no puede usar una sola herramienta para todo?**

---

## Glosario del Módulo
(Aquí puedes pegar la tabla del glosario cuando la tengas).
