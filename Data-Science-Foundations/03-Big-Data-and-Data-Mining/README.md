# Módulo 3: Big Data and Data Mining

Este módulo se sumerge en la infraestructura que hace posible la ciencia de datos a gran escala. Aquí documentaré mi aprendizaje sobre Cloud, Big Data y las herramientas y técnicas para "minar" valor de conjuntos de datos masivos.

## 🎯 Mi Objetivo con este Módulo

* **¿Qué sé ya sobre esto?** (Ej: "He oído 'Big Data' mil veces, pero no sé qué lo define. 'Cloud' es como Google Drive, pero para empresas. 'Hadoop' y 'Spark' son nombres que he visto, pero no sé qué hacen.")
* **¿Cuál es mi meta de aprendizaje?** (Ej: "Quiero entender por qué un Data Scientist no puede usar solo su laptop. ¿Cuándo se vuelve 'Big Data' un problema? Y quiero entender la diferencia fundamental entre Hadoop, Spark y el 'Data Mining'.")
* **¿Qué estrategia utilizaré?** El Método de Deconstrucción Aplicada 2.0.

---

## Paso 1: Vistazo al Resultado Final - El Caso de Meta (Facebook)

Para entender "Big Data" y "Data Mining", he analizado a uno de sus pioneros y mayores usuarios: Meta. Ellos se enfrentaron a problemas de escala tan grandes que tuvieron que inventar sus propias herramientas.

### Análisis Guiado

* **El Problema de Negocio:**
    1.  **Para Usuarios:** Filtrar miles de publicaciones para mostrar solo el contenido más relevante en el News Feed y retener la atención del usuario.
    2.  **Para Anunciantes:** Permitir una segmentación híper-específica para que las marcas muestren anuncios solo a las audiencias que les interesan (ej. "mujeres de 30-40 que les gusta el yoga").

* **Los Datos (El "Big Data"):** Aquí es donde las "3 V" son obvias:
    * **Volumen:** Petabytes de datos (trillones de posts, likes, fotos, videos).
    * **Velocidad:** Millones de nuevos datos (likes, comentarios, shares) generados por segundo.
    * **Variedad:** Datos estructurados (perfil), no estructurados (fotos, texto) y semi-estructurados (logs de clics).

* **El Resultado Observable (El Producto de "Data Mining"):**
    1.  **El News Feed:** Es un producto de "minería de datos" que predice qué publicaciones te interesarán más.
    2.  **Los Anuncios Segmentados:** El resultado de "minar" los perfiles y comportamientos de miles de millones de usuarios para agruparlos en audiencias vendibles.
    3.  **"Gente que podrías conocer":** Un algoritmo de minería de datos que analiza las redes sociales.

### Conexión con las Herramientas del Módulo
La única forma de lograr esto es con herramientas de Big Data:
* **Cloud:** No se usa una sola supercomputadora, sino un clúster de miles de máquinas baratas. Este conjunto de máquinas es la "nube".
* **HDFS (Hadoop File System):** Es el "disco duro" de la nube. Un sistema de archivos que reparte esos petabytes de datos entre todas las máquinas del clúster.
* **Hadoop (MapReduce) y Spark:** Son los "cerebros" del procesamiento. Permiten ejecutar una tarea (ej: "contar todos los likes de 'hiking'") en todas las miles de máquinas a la vez, en lugar de una por una. **Spark** es la versión moderna y más rápida.
* **Hive:** La herramienta que Meta *inventó* para que sus Data Scientists pudieran usar lenguaje **SQL** (que ya sabían) para lanzar trabajos de **Hadoop/Spark** (que eran muy complejos de programar), haciendo el análisis de Big Data accesible.

---

## Paso 2: Fundamentos Conectados a la Realidad

Aquí documentaré mis notas de cada lección, conectándolas siempre con el caso de Meta.

### 🎥 "How Big Data is Driving Digital Transformation"
* (Tus notas aquí... ¿Qué es la transformación digital? ¿Cómo la impulsan los datos?)
* **Conexión con el Caso Práctico:** (Ej: "Meta transformó la publicidad. Pasó de anuncios en TV para 'todos' a anuncios digitales específicos para 'mí'. Eso es imposible sin Big Data.")

### 🎥 "Introduction to Cloud" / "Cloud for Data Science"
* (Tus notas aquí... ¿Qué es Cloud Computing? ¿Qué es IaaS, PaaS, SaaS? ¿Por qué lo usan los Data Scientists?)
* **Conexión con el Caso Práctico:** (Ej: "Meta no podría tener un edificio con una supercomputadora. Necesita miles de computadoras (un 'cluster') en todo el mundo. Eso es una **Cloud** (aunque sea privada). Un DS en Meta no usa su laptop para entrenar un modelo, pide prestado poder de la 'nube' de Meta.")

### 🎥 "Foundations of Big Data"
* (Tus notas aquí... ¿Cuáles son las '3 V'? Volumen, Velocidad, Variedad)
* **Conexión con el Caso Práctico:**
    * **Volumen (Meta):** Petabytes de fotos, videos y posts.
    * **Velocidad (Meta):** Millones de 'likes', comentarios y mensajes por segundo.
    * **Variedad (Meta):** Texto (posts), imágenes (fotos), video, datos estructurados (tu perfil).

### 🎥 "Big Data Processing Tools: Hadoop, HDFS, Hive, and Spark"
* **Hadoop (MapReduce):** (Definición)
* **HDFS:** (Definición)
* **Hive:** (Definición)
* **Spark:** (Definición)
* **Conexión con el Caso Práctico:** (Ej: "Meta *inventó* **Hive**. Lo necesitaban para que sus analistas, que sabían SQL, pudieran analizar los datos guardados en **HDFS** sin tener que aprender a programar **Hadoop (MapReduce)**. **Spark** es la evolución moderna y rápida de Hadoop.")

### 📖 "Data Mining"
* (Tus notas aquí... ¿Qué es? ¿Cuál es el objetivo? ¿Técnicas?)
* **Conexión con el Caso Práctico:** (Ej: "El **Data Mining** es lo que hace Meta para decidir qué anuncio mostrarme. 'Mina' mis likes, posts y los de mis amigos para clasificarme en un grupo (ej: 'persona interesada en hiking'). Así, las marcas de botas de montaña pueden pagarme para mostrarme su anuncio.")

---

## 🚀 Conclusión del Módulo

(Escribe tu reflexión final aquí cuando termines el módulo).
* **¿Qué funcionó bien?**
* **¿Cuál es la diferencia clave que aprendí entre Hadoop y Spark?**
* **¿Cómo cambió mi entendimiento de 'Cloud'?**
