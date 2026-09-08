# Portafolio de ciencia de datos — Luis Javier Rubio Hernández

Matemático · Magíster en Matemáticas · Estudiante de Maestría en Ciencia de Datos

Cinco análisis reproducibles en Python. Cada cuaderno se abre en Google Colab y se ejecuta de
principio a fin sin descargar nada: los datos se leen desde este mismo repositorio o desde la
fuente pública original.

---

## Cuadernos

| | Cuaderno | Qué demuestra | Datos |
|---|---|---|---|
| 01 | [COVID-19: cuando los datos no podían con la realidad](01_covid19_johns_hopkins.ipynb) | Reestructuración de series acumuladas, auditoría de calidad, concentración con Lorenz y Gini | Johns Hopkins (URL pública) |
| 02 | [¿Qué significa que una máquina aprenda?](02_fundamentos_aprendizaje_automatico.ipynb) | Verificación numérica de fundamentos: riesgo empírico, convergencia del gradiente, sesgo–varianza | Sintéticos con semilla fija |
| 03 | [Segmentación de clientes en marketing directo](03_segmentacion_clientes_marketing.ipynb) | Depuración validada, prueba de Little, imputación múltiple por PMM, contrastes no paramétricos con tamaños del efecto | `datos/campana_marketing_directo.csv` |
| 04 | [4.627 masacres del conflicto armado colombiano](04_masacres_conflicto_armado_colombia.ipynb) | EDA sobre datos abiertos, Kruskal-Wallis, concentración territorial, coocurrencia entre hechos | `datos/masacres_omc_colombia.csv` |
| 05 | [¿Por qué mi canal de YouTube se resiste a morir?](05_canal_youtube_epsilon_delta.ipynb) | Ley de Pareto, CTR ponderado, bootstrap, retención estimada | `datos/youtube_epsilon_delta_videos.csv` |
| 06 | [Alcohol y rendimiento académico](06_alcohol_rendimiento_estudiantil.ipynb) | Faltantes estructurales, contrastes no paramétricos, modelo con control, análisis de potencia | `datos/alcohol_rendimiento_estudiantil.csv` |

## Estructura

```
.
├── README.md
├── 01_covid19_johns_hopkins.ipynb
├── 02_fundamentos_aprendizaje_automatico.ipynb
├── 03_segmentacion_clientes_marketing.ipynb
├── 04_masacres_conflicto_armado_colombia.ipynb
├── 05_canal_youtube_epsilon_delta.ipynb
├── 06_alcohol_rendimiento_estudiantil.ipynb
└── datos/
    ├── alcohol_rendimiento_estudiantil.csv
    ├── campana_marketing_directo.csv
    ├── masacres_omc_colombia.csv
    └── youtube_epsilon_delta_videos.csv
```

## Competencias demostradas

**Preparación y validación.** Reestructuración de formato ancho a largo; diferenciación de series
acumuladas; detección de atípicos por IQR; identificación de inconsistencias de dominio;
validación de la depuración con Kolmogorov-Smirnov y norma de Frobenius entre matrices de
correlación.

**Datos faltantes.** Prueba MCAR de Little implementada con estimación EM; imputación múltiple por
*predictive mean matching* con extracción bayesiana de coeficientes; comparación contra CART y
Ridge por estabilidad entre imputaciones y preservación de correlaciones.

**Inferencia.** Mann-Whitney con correlación rank-biserial; Kruskal-Wallis con épsilon cuadrado;
chi-cuadrado con V de Cramér; Shapiro-Wilk; Spearman; intervalos de confianza por bootstrap;
regresión múltiple con diagnóstico de residuos; análisis de potencia y efecto mínimo detectable
por la transformación z de Fisher. Todos los contrastes se reportan con su tamaño del efecto, no
solo con el valor p.

**Comunicación.** Visualización siguiendo las prácticas de Cole Nussbaumer Knaflic: gris para el
contexto, un solo color de acento para la historia, sin elementos decorativos.

## Reproducibilidad

Los cinco cuadernos están ejecutados: las salidas y figuras visibles en GitHub son las que produce
el código. Toda simulación usa semilla fija. Las celdas de carga intentan primero la URL del
repositorio y recurren a una copia local como respaldo.

Dependencias: `numpy`, `pandas`, `scipy`, `matplotlib`, `seaborn`, `scikit-learn`, `statsmodels`. Todas vienen preinstaladas
en Google Colab.
