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
La transformación digital afecta a las operaciones comerciales, actualizando los procesos y operaciones existentes y creando otros nuevos para aprovechar los beneficios de las nuevas tecnologías. La transformación digital no consiste simplemente en duplicar los procesos existentes en formato digital; el análisis en profundidad del funcionamiento de la empresa ayuda a las organizaciones a descubrir cómo mejorar sus procesos y operaciones, y a aprovechar las ventajas de integrar la ciencia de datos en sus flujos de trabajo. No cabe duda de que abordar todos los problemas que surgen en este esfuerzo requiere una nueva mentalidad, pero la transformación digital es la forma de tener éxito ahora y en el futuro. 
* **Conexión con el Caso Práctico:**
En 2018, los Rockets de Houston, un equipo de la NBA, elevaron su nivel de juego con el uso del big data. Los Rockets fueron uno de los cuatro equipos de la NBA que instalaron un sistema de seguimiento por vídeo que extraía datos sin procesar de los partidos. Analizaron los datos de seguimiento de vídeo para investigar qué jugadas ofrecían las mejores oportunidades de conseguir puntuaciones altas y descubrieron algo sorprendente. El análisis de los datos reveló que los tiros que ofrecen las mejores oportunidades de conseguir puntuaciones altas son los mates de dos puntos desde dentro de la zona de dos puntos y los tiros de tres puntos desde fuera de la línea de tres puntos, no los tiros de dos puntos a larga distancia desde dentro de la misma. Este descubrimiento cambió por completo la forma en que el equipo abordaba cada partido, aumentando el número de intentos de tiros de tres puntos. En la temporada 2017-18, los Rockets encestaron más tiros de tres puntos que ningún otro equipo en la historia de la NBA, y esta fue una de las principales razones por las que ganaron más partidos que cualquiera de sus rivales.

### 🎥 "Introduction to Cloud" / "Cloud for Data Science"
¿Qué es Cloud Computing? 
Es la entrega de recursos commputacionales bajo demanda, como redes, servidores, almacenamiento, aplicaciones, servicios, centros de datos, todo sobre internet y bajo un sistema de pago por uso. A Cloud Computing se accede mediante internet en vez de localmente. 

La computación en la nube se compone de cinco características esenciales, tres modelos de implementación y tres modelos de servicio. La computación en la nube se compone de cinco características esenciales, tres modelos de implementación y tres modelos de servicio.

Las 5 caracteristicas esenciales son: 
- On-demand self-service: Se puede acceder a los recursos de la nube mediante una interfaz sencilla sin necesidad de   interacción humana con cada proveedor de servicios.
- Broad network access: El amplio acceso a la red significa que a través de la red se pueden acceder a los recursos de cloud computing en teléfonos móviles, tabletas, computadoras y estaciones de trabajo.
- Resource pooling: La agrupación de recursos es lo que le da a los proveedores de la nube economía de escala, haciendo que la nube sea rentable. Al utilizar un modelo multiusuario, los recursos informáticos se agrupan para atender a varios consumidores, y los recursos en la nube se asignan y reasignan dinámicamente según la demanda, sin que los clientes necesiten saber la ubicación física de estos recursos. El "resource pooling" es como un gran depósito de recursos que se comparte entre diferentes usuarios. Imagina que tienes un grupo de amigos y todos deciden usar una piscina comunitaria. En lugar de que cada uno tenga su propia piscina en casa, todos pueden disfrutar de la misma piscina cuando lo deseen. De esta manera, se aprovechan mejor los recursos y se reduce el costo para cada uno. En el contexto de la computación en la nube, los proveedores agrupan recursos como servidores, almacenamiento y redes para servir a múltiples clientes al mismo tiempo. Esto permite que los costos sean más bajos y que los recursos se utilicen de manera más eficiente.
- Rapid elasticity: Implica que puede acceder a más recursos cuando los necesita y reducirlos cuando no los necesita, ya que los recursos se aprovisionan y liberan de forma elástica.
- Measured service: Significa que solo paga por lo que usa o reserva sobre la marcha. Si no utilizas los recursos, no pagas.

Los 3 modelos de implementación de la nube indican donde reside la infraestructura, a quién le pertenece, quien la maneja y cómo se ponen a disposición de los usuarios los recursos y servicios de la nube y son: 
- Públicos: Es cuando tú aprovechas los servicios de la nube a través de internet abierto en hardware propiedad del proveedor de la nube, pero otras empresas comparten su uso. 
- Privados: La infraestructura de la nube se aprovisiona para el uso exclusivo de una sola organización. Puede funcionar de forma local o puede ser propiedad de un proveedor de servicios, gestionado y operado por él. 
- Híbridos: Es cuando se utikiza una combinación de nubes públicas y privadas que funcionan juntas sin problemas.

Los 3 modelos de servicio se basan en las 3 capas de un conjunto de computación: Infraestructura, Plataforma y Aplicación, y son los siguientes: 

- Iaas (infraestructura como servicio): En un modelo de IaaS, puede acceder a la infraestructura y a los recursos informáticos físicos, como los servidores, las redes, el almacenamiento y el espacio del centro de datos, sin necesidad de administrarlos ni operarlos. Think of this as renting a fully equipped workshop. You get access to all the tools and machines (like servers and storage) you need to build your projects, but you don’t have to worry about maintaining the workshop itself. You can use the resources as you need them and pay only for what you use.
- PaaS (plataforma como servicio): En un modelo PaaS, puede acceder a la plataforma que incluye las herramientas de hardware y software que normalmente se necesitan para desarrollar e implementar aplicaciones para los usuarios a través de Internet. This is like renting a space in a bakery where you can bake your cakes. The bakery provides the ovens, ingredients, and tools, so you can focus on creating delicious treats without worrying about the setup. In PaaS, you get the tools and environment to develop and deploy applications without managing the underlying infrastructure.
- SaaS (software como servicio): SaaS es un modelo de licencia y entrega de software en el que el software y las aplicaciones se alojan de forma centralizada y se licencian mediante suscripción. Imagine subscribing to a streaming service like Netflix. You can watch movies and shows without needing to download or install anything on your device. SaaS works the same way; you access software applications over the Internet, usually through a subscription, without needing to install them on your computer.

Diferencias: 
- IaaS: Control total sobre la infraestructura, ideal para empresas que necesitan personalización.
- PaaS: Enfoque en el desarrollo de aplicaciones, sin preocuparse por la infraestructura.
- SaaS: Acceso a aplicaciones listas para usar, sin necesidad de instalación.

La nube es una "bendición" para los data scientist ya que pueden almacenar ahí no solo grandes conjuntos de datos sino también los algoritmos que usarán para trabajar dichos conjuntos de datos. La nube èrmite que varias entidades de trabajo, trabajen con los mismos datos, al mismo tiempo, por ejemplo, colegas de Alemania, India y Ghana pueden trabajar de forma colectiva ya que la información, algoritmos, herramientas, respuestas, resultados y todo lo qye necesiten, están disponibles en un lugar central (nube) y también esta permite acceso instantáneo a las tecnologías. 


### 🎥 "Foundations of Big Data"

Los macrodatos (big data) se refieren a los volúmenes de datos dinámicos, grandes y dispares que crean las personas, las herramientas y las máquinas. Requiere una tecnología nueva, innovadora y escalable para recopilar, alojar y procesar analíticamente la gran cantidad de datos recopilados a fin de obtener información empresarial en tiempo real relacionada con los consumidores, el riesgo, las ganancias, el rendimiento, la gestión de la productividad y el aumento del valor para los accionistas. Las características que tienen en común todas las definiciones de big data son the V´s of Big Data: 
- Velocity -> The speed at which data accumulates. 
- Volume -> The scale of the data. Sus drivers son:
        - Aumento en las fuentes de datos.
        - Sensores de mayor resolución.
        - Infraestructura escalable.
- Variety -> Diversity of the data and also reflects that data comes from different sources. 
- Veracity -> Is the quality and origin of data and its conformity to facts and accuracy. Se considera que el 80% de los datos son no estructurados, por lo que debemos idear formas de generar informacion fiable y precisa. Sus drivers son: 
        - Costos asociados. A medida que se recopilan y almacenan grandes volúmenes de datos, los costos de asegurar         la calidad y la precisión de esos datos pueden aumentar. Las organizaciones deben invertir en herramientas y         procesos para verificar la veracidad de la información.
        - Necesidad de trazabilidad. Esto implica la capacidad de rastrear el origen de los datos y cómo han sido             manipulados a lo largo del tiempo. La trazabilidad es crucial para garantizar que los datos sean precisos y          confiables, especialmente en entornos donde las decisiones se basan en esos datos.
- Value -> Our ability and need to turn data into value. Value is not just profit, also is social benefit. 

Tools such as Apache Spark, Hadoop and its ecosystem provide ways to extract, load, analyze and process the data across distributed compute resources. 

Una de las ventajas de los clusters de Big Data es que son escalables linealmente, es decir, si tu tienes el doble de servidores, tienes el doble de rendimiento. 

Procesos para manejar grandes cantidades de datos de manera eficiente:
      - Map or Mapper Process: Imagina que tienes un gran libro y quieres contar cuántas veces aparece cada palabra. En el proceso Map, divides el libro en varias páginas y le das una página a cada amigo. Cada amigo cuenta las palabras en su página y anota cuántas veces aparece cada una. Así, en lugar de contar todas las palabras de una vez, cada amigo trabaja en su parte y envía sus resultados.
      - Reduce process: Ahora que todos tus amigos han contado las palabras en sus páginas, es hora de juntar toda esa información. En el proceso Reduce, tú tomas las cuentas de cada amigo y las sumas. Por ejemplo, si un amigo contó "gato" 3 veces y otro amigo 5 veces, tú sumas esos números y obtienes que "gato" aparece 8 veces en total. Este proceso organiza y simplifica los resultados para que puedas ver el total de cada palabra en el libro.

* **Conexión con el Caso Práctico:**
    * **Volumen (Meta):** Petabytes de fotos, videos y posts.
    * **Velocidad (Meta):** Millones de 'likes', comentarios y mensajes por segundo.
    * **Variedad (Meta):** Texto (posts), imágenes (fotos), video, datos estructurados (tu perfil).

### 🎥 "Big Data Processing Tools: Hadoop, HDFS, Hive, and Spark"
Estas herramientas proveen de formas de trabajar con grandes conjuntos de datos estructurados, semi estructurados y no estructurados para aprovechar el valor de big data. 

* **Apache Hadoop**

Distributed Storage and Processing: Hadoop allows for the storage and processing of large datasets across clusters of computers, providing a reliable and scalable solution.
Hadoop Distributed File System (HDFS): HDFS partitions files across multiple nodes, enabling parallel access and fault tolerance through data replication. Uso: Ideal para almacenar y procesar grandes volúmenes de datos de manera distribuida.

* **Apache Hive**

Data Warehousing: Hive is designed for reading, writing, and managing large datasets stored in HDFS, using SQL-like queries for data analysis.
High Latency: While suitable for ETL and reporting tasks, Hive is less appropriate for applications requiring fast response times due to its read-based nature. Uso: Mejor para tareas de análisis de datos y generación de informes, no para procesamiento en tiempo real.

* **Apache Spark**

Real-Time Data Processing: Spark is a general-purpose data processing engine that excels in real-time analytics and complex data processing.
In-Memory Processing: It significantly speeds up computations by processing data in memory and supports various programming languages, making it versatile for different applications. Uso: Ideal para análisis en tiempo real, procesamiento de flujos de datos y machine learning.


### 📖 "Data Mining"
El primer paso en la extracción de datos requiere que se establezcan metas par el ejercicio. Obviamente, debes identificar las preguntas clave que necesitan ser respondidas. Además de tener en cuenta los costos y beneficios del ejercicio, debes determinar por adelantado el nivel esperado de exactitud y utilidad de los resultados obtenidos de la extracción de datos. 
    - Selecting Data 
    - Preprocessing Data
    - Transforming Data
    - Storing Data
    - Mining Data
    - Evaluating Mining Results 
* **Conexión con el Caso Práctico:** (Ej: "El **Data Mining** es lo que hace Meta para decidir qué anuncio mostrarme. 'Mina' mis likes, posts y los de mis amigos para clasificarme en un grupo (ej: 'persona interesada en hiking'). Así, las marcas de botas de montaña pueden pagarme para mostrarme su anuncio.")

---

## Glosario del Módulo: Big Data y Data Mining

¡Bienvenido! Este glosario contiene muchos de los términos de esta lección. Es importante que reconozcas estos términos cuando trabajes en la industria, participes en grupos de usuarios y en otros programas de certificación.

| Term | Definition | Video where the term is introduced |
| --- | --- | --- |
| Analytics | The process of examining data to draw conclusions and make informed decisions is a fundamental aspect of data science, involving statistical analysis and data-driven insights. | Data Scientists at New York University |
| Big Data | Vast amounts of structured, semi-structured, and unstructured data are characterized by its volume, velocity, variety, veracity and value, which, when analyzed, can provide competitive advantages and drive digital transformations. | How Big Data is Driving Digital Transformation |
| Big Data Cluster | A distributed computing environment comprising thousands or tens of thousands of interconnected computers that collectively store and process large datasets. | What is Hadoop? |
| Broad Network Access | The ability to access cloud resources via standard mechanisms and platforms such as mobile devices, laptops, and workstations over networks. | Introduction to Cloud |
| Chief Data Officer (CDO) | An emerging role responsible for overseeing data-related initiatives, governance, and strategies, ensuring that data plays a central role in digital transformation efforts. | How Big Data is Driving Digital Transformation |
| Chief Information Officer (CIO) | An executive is responsible for managing an organization's information technology and computer systems, contributing to technology-related aspects of digital transformation. | How Big Data is Driving Digital Transformation |
| Cloud Computing | The delivery of on-demand computing resources, including networks, servers, storage, applications, services, and data centers, over the Internet on a pay-for-use basis. | Introduction to Cloud |
| Cloud Deployment Models | Categories that indicate where cloud infrastructure resides, who manages it, and how cloud resources and services are made available to users, including public, private, and hybrid models. | Introduction to Cloud |
| Cloud Service Models | Models based on the layers of a computing stack, including Infrastructure as a Service (IaaS), Platform as a Service (PaaS), and Software as a Service (SaaS), represent different cloud computing offerings. | Introduction to Cloud |
| Commodity Hardware | Standard, off-the-shelf hardware components are used in a big data cluster, offering cost-effective solutions for storage and processing without relying on specialized hardware. | What is Hadoop? |
| Data Algorithms | Computational procedures and mathematical models used to process and analyze data made accessible in the cloud for data scientists to deploy on large datasets efficiently. | Cloud for Data Science |
| Data Replication | A strategy in in which data is duplicated across multiple nodes in a cluster to ensure data durability and availability, reducing the risk of data loss due to hardware failures. | What is Hadoop? |
| Data Science | An interdisciplinary field that involves extracting insights and knowledge from data using various techniques, including programming, statistics, and analytical tools. | Data Scientists at New York University |
| Deep Learning | A subset of machine learning that involves artificial neural networks inspired by the human brain, capable of learning and making complex decisions from data on their own. | Data Scientists at New York University |
| Digital Change | The integration of digital technology into business processes and operations leads to improvements and innovations in how organizations operate and deliver value to customers. | How Big Data is Driving Digital Transformation |
| Digital Transformation | A strategic and cultural organizational change driven by data science, especially Big Data, to integrate digital technology across all areas of the organization, resulting in fundamental operational and value delivery changes. | How Big Data is Driving Digital Transformation |
| Distributed Data | The practice of dividing data into smaller chunks and distributing them across multiple computers within a cluster enables parallel processing for data analysis. | What is Hadoop? |
| Hadoop | A distributed storage and processing framework used for handling and analyzing large datasets, particularly well-suited for big data analytics and data science applications. | Data Scientists at New York University |
| Hadoop Distributed File System (HDFS) | A storage system within the Hadoop framework that partitions and distributes files across multiple nodes, facilitating parallel data access and fault tolerance. | What is Hadoop? |
| Infrastructure as a Service (IaaS) | A cloud service model that provides access to computing infrastructure, including servers, storage, and networking, without the need for users to manage or operate them. | Introduction to Cloud |
| Java-Based Framework | Hadoop is implemented in Java, an open-source, high-level programming language, providing the foundation for building distributed storage and processing solutions. | Big Data Processing Tools: Hadoop, HDFS, Hive, and Spark |
| Map Process | The initial step in Hadoop's MapReduce programming model, where data is processed in parallel on individual cluster nodes, often used for data transformation tasks. | What is Hadoop? |
| Measured Service | A characteristic where users are billed for cloud resources based on their actual usage, with resource utilization transparently monitored, measured, and reported. | Introduction to Cloud |
| On-Demand Self-Service | The capability for users to access and provision cloud resources such as processing power, storage, and networking using simple interfaces without human interaction with service providers. | Introduction to Cloud |
| Rapid Elasticity | The ability to quickly scale cloud resources up or down based on demand, allowing users to access more resources when needed and release them when not in use. | Introduction to Cloud |
| Reduce Process | The second step in Hadoop's MapReduce model is where results from the mapping process are aggregated and processed further to produce the final output, typically used for analysis. | What is Hadoop? |
| Replication | The act of creating copies of data pieces within a big data cluster enhances fault tolerance and ensures data availability in case of hardware or node failures. | What is Hadoop? |
| Resource Pooling | A cloud characteristic where computing resources are shared and dynamically assigned to multiple consumers, promoting economies of scale and cost-efficiency. | Introduction to Cloud |
| Skills Network Labs (SN Labs) | Learning resources provided by IBM, including tools like Jupyter Notebooks and Spark clusters, are available to learners for cloud data science projects and skill development. | Cloud for Data Science |
| Spilling to Disk | A technique used in memory-constrained situations where data is temporarily written to disk storage when memory resources are exhausted, ensuring uninterrupted processing. | Big Data Processing Tools: Hadoop, HDFS, Hive, and Spark |
| STEM Classes | Science, Technology, Engineering, and Mathematics (STEM) courses typically taught in high schools prepare students for technical careers, including data science. | Data Scientists at New York University |
| Variety | The diversity of data types, including structured and unstructured data from various sources such as text, images, video, and more, posing data management challenges. | Foundations of Big Data |
| Velocity | The speed at which data accumulates and is generated, often in real-time or near-real-time, drives the need for rapid data processing and analytics. | Foundations of Big Data |
| Veracity | The quality and accuracy of data, ensuring that it conforms to facts and is consistent, complete, and free from ambiguity, impacts data reliability and trustworthiness. | Foundations of Big Data |
| Video Tracking System | A system used to capture and analyze video data from games, enabling in-depth analysis of player movements and game dynamics, contributing to data-driven decision-making in sports. | How Big Data is Driving Digital Transformation |
| Volume | The scale of data generated and stored is driven by increased data sources, higher-resolution sensors, and scalable infrastructure. | Foundations of Big Data |
| V's of Big Data | A set of characteristics common across Big Data definitions, including Velocity, Volume, Variety, Veracity, and Value, highlighting the rapid generation, scale, diversity, quality, and value of data. | Foundations of Big Data |

---

## 🚀 Conclusión del Módulo

(Escribe tu reflexión final aquí cuando termines el módulo).
* **¿Qué funcionó bien?**
* **¿Cuál es la diferencia clave que aprendí entre Hadoop y Spark?**
* **¿Cómo cambió mi entendimiento de 'Cloud'?**
