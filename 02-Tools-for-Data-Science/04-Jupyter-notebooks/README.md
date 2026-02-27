# 📔 GUÍA MAESTRA: ECOSISTEMA JUPYTER (Notebooks, Lab & Architecture)

## 📑 1. ¿QUÉ ES UN JUPYTER NOTEBOOK?
El nombre **Jupyter** es un acrónimo de los tres lenguajes de programación originales para los que fue diseñado: **JU**lia, **PY**thon y **R**. Actualmente, es un estándar agnóstico que soporta más de 40 lenguajes (incluyendo C++, Java, Scala y Ruby) mediante el uso de diferentes **kernels**.

### 🔬 El Concepto del Científico de Datos
Un Jupyter Notebook es como un cuaderno para científicos, donde un investigador registra todos los pasos para realizar sus experimentos y los resultados que puede reproducir. De la misma forma, permite a los *Data Scientists* registrar sus experimentos de datos y resultados que otros pueden reutilizar.



### 🛠️ Características Principales
* **Combinación de contenido:** Permite combinar texto enriquecido, bloques de código y la salida (*output*) del código en un solo archivo.
* **Visualización integrada:** Al correr el código, se generan gráficos y tablas inmediatamente debajo de la celda en el mismo archivo.
* **Portabilidad:** Puedes exportar el Notebook a PDF o HTML para compartirlo con cualquier persona.
* **Nube:** Se pueden usar en servicios basados en la nube como **IBM Watson Studio** y **Google Colab**, sin necesidad de instalación local.

---

## 🚀 2. JUPYTERLAB: EL ENTORNO PROFESIONAL
**JupyterLab** es la interfaz de próxima generación para Project Jupyter. Es *Open Source* y mucho más flexible que el Notebook clásico.

### 🌟 Funcionalidades de JupyterLab
* **Multitarea:** Permite acceder a múltiples archivos de Notebook, otros códigos y archivos de datos simultáneamente.
* **Integración:** Incluye editores de texto, terminales y componentes personalizados.
* **Compatibilidad:** Soporta formatos como CSV, JSON, PDF, Vega, entre otros.

**Instalación:**
* Vía terminal: `$ pip install jupyterlab`
* Vía **Anaconda** (instalación local recomendada).

---

## 🏗️ 3. ARQUITECTURA TÉCNICA DE JUPYTER
Jupyter implementa un modelo de dos procesos: **Kernel** y **Cliente**.



### 🧩 Componentes del Sistema
1.  **El Cliente:** Es la interfaz web donde el usuario manda código al kernel.
2.  **El Kernel (Motor Computacional):** Es el responsable de ejecutar el código contenido en el Notebook.
    * Existe un kernel para cada lenguaje.
    * Al abrir un documento, el kernel asociado se lanza automáticamente.
    * Actúa como un puente entre el código y la computadora.
    * *Nota:* Si corres el kernel localmente, debes instalar los lenguajes manualmente vía línea de comandos.
3.  **Notebook Server:** Es el encargado de guardar y cargar los notebooks.
4.  **Formato de Archivo:** Al guardar, el archivo se envía del buscador al servidor y se almacena como un archivo **JSON** con extensión `.ipynb`.
5.  **NBConvert:** Herramienta que convierte los archivos `.ipynb` a otros formatos (PDF, HTML, etc.).

---

## ✍️ 4. DOMINANDO EL FORMATO MARKDOWN
Markdown permite dar estructura y estilo al texto de tus celdas de documentación.

### 🖋️ Estilos de Texto
* **Negrita:** `**texto**` o `__texto__`
* *Itálica:* `*texto*` o `_texto_`
* ***Negrita + Itálica:*** `***texto***` o `___texto___`

### 📏 Estructura y Multimedia
* **Títulos:** 6 niveles, desde `# Heading 1` (Mayor) hasta `###### Heading 6` (Menor).
* **Hipervínculos:** `[Nombre del link](URL)`
* **Imágenes:** `![alt text](PATH_O_URL)`
* **Listas:**
    * No ordenadas: `-`, `*` o `+` antes del ítem.
    * Ordenadas: `1.` antes del ítem.

### 📊 Tablas
```markdown
| Encabezado 1 | Encabezado 2 |
| ------------ | ------------ |
| Fila 1       | Dato A       |
| Fila 2       | Dato B       |
