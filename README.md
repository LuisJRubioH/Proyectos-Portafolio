# Proyectos-Portafolio

**Matemáticas, análisis de datos y aprendizaje automático: comprender, aplicar y comunicar.**

Soy **Luis Javier Rubio Hernández**, matemático, magíster en Matemáticas y docente universitario. Actualmente curso la **Maestría en Ciencia de Datos en la Pontificia Universidad Javeriana Cali**. Este repositorio reúne proyectos, análisis y notas de estudio con los que documento mi formación y construyo mi portafolio en ciencia de datos.

Aquí conecto mi formación matemática con preguntas sobre salud pública, educación, comportamiento de clientes y realidad social. Me interesa comprender qué hace un método, bajo qué supuestos funciona y hasta dónde permite interpretar los resultados.

## Filosofía del repositorio

**Aprender haciendo y explicar lo aprendido con fundamento.** Cada proyecto es una oportunidad para formular preguntas, examinar los datos, justificar decisiones y comunicar conclusiones que puedan contrastarse con el trabajo realizado.

El repositorio se guía por estos principios:

- **Rigor matemático y estadístico.** Explicitar definiciones, supuestos y limitaciones; distinguir una demostración de una comprobación numérica y una asociación de una relación causal.
- **Lectura crítica de los datos.** Revisar su procedencia, estructura y calidad antes de interpretar cifras. Un registro describe lo documentado por una fuente, con sus alcances y omisiones.
- **Trazabilidad y reproducibilidad.** Documentar cómo se pasa de los datos a los resultados, incluyendo transformaciones, dependencias y decisiones metodológicas.
- **Comunicación clara.** Acompañar el código y las fórmulas con explicaciones comprensibles. Las visualizaciones deben ayudar a responder preguntas y conservar el contexto de los resultados.
- **Aprendizaje continuo.** Revisar los análisis a medida que avanzo en mi formación, corregir errores y hacer explícitos los aspectos pendientes.

En temas sociales, el análisis exige además reconocer a las personas y comunidades detrás de los registros y tratar las conclusiones con la responsabilidad que ese contexto requiere.

## Del análisis a LinkedIn

Los **notebooks** documentan el desarrollo técnico: preparación de datos, exploración, cálculos, simulaciones y visualizaciones. Los **PDF** son materiales que utilizo como base o acompañamiento de mis publicaciones en **LinkedIn**, para compartir hallazgos, explicar conceptos y reflexionar sobre lo aprendido durante la maestría.

Ambos formatos se complementan: el PDF facilita la lectura y la divulgación; el notebook permite examinar el procedimiento que respalda el contenido. Algunos documentos son notas conceptuales y otros presentan análisis aplicados. Cuando existen versiones en distintos lenguajes, conviene consultar sus decisiones de implementación antes de comparar resultados.

## Contenido

| Tema | Pregunta o enfoque | Material disponible |
| --- | --- | --- |
| COVID-19 — Johns Hopkins | Cómo interpretar series acumuladas, construir agregaciones temporales y reconocer las limitaciones de los datos reportados. | Notebook `01` y PDF. |
| Fundamentos del aprendizaje automático | Qué significa aprender: riesgo, función de costo, optimización y evaluación, con ejemplos y simulaciones. | Notebook `02` y PDF. |
| Segmentación de clientes en marketing directo | Preparación de datos, tratamiento de faltantes y caracterización de perfiles según la respuesta a una campaña. | Notebook `03` en Python y PDF del análisis desarrollado en R. |
| Masacres del conflicto armado colombiano | Exploración temporal, territorial y por presuntos responsables, considerando los límites del registro. | Notebook `04` y PDF. |
| Canal de YouTube de matemáticas | Análisis del desempeño del canal y reflexión sobre el alcance de los contenidos educativos. | PDF; notebook por incorporar. |

## Estructura propuesta

Esta es la organización prevista para el repositorio. Las rutas siguientes sirven como guía de reorganización; las carpetas y los archivos pendientes se incorporarán progresivamente.

| Ruta desde la raíz | Contenido y función |
| --- | --- |
| `README.md` | Presentación, filosofía y guía del portafolio. |
| `LICENSE` | Licencia del repositorio. |
| `.gitignore` | Exclusión de entornos locales, archivos temporales y datos que no deban publicarse. |
| `requirements.txt` | Dependencias de Python con las versiones utilizadas, una vez verificadas. |
| `notebooks/` | Cuadernos de análisis y experimentación. |
| `data/README.md` | Fuentes, fechas de descarga, diccionario de variables e instrucciones de acceso a los datos. |
| `data/raw/` | Archivos originales, conservados sin modificaciones, cuando se permita su redistribución. |
| `data/processed/` | Datos derivados de la preparación y limpieza. |
| `docs/linkedin/` | PDF utilizados para las publicaciones en LinkedIn. |
| `docs/linkedin/README.md` | Índice que relaciona cada PDF con su notebook y, cuando esté disponible, su publicación. |
| `assets/figures/` | Gráficos exportados para documentos y publicaciones. |
| `assets/images/` | Imágenes, diagramas y otros recursos de apoyo. |
| `projects/` | Proyectos autónomos con varios archivos o una estructura propia. Cada uno tendrá su README. |
| `src/` | Funciones reutilizables cuando varios notebooks compartan código. Se añadirá cuando sea necesario. |

### Nombres de los notebooks

Conservar los nombres actuales permite mantener una secuencia clara:

```text
notebooks/01_covid19_johns_hopkins.ipynb
notebooks/02_fundamentos_aprendizaje_automatico.ipynb
notebooks/03_segmentacion_clientes_marketing.ipynb
notebooks/04_masacres_conflicto_armado_colombia.ipynb
```

Para el análisis del canal, el nombre previsto es `notebooks/05_analisis_canal_youtube.ipynb`, cuando se incorpore el cuaderno.

### Organización de los PDF

Se propone renombrarlos con el mismo identificador del notebook asociado. El título editorial puede conservarse dentro del documento.

| Documento actual | Ruta propuesta |
| --- | --- |
| Cuando los datos no podían.pdf | `docs/linkedin/01_covid19_johns_hopkins.pdf` |
| ¿Qué significa, exactamente,.pdf | `docs/linkedin/02_fundamentos_aprendizaje_automatico.pdf` |
| Segmentación de clientes.pdf | `docs/linkedin/03_segmentacion_clientes_marketing.pdf` |
| 4,627 masacres lo que los datos revelan.pdf | `docs/linkedin/04_masacres_conflicto_armado_colombia.pdf` |
| ¿Por qué mi canal de YouTube.pdf | `docs/linkedin/05_analisis_canal_youtube.pdf` |

Los proyectos independientes, como el de consumo de alcohol y desempeño estudiantil, pueden ubicarse en `projects/alcohol_student_performance/`, conservando su organización interna. El diagrama `ERD Practice.png` puede trasladarse a `assets/images/erd_practice.png`.

## Cómo consultar y reproducir el trabajo

Para conocer un tema, comienza por su PDF. Para revisar el método y los cálculos, consulta el notebook correspondiente.

Para ejecutar un cuaderno:

1. Revisa su introducción, las fuentes y las dependencias importadas.
2. Obtén los datos siguiendo la documentación y respeta sus condiciones de uso.
3. Ajusta las rutas a la estructura adoptada. Algunos cuadernos todavía contienen referencias `USUARIO/REPO`, rutas `datos/` o cargas desde archivos situados junto al notebook.
4. Abre el cuaderno en Jupyter o Google Colab, selecciona el entorno adecuado y ejecuta las celdas en orden desde un kernel limpio.

La reorganización deberá acompañarse de la actualización de las rutas y los enlaces de Colab. La reproducción de resultados depende también de la versión de los datos, las bibliotecas y, cuando corresponda, las semillas aleatorias.

## Herramientas

Los cuadernos compartidos utilizan **Python**, con bibliotecas como **pandas, NumPy, Matplotlib, SciPy y scikit-learn**. Parte del trabajo de análisis también se desarrolla en **R**, con herramientas como **bookdown** y **mice**. Cada proyecto debe indicar cuáles necesita realmente.

## Fuentes y uso del material

Las fuentes de datos y las referencias metodológicas se documentan en los materiales de cada proyecto. Para reutilizar el contenido, consulta `LICENSE`; los datos de terceros conservan sus propias condiciones de uso.

Este portafolio está en construcción y refleja mi proceso de aprendizaje. Las observaciones técnicas y las correcciones fundamentadas son bienvenidas a través de los issues del repositorio.

**Luis Javier Rubio Hernández**  
Matemático · Magíster en Matemáticas · Docente universitario · Estudiante de Maestría en Ciencia de Datos
