# 🧠 Guía Maestra: RStudio, Ciencia de Datos y Control de Versiones (Git/GitHub)

Este documento es una referencia completa diseñada para entender el flujo de trabajo profesional en Ciencia de Datos, desde la manipulación estadística en R hasta la colaboración global en GitHub.

---

## 1. El Entorno de R y RStudio
R es un lenguaje de programación especializado en estadística y visualización. Para trabajarlo de forma eficiente, utilizamos **RStudio**, el IDE (Entorno de Desarrollo Integrado) estándar de la industria.

### Configuración de la Interfaz (Los 4 Paneles)
1. **Source (Editor de Scripts):** Donde escribes y guardas tus archivos `.R`. Es tu "borrador" permanente.
2. **Console (Consola):** El motor de R. Ejecuta comandos inmediatos. Lo que escribes aquí no se guarda al cerrar la sesión.
3. **Environment / History:** Muestra todos los objetos (datasets, variables, funciones) que tienes cargados en la memoria activa.
4. **Files / Plots / Help / Viewer:** Panel multiusos para navegar por carpetas, ver gráficos generados y leer la documentación de las librerías.

---

## 2. Visualización Avanzada: La Gramática de Gráficos (`ggplot2`)
En lugar de funciones aisladas, R utiliza una lógica de capas basada en la **Gramática de Gráficos**.

### La Ecuación del Gráfico
$$Gráfico = Datos + Aesthetics (aes) + Geometries (geom)$$

* **Data:** El dataframe de origen.
* **Aesthetics (`aes`):** Define la relación visual. ¿Qué columna va en el eje $X$? ¿Cuál en el $Y$? ¿Qué columna define el color o el tamaño?
* **Geometries (`geom_`):** La capa física. `geom_point()` para dispersión, `geom_bar()` para barras, `geom_line()` para tendencias.
* **Faceting:** Permite crear sub-gráficos automáticos basados en una variable categórica usando `facet_wrap()`.

---

## 3. Conexión Profesional: RStudio + GitHub
Para trabajar de forma segura sin introducir contraseñas constantemente, se utiliza un **PAT (Personal Access Token)**.

### Pasos de Configuración:
1. **Instalar herramientas:** `install.packages(c("usethis", "gitcreds"))`
2. **Generar Token:** Ejecutar `usethis::create_github_token()`. Se abrirá GitHub; genera el token y **cópialo**.
3. **Vincular Credenciales:** Ejecutar `gitcreds::gitcreds_set()` y pegar el token cuando se solicite.
4. **Verificación:** Tras reiniciar RStudio, aparecerá la pestaña **Git** en el panel superior derecho.

---

## 4. Fundamentos de Git: El Ciclo de Vida del Código
Git es un sistema de control de versiones **distribuido**. No guarda archivos nuevos cada vez, sino "snapshots" (fotos) de los cambios.

### Flujo de Trabajo Local
1. **Working Directory:** Archivos en los que estás trabajando actualmente.
2. **Staging Area (`git add`):** El "limbo". Aquí seleccionas qué cambios están listos para ser guardados.
3. **Local Repository (`git commit`):** Se crea una versión en tu historial local con un mensaje descriptivo.

### Sincronización Remota (GitHub)
* **Push:** Empujar tus cambios locales al servidor de GitHub.
* **Pull:** Traer los cambios que otros han hecho en la nube a tu computadora.
* **Clone:** Descargar un repositorio completo por primera vez.

---

## 5. Estrategia de Ramas (Branching) y Colaboración
Trabajar en equipo requiere que el código principal nunca se rompa.

* **Main Branch (Rama Principal):** Contiene el código estable y listo para producción. **No se recomienda trabajar directamente aquí.**
* **Child Branch (Rama Secundaria):** Ramas creadas para desarrollar una nueva función o corregir un error (*Feature branches*).
* **Pull Request (PR):** Es una solicitud para fusionar (Merge) una rama secundaria con la principal. Permite la revisión de código por parte de pares.

---

## 6. Resolución de Conflictos (Merge Conflicts)
Un conflicto ocurre cuando dos fuentes modifican la **misma línea** de código y Git no sabe cuál elegir.

**Cómo resolverlo:**
1. Git marcará el archivo conflictivo con etiquetas:
   - `<<<<<<< HEAD`: Tu versión local.
   - `=======`: Separador.
   - `>>>>>>> [ID_del_commit]`: La versión que viene de fuera.
2. Debes editar el archivo manualmente, borrar las etiquetas y dejar el código final deseado.
3. Realiza un nuevo `Add`, `Commit` y `Push` para cerrar el conflicto.

---

## 📚 Glosario de Comandos Esenciales

| Comando | Acción |
| :--- | :--- |
| `git status` | Revisa qué archivos han cambiado. |
| `git log` | Mira el historial de versiones (commits). |
| `git checkout -b [nombre]` | Crea una nueva rama y se mueve a ella. |
| `git merge [rama]` | Combina una rama con la actual. |
| `install.packages()` | Instala librerías desde CRAN en R. |
