# Introducción al Análisis de Datos — UTN FRA

Apuntes y material de la cursada de **Introducción al Análisis de Datos** (Tecnicatura Universitaria en Programación, UTN Facultad Regional Avellaneda), 2do. cuatrimestre 2026. Profesor: Fernández, Luis Nahuel.

## Funcionamiento de la materia

[![Ver PDF](https://img.shields.io/badge/PDF-Funcionamiento%20de%20la%20materia-blue?logo=adobeacrobatreader)](Material/0%20-%20Funcionamiento.pdf)

- **Modalidad:** clases con código en Python y R (libre elección de lenguaje/IDE, no se evalúa código). El código de clase se comparte por Google Colab.
- **Asistencia:** se exige 75% (máximo 3 faltas en el cuatrimestre).
- **Regularidad:** 4 o más en ambos parciales.
- **Aprobación:** 6 o más en ambos parciales, o final en caso de no lograrlo.

### Exámenes
| Instancia | Fecha | Tipo |
|---|---|---|
| Primer parcial | 2/10 | Teórico y virtual |
| Recuperatorio 1er parcial | 16/10 | — |
| Segundo parcial (TP final) | — | Informe usando bases de la Encuesta Permanente de Hogares (INDEC) |
| Defensa TP final | 27/11 | — |
| Recuperatorio TP final | 4/12 | — |
| Finales / última instancia recuperatorio | 11/12 | Examen integrador (nota máx. 4) para quienes no regularizaron |

### Cronograma de clases
| Clase | Tema |
|---|---|
| 21/8 | Conceptos básicos |
| 28/8 | Numpy |
| 4/9 | Pandas |
| 11/9 | Data cleaning |
| 18/9 | Análisis exploratorio de datos y estadística descriptiva |
| 25/9 | Visualización de datos |
| 2/10 | Primer parcial teórico |
| 9/10 | Análisis de datos con R |
| 16/10 | Recuperatorio primer parcial |
| 23/10 | Integración de fuentes / SQL con pandas / Cassandra |
| 30/10 | Conceptos básicos del modelado de datos |
| 6/11 | Modelos de clasificación |
| 13/11 | Modelos de regresión |
| 20/11 | Modelos de clustering |
| 27/11 | Defensa TP final |
| 4/12 | Recuperatorio TP final |
| 11/12 | Instancia de finales y última instancia de recuperatorio |

### Bibliografía
**Obligatoria**
- Chan, D., Badano, C., Rey, A. (2019). *Análisis inteligente de datos con lenguaje R* (pp. 1-73). edUTecNe. — se ven los dos primeros capítulos (introducción a la minería de datos e introducción al análisis de datos).
- McKinney, W. (2023). *Python para análisis de datos*. Ediciones Anaya Multimedia. (Trabajo original 2022) — el autor es el creador de la librería Pandas; se usa más como referencia práctica de Python que conceptual.

**Optativa**
- Mitchell, T. (1997). *Machine Learning*. McGraw Hill.
- Szretter Noste, M. E. (2017). *Apunte de regresión lineal*. FCEyN UBA.
- Zenaida Hernández, M. (2012). *Métodos de análisis de datos* (apuntes). Universidad de La Rioja.

### Herramientas
Python, R, SQL, Cassandra, Pandas.

---

## Clase 1 — Conceptos fundamentales del análisis de datos (21/8)

[![Ver PDF](https://img.shields.io/badge/PDF-Clase%201-blue?logo=adobeacrobatreader)](Material/1%20-%20Clase%201.pdf)

**Dato:** representación de un hecho, observación o característica de un objeto/persona/evento (números, texto, fecha, símbolos, etc.). Por sí solo carece de contexto y significado para tomar decisiones. Ej: 38.5, "Azul", 2026-08-04, 125, "Juan Pérez".

**Tipos de datos según su estructura:**
- **Estructurados:** organizados en tablas (filas/columnas), ej. bases de datos relacionales.
- **Semiestructurados:** XML, JSON, CSV, logs, APIs.
- **No estructurados:** texto libre, imágenes, audio, video, redes sociales.

**¿De qué trata el análisis de datos?** Proceso de recolección (bases de datos, archivos, encuestas) → limpieza → transformación → exploración y visualización → análisis e interpretación → conocimiento accionable (toma de decisiones, resolución de problemas).

**Definición (Wikipedia):** proceso que consiste en inspeccionar, limpiar y transformar datos con el objetivo de resaltar información útil, para sugerir conclusiones y apoyo en la toma de decisiones.

**Perspectiva académica:** una visión más ligada a la estadística reduce el análisis de datos a estadística descriptiva (analiza los datos disponibles) o inferencial (a partir de una muestra, genera predicciones/definiciones para el universo). En la práctica actual, el analista excede ese campo y recurre también a aprendizaje automático y minería de datos.

**Data Mining y Big Data:**
- La minería de datos surge en el siglo XIX con los datos sociales de Quetelet, biológicos de Galton y agronómicos de Fisher.
- Forma parte del proceso de "descubrimiento de conocimiento a partir de los datos" (KDD). Busca extraer información de una gran base de datos sin conocimiento previo, encontrando patrones/relaciones sistemáticas y anomalías.
- **Big Data — las 3(+2) V:** Volumen, Velocidad, Variedad (+ Veracidad y Valor).

**Análisis estadístico vs. Minería de datos**
| Análisis estadístico | Minería de datos |
|---|---|
| Procedimiento hipotético deductivo | Procedimiento inductivo |
| Técnicas confirmatorias | Técnicas exploratorias |
| Supuestos iniciales | Sin supuestos iniciales |
| Herramientas informáticas opcionales | Recursos informáticos indispensables |

**Tipos de variables:**
- **Categóricas:** cualitativas, no se pueden ordenar.
- **Ordinales:** se pueden ordenar, pero no establecer distancia entre valores.
- **Cuantitativas discretas:** numéricas, sin valores intermedios entre dos consecutivos.
- **Cuantitativas continuas:** numéricas, con infinitos valores intermedios posibles.

**Clasificación del análisis según cantidad de variables:**
- **Univariado:** analiza una sola variable. Medidas de tendencia central (media, mediana, moda) y de dispersión (varianza, rango, curtosis). Ej: media etaria del aula.
- **Bivariado/multivariado:** analiza dos o más variables (relación, dependencia, patrones). Ej: clusterización de clientes, regresión entre edad y peso.

**Evolución tecnológica del lenguaje dominante:** históricamente C fue el más usado; luego R creció fuerte hasta llegar a estar en el top 10 (siendo un lenguaje enfocado solo en análisis de datos), mientras C fue cayendo. En 2017 aparece el paper *"Attention Is All You Need"*, que impulsa la explosión de la IA. Desde entonces Python asciende y se convierte en el lenguaje más usado, al superar a R, por ser el lenguaje de la inteligencia artificial y del procesamiento de grandes volúmenes de datos.

### Conceptos estadísticos fundamentales

**Ley de los grandes números** (Jacob Bernoulli, s. XVII): la frecuencia relativa de un evento tiende a converger hacia su probabilidad teórica a medida que aumenta el número de ensayos. En estadística inferencial: a medida que crece el tamaño de la muestra, la media muestral tiende a aproximarse al valor esperado (esperanza matemática) de la población.
- Implicancia práctica: no se pueden sacar conclusiones definitivas sobre fenómenos masivos a partir de casos aislados; hace falta una muestra representativa y lo suficientemente grande.
- Está vinculado al auge de la IA: el salto de capacidad entre modelos (ej. GPT-2 a GPT-3) se explica en gran parte por el volumen de datos de entrenamiento — es una cuestión de escala, no solo conceptual.

**Teorema central del límite** (desarrollado entre los siglos XVIII y XIX, reformulado hasta el s. XX): dada una población con cualquier distribución, la distribución de las medias muestrales tiende a una distribución normal a medida que aumenta el tamaño de la muestra, siempre que la varianza poblacional sea finita.
- Permite, conociendo las propiedades de la distribución normal, testear si una diferencia observada entre dos grupos (ej. rendimiento de dos semillas, una original y una modificada genéticamente) es significativa o no.
- Pendiente de investigar (consigna del profesor): la relación entre el teorema central del límite y el **test de hipótesis**.

---

## Notas de la clase

- Materia de último cuatrimestre, con manejo flexible pero exigiendo marcar asistencia en cada clase.
- 16 clases en total, sin feriados; 4 dedicadas a parciales/instancias evaluativas.
- Primer parcial: teórico, probablemente presencial (se confirma más cerca de la fecha); si es virtual, con cámara prendida y compartiendo pantalla.
- Segundo parcial: trabajo práctico final, similar a cuatrimestres anteriores, se entrega en la segunda mitad de la cursada.
- Quienes no regularicen (menos de 4 en algún parcial) pueden presentarse el 11/12 a un examen integrador para regularizar (nota máxima 4).
- Bibliografía obligatoria: se cubren los dos primeros capítulos del libro de Chan, Badano y Rey (~70 páginas), con ejemplos en R; es la bibliografía "de cabecera" en lo conceptual. El libro de McKinney (Pandas) es más flojo conceptualmente pero útil como referencia práctica de Python.
- El profesor no graba las clases; sube el contenido de las diapositivas al campus.

---

## Estructura del repositorio

```
.
├── README.md
└── Material/
    ├── 0 - Funcionamiento.pdf
    ├── 1 - Clase 1.pdf
    └── ...
```

Cada nueva clase se agrega a `Material/` numerada en orden (`2 - Clase 2.pdf`, `3 - Clase 3.pdf`, ...), y el README se actualiza sumando su sección con el botón correspondiente.
