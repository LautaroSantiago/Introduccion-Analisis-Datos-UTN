# <font color="#1F6FEB">Introducción al Análisis de Datos</font>

Apuntes de cursada y material de clase de la materia **Introducción al Análisis de Datos** (Tecnicatura Universitaria en Programación, UTN Facultad Regional Avellaneda). El objetivo del repositorio es centralizar lo que se va viendo en cada clase, dejar registro de los conceptos y consignas del profesor, y servir de referencia rápida para repasar antes de los parciales.

**Cursada:** 2do. cuatrimestre 2026

<p align="center">

[![Abrir en Colab](https://img.shields.io/badge/📓_Google_Colab-Acceso_directo-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com/drive/1x-5Rp6Erfq18CL7-0ANoI4189KSpoTMt?usp=sharing)

</p>

---

## <font color="#8250DF">🧭 Índice</font>

- [<font color="#8250DF"><strong>Funcionamiento de la materia</strong></font>](#funcionamiento)
  - [<font color="#1A7F37">Modalidad y criterios de evaluación</font>](#funcionamiento-modalidad)
  - [<font color="#1A7F37">Exámenes</font>](#funcionamiento-examenes)
  - [<font color="#1A7F37">Cronograma de clases</font>](#funcionamiento-cronograma)
  - [<font color="#1A7F37">Bibliografía</font>](#funcionamiento-bibliografia)
  - [<font color="#1A7F37">Herramientas</font>](#funcionamiento-herramientas)
- [<font color="#8250DF"><strong>Clase 1 — 21/8 · Conceptos fundamentales del análisis de datos</strong></font>](#clase-1)
  - [<font color="#1A7F37">Dato y tipos de datos</font>](#clase-1-dato)
  - [<font color="#1A7F37">¿De qué trata el análisis de datos?</font>](#clase-1-de-que-trata)
  - [<font color="#1A7F37">Data Mining y Big Data</font>](#clase-1-data-mining)
  - [<font color="#1A7F37">Análisis estadístico vs. Minería de datos</font>](#clase-1-vs-mineria)
  - [<font color="#1A7F37">Tipos de variables</font>](#clase-1-variables)
  - [<font color="#1A7F37">Bases de datos: SQL vs. NoSQL (columnares)</font>](#clase-1-bases-de-datos)
  - [<font color="#1A7F37">Clasificación del análisis según cantidad de variables</font>](#clase-1-clasificacion-analisis)
  - [<font color="#9A6700">Evolución tecnológica del lenguaje dominante</font>](#clase-1-evolucion-lenguajes)
  - [<font color="#1A7F37">Ley de los grandes números</font>](#clase-1-ley-grandes-numeros)
  - [<font color="#1A7F37">Teorema central del límite</font>](#clase-1-teorema-central-limite)
  - [<font color="#9A6700">Relación entre el TCL y el test de hipótesis</font>](#clase-1-tcl-test-hipotesis)
  - [<font color="#1A7F37">Notas de la clase</font>](#clase-1-notas)
- [<font color="#8250DF"><strong>Clase 2 — 28/8 · Numpy y primer acercamiento a Pandas</strong></font>](#clase-2)
  - [<font color="#1A7F37">¿Por qué estudiar Numpy?</font>](#clase-2-motivacion)
  - [<font color="#1A7F37">Qué es Numpy y características generales</font>](#clase-2-definicion)
  - [<font color="#1A7F37">La clase `ndarray`</font>](#clase-2-ndarray)
  - [<font color="#1A7F37">Funciones y atributos principales</font>](#clase-2-funciones)
  - [<font color="#1A7F37">Ecosistema: dónde se usa Numpy</font>](#clase-2-ecosistema)
  - [<font color="#9A6700">Experimento en clase: listas vs. Numpy</font>](#clase-2-experimento)
  - [<font color="#1A7F37">Imágenes como matrices</font>](#clase-2-imagenes)
  - [<font color="#1A7F37">Introducción a Pandas</font>](#clase-2-pandas-intro)
  - [<font color="#1A7F37">Series y DataFrames</font>](#clase-2-series-dataframes)
  - [<font color="#1A7F37">Indexado y filtrado</font>](#clase-2-indexado)
  - [<font color="#1A7F37">Notas de la clase</font>](#clase-2-notas)
- [<font color="#9A6700"><strong>🟣 2/10 · Primer parcial teórico</strong></font>](#eval-2-10)
- [<font color="#8250DF"><strong>Clase 7 — 9/10 · Análisis de datos con R</strong></font>](#clase-7) *(pendiente)*
- [<font color="#9A6700"><strong>🟣 16/10 · Recuperatorio primer parcial</strong></font>](#eval-16-10)
- [<font color="#8250DF"><strong>Clase 8 — 23/10 · Integración de fuentes / SQL con pandas / Cassandra</strong></font>](#clase-8) *(pendiente)*
- [<font color="#8250DF"><strong>Clase 9 — 30/10 · Conceptos básicos del modelado de datos</strong></font>](#clase-9) *(pendiente)*
- [<font color="#8250DF"><strong>Clase 10 — 6/11 · Modelos de clasificación</strong></font>](#clase-10) *(pendiente)*
- [<font color="#8250DF"><strong>Clase 11 — 13/11 · Modelos de regresión</strong></font>](#clase-11) *(pendiente)*
- [<font color="#8250DF"><strong>Clase 12 — 20/11 · Modelos de clustering</strong></font>](#clase-12) *(pendiente)*
- [<font color="#9A6700"><strong>🟣 27/11 · Defensa TP final</strong></font>](#eval-27-11)
- [<font color="#9A6700"><strong>🟣 4/12 · Recuperatorio TP final</strong></font>](#eval-4-12)
- [<font color="#1A7F37"><strong>🟢 11/12 · Instancia de finales y última instancia de recuperatorio</strong></font>](#eval-11-12)

---

## <a id="funcionamiento"></a><font color="#8250DF">🗓️ Funcionamiento de la materia</font>

[![Ver PDF](https://img.shields.io/badge/📄_Ver_PDF-Funcionamiento_de_la_materia-0A66C2?style=for-the-badge)](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/LautaroSantiago/Introduccion-Analisis-Datos-UTN/master/Material/0%20-%20Funcionamiento.pdf)

### <a id="funcionamiento-modalidad"></a><font color="#1A7F37">Modalidad y criterios de evaluación</font>

- **Modalidad:** clases con código en Python y R. Libre elección de lenguaje/IDE — **no se evalúa código**. El código visto en clase se comparte por Google Colab (hay que hacer copia propia para poder modificarlo).
- **Asistencia:** se exige 75% (máximo 3 faltas en el cuatrimestre).
- **Regularidad:** 4 o más en ambos parciales.
- **Aprobación:** 6 o más en ambos parciales, o final en caso de no lograrlo.

### <a id="funcionamiento-examenes"></a><font color="#1A7F37">Exámenes</font>

| Instancia | Fecha | Detalle |
|---|---|---|
| Primer parcial | 2/10 | Teórico y virtual |
| Recuperatorio 1er parcial | 16/10 | — |
| Segundo parcial (TP final) | — | Informe utilizando las bases de la Encuesta Permanente de Hogares (INDEC) |
| Defensa TP final | 27/11 | — |
| Recuperatorio TP final | 4/12 | — |
| Finales / última instancia de recuperatorio | 11/12 | Examen integrador (nota máx. 4) para quienes no regularizaron |

### <a id="funcionamiento-cronograma"></a><font color="#1A7F37">Cronograma de clases</font>

Cada clase se despliega individualmente con su desarrollo completo adentro. Se va actualizando a medida que avanza la cursada — las que todavía no se dictaron dicen *"pendiente"*.

<details>
<summary><a id="clase-1"></a><font color="#1A7F37"><strong>Clase 1 — 21/8 · Conceptos fundamentales del análisis de datos</strong></font></summary>

[![Ver PDF](https://img.shields.io/badge/📄_Ver_PDF-Clase_1-0A66C2?style=for-the-badge)](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/LautaroSantiago/Introduccion-Analisis-Datos-UTN/master/Material/1%20-%20Clase%201.pdf)

#### <a id="clase-1-dato"></a><font color="#1A7F37">Dato y tipos de datos</font>

**Dato:** representación de un hecho, una observación o una característica de un objeto, persona o evento, expresada mediante números, texto, fecha, símbolos o cualquier otro formato. Por sí solo, un dato carece de contexto y significado suficiente para tomar decisiones. *Ejemplos: 38.5, "Azul", 2026-08-04, 125, "Juan Pérez".*

**Tipos de datos según su estructura:**
- **Estructurados:** organizados en tablas (filas/columnas). Ej: bases de datos relacionales.
- **Semiestructurados:** XML, JSON, CSV, logs, APIs.
- **No estructurados:** texto libre, imágenes, audio, video, redes sociales.

#### <a id="clase-1-de-que-trata"></a><font color="#1A7F37">¿De qué trata el análisis de datos?</font>

Proceso de **recolección** (bases de datos, archivos, encuestas) → **limpieza** → **transformación** → **exploración y visualización** → **análisis e interpretación** → **conocimiento accionable** (toma de decisiones, resolución de problemas, respuestas a preguntas).

> **Definición (Wikipedia):** "El análisis de datos es un proceso que consiste en inspeccionar, limpiar y transformar datos con el objetivo de resaltar información útil, para sugerir conclusiones y apoyo en la toma de decisiones."

**Perspectiva académica:** una visión más ligada a la estadística reduce el análisis de datos a estadística descriptiva (analiza los datos disponibles) o inferencial (a partir de una muestra de un universo, genera predicciones/definiciones generales para ese universo). En la práctica actual, el analista de datos excede ese campo tradicional y recurre también al aprendizaje automático y la minería de datos.

#### <a id="clase-1-data-mining"></a><font color="#1A7F37">Data Mining y Big Data</font>

- La minería de datos (*data mining*) surge en el siglo XIX con el análisis de los datos sociales de Quetelet, biológicos de Galton y agronómicos de Fisher. Es un concepto muy reciente si se lo compara con la estadística tradicional (que tiene miles de años de desarrollo).
- Forma parte del proceso conocido como **KDD** (*Knowledge Discovery in Databases* — descubrimiento de conocimiento a partir de los datos): el objetivo es extraer información de una gran base de datos, sin disponer de conocimiento previo, para construir patrones y/o relaciones sistemáticas de valor, así como anomalías. "Sin conocimiento previo" implica un abordaje empírico: se llega a los datos sin una hipótesis de partida y se observa qué está sucediendo.
- **Big Data — las 5 "V":** Volumen, Velocidad y Variedad como las tres centrales; Veracidad y Valor como las dos adicionales a tener en cuenta. *⚠️ Marcado explícitamente como tema de parcial.*
- Definir Big Data por una cantidad fija (ej. "más de X TB") pierde sentido rápido, porque la capacidad de procesamiento crece todo el tiempo — por eso se lo define como concepto y no como una cifra. Es un campo en permanente evolución, donde los términos de moda van cambiando (ciencia de datos → minería de datos → big data → inteligencia artificial), aunque todos están relacionados entre sí.

#### <a id="clase-1-vs-mineria"></a><font color="#1A7F37">Análisis estadístico vs. Minería de datos</font>

| Análisis estadístico | Minería de datos |
|---|---|
| Procedimiento hipotético deductivo | Procedimiento inductivo |
| Técnicas confirmatorias | Técnicas exploratorias |
| Supuestos iniciales | Sin supuestos iniciales |
| Herramientas informáticas opcionales | Recursos informáticos indispensables |

El procedimiento **hipotético-deductivo** parte de una hipótesis y la contrasta con la realidad para ver si se sostiene o no. El procedimiento **inductivo**, en cambio, generaliza a partir de la observación, sin hipótesis previa. Durante buena parte del siglo XX el método inductivo estuvo "mal visto" en el ámbito científico — se pensaba que ya no era necesario dado el desarrollo alcanzado por el método hipotético-deductivo — pero la aparición de los grandes volúmenes de datos actuales lo volvió a poner en valor. Aun así, hay que ser cauteloso con las generalizaciones que produce, ya que carecen del respaldo de una hipótesis validada.

#### <a id="clase-1-variables"></a><font color="#1A7F37">Tipos de variables</font>

- **Categóricas:** cualitativas, no se pueden ordenar. Ej: nombre, ciudad.
- **Ordinales:** se pueden ordenar, pero no se puede establecer distancia entre valores. Ej: una calificación de atención al cliente (mala, regular, buena, muy buena).
- **Cuantitativas discretas:** numéricas; entre dos valores consecutivos no poseen valores intermedios. Ej: cantidad de hijos de una persona.
- **Cuantitativas continuas:** numéricas; entre dos valores poseen infinitos valores intermedios. Ej: una distancia.

> *⚠️ Marcado explícitamente como tema de parcial:* esta clasificación es "recontrabásica" — aplicar mal esta distinción en el trabajo práctico final (usar técnicas de variables cuantitativas sobre variables categóricas, por ejemplo) es motivo de ir a recuperatorio.

#### <a id="clase-1-bases-de-datos"></a><font color="#1A7F37">Bases de datos: SQL vs. NoSQL (columnares)</font>

Dentro de la "pata tecnológica" del análisis de datos, se repasó la diferencia entre tipos de bases de datos:

- **SQL:** construida priorizando la **persistencia y consistencia** de la información (toda la información tiene que estar siempre disponible y completa — por ejemplo, en una cuenta bancaria no puede faltar información). Está organizada por filas: procesar una sola columna igual implica recorrer en memoria toda la fila, lo cual es costoso si solo se necesita una porción de los datos.
- **NoSQL:** prioriza la **velocidad de procesamiento** por sobre la consistencia total. Es útil en casos donde no hace falta tener siempre el 100% de la información disponible (ej: una red social puede seguir funcionando aunque se pierda temporalmente un nodo o *data center*).
- **Bases de datos columnares** (ej. **Cassandra**, un tipo de NoSQL): invierten la lógica de procesamiento respecto a SQL — trabajan columna por columna en lugar de fila por fila, lo cual resulta mucho más eficiente cuando el análisis de datos necesita operar sobre variables (columnas) puntuales en vez de registros completos.

#### <a id="clase-1-clasificacion-analisis"></a><font color="#1A7F37">Clasificación del análisis según cantidad de variables</font>

| Univariado | Bivariado o multivariado |
|---|---|
| Análisis de una sola variable a la vez. | Se analizan dos o más variables, a nivel de su relación, dependencia o patrones. |
| Medidas de tendencia central (media, mediana, moda) o de dispersión (varianza, rango) u otras (curtosis). | Ej: clusterización de clientes de una empresa, regresión entre edad y peso. |
| Ejemplo: media etaria del aula. | |

#### <a id="clase-1-evolucion-lenguajes"></a><font color="#9A6700">Evolución tecnológica del lenguaje dominante</font>

Históricamente **C** fue el lenguaje más usado. Python fue creado por **Guido van Rossum en 1989**, con la filosofía de ser un lenguaje simple y accesible — priorizando que sea fácil de leer por sobre estar altamente optimizado (algo que en la década de 1990, con hardware muy limitado, generó bastantes críticas). Con el tiempo, **R** creció fuerte hasta ubicarse en el top 10 (siendo un lenguaje enfocado exclusivamente en análisis de datos), mientras C fue perdiendo terreno. En 2017 aparece el paper *"Attention Is All You Need"*, que impulsa la explosión de la inteligencia artificial. Desde entonces, **Python** asciende hasta convertirse en el lenguaje más usado, superando incluso a R, por ser el lenguaje de la IA y del procesamiento de grandes volúmenes de datos — impulsado en gran parte por Numpy (ver Clase 2).

#### <a id="clase-1-ley-grandes-numeros"></a><font color="#1A7F37">Ley de los grandes números</font>

Formulada originalmente por **Jacob Bernoulli** en el siglo XVII: la frecuencia relativa de un evento tiende a converger hacia su probabilidad teórica a medida que aumenta el número de ensayos. En el contexto de la estadística inferencial: a medida que crece el tamaño de una muestra tomada de una población, la media muestral tiende a aproximarse cada vez más al valor esperado (esperanza matemática) de la población.

> *⚠️ Marcado explícitamente como concepto a estudiar/consolidar para los exámenes, junto con el teorema central del límite (ver abajo).*

- **Implicancia práctica:** no se pueden sacar conclusiones definitivas sobre fenómenos masivos a partir de casos aislados; hace falta una muestra representativa y lo suficientemente grande.
- **Vínculo con la IA:** el salto de capacidad entre modelos (ej. GPT-2 a GPT-3) se explica en gran parte por el volumen de datos de entrenamiento — es una cuestión de escala, no solo conceptual.

#### <a id="clase-1-teorema-central-limite"></a><font color="#1A7F37">Teorema central del límite</font>

Desarrollado originalmente entre los siglos XVIII y XIX, y reformulado hasta el siglo XX. Establece que, dada una población con cualquier distribución, la distribución de las medias muestrales tiende a una distribución normal a medida que aumenta el tamaño de la muestra, siempre que la varianza poblacional sea finita.

- Permite, conociendo las propiedades de la distribución normal, testear si una diferencia observada entre dos grupos (ej. rendimiento de dos semillas, una original y una modificada genéticamente) es significativa o no.

> *⚠️ Concepto que el profesor pidió consolidar bien para los exámenes — es habitual confundirlo con la ley de los grandes números.*

#### <a id="clase-1-tcl-test-hipotesis"></a><font color="#9A6700">Relación entre el TCL y el test de hipótesis</font>

*(Consigna del profesor para investigar.)*

El test de hipótesis necesita saber qué forma tiene la distribución de un estadístico (por ejemplo, la media muestral) para poder calcular probabilidades y decidir si un resultado es "raro" o no. El **Teorema Central del Límite** es lo que garantiza esa forma: dice que, sin importar cómo se distribuya la población original, la distribución de las medias muestrales se aproxima a una normal a medida que crece el tamaño de la muestra (n).

Eso es lo que habilita todo el mecanismo del test de hipótesis:

1. Se plantea una **hipótesis nula (H₀)** (ej: "las dos semillas rinden igual").
2. Gracias al TCL, se sabe que la media muestral sigue (aproximadamente) una distribución normal, con lo cual se puede calcular su desvío estándar (error estándar) y ubicar el resultado observado dentro de esa curva.
3. Se calcula qué tan probable es obtener la diferencia observada (o una más extrema) **si H₀ fuera cierta** — esto es el **p-valor**.
4. Si esa probabilidad es muy baja (por debajo de un umbral, típicamente 0.05), se **rechaza H₀**: la diferencia es estadísticamente significativa y no se explica solo por azar muestral.

> **Idea clave:** en el ejemplo de las semillas no alcanza con comparar dos medias "a ojo". El TCL permite construir la distribución esperada de esas medias bajo el supuesto de que no hay diferencia real, y sobre esa distribución normal se aplica el test para decidir si la diferencia observada es lo bastante grande como para no ser producto del azar. Sin el TCL no habría base teórica para saber qué distribución usar ni cómo calcular esas probabilidades — es el fundamento estadístico detrás de la mayoría de los test de hipótesis paramétricos (test t, test z, ANOVA, etc.).

#### <a id="clase-1-notas"></a><font color="#1A7F37">Notas de la clase</font>

- Materia de último cuatrimestre, con manejo flexible pero exigiendo marcar asistencia en cada clase.
- 16 clases en total, sin feriados; 4 dedicadas a parciales/instancias evaluativas.
- Primer parcial: teórico, probablemente presencial (se confirma más cerca de la fecha); si es virtual, con cámara prendida y compartiendo pantalla.
- Segundo parcial: trabajo práctico final, similar a cuatrimestres anteriores, se entrega en la segunda mitad de la cursada.
- El profesor no graba las clases; sube el contenido de las diapositivas al campus.

</details>

<details>
<summary><a id="clase-2"></a><font color="#1A7F37"><strong>Clase 2 — 28/8 · Numpy y primer acercamiento a Pandas</strong></font></summary>

#### <a id="clase-2-motivacion"></a><font color="#1A7F37">¿Por qué estudiar Numpy?</font>

La clase retoma la Clase 1: el crecimiento exponencial del volumen de datos disponibles en la web (desde los años 90) generó la necesidad de desarrollar tanto tecnologías como herramientas estadísticas para procesarlos. Esta clase se centra en el eje tecnológico: qué hizo que **Python** se expandiera hasta convertirse en el lenguaje hegemónico del análisis de datos y la inteligencia artificial.

Numpy no es una librería que se use de forma directa y permanente en el trabajo práctico final (para eso está Pandas, que se construye sobre ella), pero entender su funcionamiento explica gran parte de por qué Python llegó a ser tan popular en este campo.

> *⚠️ Marcado explícitamente como tema de parcial:* por qué Numpy es tan importante para la expansión de Python.

#### <a id="clase-2-definicion"></a><font color="#1A7F37">Qué es Numpy y características generales</font>

**Numpy** (*Numerical Python*) sirve para la manipulación eficiente de vectores. Aunque su nombre remite al procesamiento de números, sus características van más allá de solo trabajar con variables cuantitativas: apuntan a optimizar cualquier procedimiento que involucre datos numéricos.

Características principales:
- Está **desarrollada en C** (no en Python), un lenguaje de bajo nivel, tipado y compilado, que permite un acceso mucho más preciso y directo a la memoria — algo que Python, al ser de alto nivel, no ofrece por sí mismo.
- Está orientada al trabajo con **arrays multidimensionales** y grandes volúmenes de información.
- Es de código abierto y multiplataforma.
- Está optimizada con altos estándares de calidad, lo que da como resultado dos ventajas centrales: **mayor velocidad de procesamiento** y **menor uso de memoria**.

Python se diseñó priorizando la legibilidad por sobre la optimización (el programador pasa más tiempo leyendo código que escribiéndolo). Numpy funciona como un "parche" que compensa esa falta de optimización en el trabajo con datos numéricos, combinando lo mejor de dos mundos: la legibilidad de un lenguaje de alto nivel y el rendimiento de uno de bajo nivel como C.

#### <a id="clase-2-ndarray"></a><font color="#1A7F37">La clase `ndarray`</font>

Es la clase fundamental de Numpy — base de todas las operaciones matemáticas y numéricas que ofrece la librería.

> *⚠️ Marcado explícitamente como tema de parcial:* cuáles son las características de `ndarray` y por qué es tan importante.

A diferencia de las **listas de Python** (mutables, de tamaño variable, capaces de mezclar tipos de datos en distintas posiciones, lo que obliga a reservar y gestionar memoria de forma poco eficiente), un `ndarray`:
- Se crea con un **tamaño fijo** desde su instanciación, con espacios de memoria contiguos reservados.
- Exige que **todos sus elementos sean del mismo tipo**. La excepción es un vector de objetos, que sí permite mezclar tamaños o tipos distintos, aunque a costa de perder parte de la optimización.
- Al tener tamaño y tipo fijos, permite reservar en memoria exactamente el espacio necesario, sin desperdicio — lo cual acelera notablemente las operaciones matemáticas y algebraicas sobre grandes volúmenes de datos.

#### <a id="clase-2-funciones"></a><font color="#1A7F37">Funciones y atributos principales</font>

**Algunas funciones útiles:**
- Creación de vectores: de ceros, de unos, con valores aleatorios.
- `arange`: una adaptación de `range` que además permite trabajar con decimales.
- `linspace`: crea un array con intervalos regulares.
- `sort`: ordenamiento de vectores.
- `concatenate`: une arrays, permitiendo también agregar dimensiones.
- `flatten`: transforma una matriz en un vector de una sola dimensión — trabajar en una dimensión suele ser más veloz que en varias, por eso muchos algoritmos de IA aplanan una matriz antes de procesarla.
- `reshape`: permite modificar la forma de un array sin generar un uso excesivo de memoria.
- Funciones matemáticas: suma, media, desvío estándar, etc.

**Atributos del `ndarray`:**
- `ndim`: número de dimensiones.
- `shape`: tupla con la cantidad de elementos en cada dimensión.
- `dtype`: tipo de dato de los elementos.
- `size`: cantidad total de elementos.
- `itemsize`: tamaño en bytes de cada elemento.
- `data` / buffer: acceso a los elementos de la matriz.
- `T`: la transpuesta de la matriz.

#### <a id="clase-2-ecosistema"></a><font color="#1A7F37">Ecosistema: dónde se usa Numpy</font>

Numpy es ampliamente utilizado por otras librerías como base — muchas veces de forma invisible para quien las usa. Aparece en: big data, estadística avanzada (frecuentista y bayesiana), álgebra lineal, procesamiento de lenguaje natural, procesamiento de imágenes y señales, grafos y redes, computación cuántica, astronomía, biología/bioinformática, análisis matemático, geografía, entre otras disciplinas.

Algunos casos de uso reales: procesamiento de las primeras imágenes de agujeros negros, detección de ondas gravitacionales, análisis de datos deportivos, seguimiento de posiciones de animales mediante aprendizaje profundo.

Librerías construidas sobre Numpy: **Pandas** (la que se usa en esta materia), Python Control (señales), NetworkX (grafos), TensorFlow y PyTorch (redes neuronales / deep learning), entre otras. Numpy sentó las bases para que Python se expandiera y que todo este ecosistema pudiera crecer.

#### <a id="clase-2-experimento"></a><font color="#9A6700">Experimento en clase: listas vs. Numpy</font>

*(Actividad práctica realizada en Google Colab.)*

Se comparó el tiempo que tardan en elevar al cuadrado un millón de elementos (10⁶):
1. Una lista de Python (usando comprensión de listas).
2. Un array de Numpy, creado con `arange`.

El resultado mostró que Numpy resolvió la operación varias decenas de veces más rápido que la lista (la diferencia relativa varió entre corridas, mostrando cierta dispersión en los resultados).

**Consigna vinculada a la ley de los grandes números:** repetir el experimento y promediar los resultados de todo el grupo, para verificar cómo, a medida que aumenta la cantidad de mediciones, el promedio se acerca a la diferencia real de rendimiento entre listas y Numpy. Con los resultados aportados por el grupo, se confirmó que Numpy es sistemáticamente más rápido, y que agregar más resultados estabiliza la estimación de esa diferencia — una aplicación directa del concepto visto en la Clase 1.

**Segunda consigna:** graficar la densidad de esos resultados y comprobar si, tal como predice el **teorema central del límite**, la distribución se aproxima a una campana de Gauss (forma de la distribución normal).

**Comparación de memoria:** una lista de Python de 10.000 elementos ocupó 360.056 bytes, mientras que un array de Numpy con la misma cantidad de elementos ocupó 80.000 bytes — otra de las razones por las que Numpy resulta más veloz: al ocupar menos memoria, todo el procesamiento es más eficiente.

#### <a id="clase-2-imagenes"></a><font color="#1A7F37">Imágenes como matrices</font>

Una imagen en blanco y negro puede representarse con una sola matriz (cada valor indica intensidad de gris). Una imagen a color, en cambio, es la **superposición de tres matrices** (canales rojo, verde y azul — de ahí el sistema RGB usado también en HTML/CSS): cada canal aporta su intensidad en cada posición, y la combinación de los tres genera el color final. Esto explica por qué Numpy es clave en el procesamiento de imágenes: generarlas o predecirlas mediante IA implica, en el fondo, operar matemáticamente sobre matrices.

#### <a id="clase-2-pandas-intro"></a><font color="#1A7F37">Introducción a Pandas</font>

**Pandas** está orientada al trabajo con **datos estructurados** (tablas — a diferencia de los no estructurados como imágenes o lenguaje, y los semiestructurados vistos en la Clase 1). Fue desarrollada por **Wes McKinney** (autor del libro de bibliografía obligatoria *Python para análisis de datos*), buscando imitar funcionalidades de un lenguaje preexistente: **R**.

Características:
- Código abierto y multiplataforma.
- Optimizada con altos estándares de calidad, ya que internamente utiliza Numpy para el procesamiento de las variables numéricas de las tablas.
- Sintaxis de alto nivel, como el resto de Python.
- Permite leer y guardar datos tabulares en distintos formatos: CSV, Excel, JSON, entre otros.
- A diferencia de Numpy (pensado sobre todo para números), permite trabajar con variables ordinales, de fecha, de texto, y realizar uniones entre tablas.

#### <a id="clase-2-series-dataframes"></a><font color="#1A7F37">Series y DataFrames</font>

Pandas se apoya en dos estructuras de datos básicas:

- **Series:** vectores unidimensionales con etiquetas. En la práctica son dos vectores corriendo en paralelo — uno de **valores** (que internamente usa la clase `ndarray` de Numpy) y otro de **índices/etiquetas** (de un tipo propio de Pandas, no de Numpy). Comparten la mayoría de los atributos de `ndarray` (`shape`, `dtype`, `size`, etc.), pero no incluyen métodos como `flatten` o `reshape`, porque no tendría sentido "aplanar" algo que necesariamente mantiene valores y etiquetas asociados en paralelo, ni mezclar en una misma estructura columnas de distinto tipo de dato.
- **DataFrames:** estructuras bidimensionales construidas sobre la base de las series (equivalen a una tabla completa, con varias columnas).

Pandas suma funciones propias para exploración, manipulación y transformación de datos: `head` (primeros elementos), `describe` (medidas de tendencia central y estadísticas descriptivas), eliminación de valores nulos, `apply` (aplicar una función a cada elemento), `info` (resumen del contenido del DataFrame), agrupamientos, y métodos para exportar a CSV/Excel, entre otros.

> **Ojo con esto:** en un DataFrame, el tipo de dato (`dtype`) que se reporta por columna corresponde al tipo de los **valores**, no al de las etiquetas/índice.

#### <a id="clase-2-indexado"></a><font color="#1A7F37">Indexado y filtrado</font>

El **índice** es una de las características más importantes de Pandas: permite filtrar y quedarse solo con los elementos relevantes para el análisis que se esté haciendo (por ejemplo, quedarse únicamente con registros de una zona geográfica puntual, descartando el resto).

Formas de seleccionar datos, ejemplificadas en clase con un dataset de personajes de un videojuego:
- **Por columnas:** por nombre (entre corchetes o con notación de punto) o por posición, usando `iloc`.
- **Por filas:** por posición con `iloc` (siempre fila a la izquierda, columna a la derecha), o mediante *queries* de estilo SQL para filtrar filas según una condición (por ejemplo, quedarse con los registros que superen cierto valor en un atributo).

**Datasets para practicar:** se mencionó **Kaggle** como una de las plataformas de referencia de la comunidad de ciencia de datos e IA, con cientos de miles de datasets públicos, notebooks y modelos preentrenados disponibles para descargar (incluye una librería propia, `kagglehub`, para acceder a ellos vía API).

#### <a id="clase-2-notas"></a><font color="#1A7F37">Notas de la clase</font>

- La clase se dio en dos partes, con material y ejercicios compartidos vía Google Colab.
- Recomendación: dedicar aunque sea media hora por semana a los ejercicios de la materia ayuda a llegar mejor preparado a los parciales y al trabajo práctico final, sin necesidad de grandes bloques de tiempo.
- Los ejercicios de cada clase quedan disponibles en la sección de materiales del campus; se retoman al principio de la clase siguiente.
- El ejercicio de esta clase consistía en empezar a observar el dataset con el que se va a trabajar en el trabajo práctico final de fin de cuatrimestre.

</details>

<details>
<summary><font color="#1A7F37">Clase 3 — 4/9 · Pandas</font></summary>

*Pendiente.*

</details>

<details>
<summary><font color="#1A7F37">Clase 4 — 11/9 · Data cleaning</font></summary>

*Pendiente.*

</details>

<details>
<summary><font color="#1A7F37">Clase 5 — 18/9 · Análisis exploratorio de datos y estadística descriptiva</font></summary>

*Pendiente.*

</details>

<details>
<summary><font color="#1A7F37">Clase 6 — 25/9 · Visualización de datos</font></summary>

*Pendiente.*

</details>

<details>
<summary><a id="eval-2-10"></a><font color="#9A6700">🟣 2/10 · Primer parcial teórico</font></summary>

**Fecha evaluatoria.** Primer parcial: teórico y virtual.

</details>

<details>
<summary><a id="clase-7"></a><font color="#1A7F37"><strong>Clase 7 — 9/10 · Análisis de datos con R</strong></font></summary>

*Pendiente.*

</details>

<details>
<summary><a id="eval-16-10"></a><font color="#9A6700">🟣 16/10 · Recuperatorio primer parcial</font></summary>

**Fecha evaluatoria.**

</details>

<details>
<summary><a id="clase-8"></a><font color="#1A7F37"><strong>Clase 8 — 23/10 · Integración de fuentes / SQL con pandas / Cassandra</strong></font></summary>

*Pendiente.*

</details>

<details>
<summary><a id="clase-9"></a><font color="#1A7F37"><strong>Clase 9 — 30/10 · Conceptos básicos del modelado de datos</strong></font></summary>

*Pendiente.*

</details>

<details>
<summary><a id="clase-10"></a><font color="#1A7F37"><strong>Clase 10 — 6/11 · Modelos de clasificación</strong></font></summary>

*Pendiente.*

</details>

<details>
<summary><a id="clase-11"></a><font color="#1A7F37"><strong>Clase 11 — 13/11 · Modelos de regresión</strong></font></summary>

*Pendiente.*

</details>

<details>
<summary><a id="clase-12"></a><font color="#1A7F37"><strong>Clase 12 — 20/11 · Modelos de clustering</strong></font></summary>

*Pendiente.*

</details>

<details>
<summary><a id="eval-27-11"></a><font color="#9A6700">🟣 27/11 · Defensa TP final</font></summary>

**Fecha evaluatoria.** Segundo parcial: defensa del trabajo práctico final (informe con bases de la Encuesta Permanente de Hogares — INDEC).

</details>

<details>
<summary><a id="eval-4-12"></a><font color="#9A6700">🟣 4/12 · Recuperatorio TP final</font></summary>

**Fecha evaluatoria.**

</details>

<details>
<summary><a id="eval-11-12"></a><font color="#1A7F37">🟢 11/12 · Instancia de finales y última instancia de recuperatorio</font></summary>

**Fecha evaluatoria.** Examen integrador para quienes no llegaron a regularizar (nota máxima 4), y última instancia de finales.

</details>

<p align="center">

[![Ver Cronograma](https://img.shields.io/badge/🖼️_Ver_Cronograma-Cronograma_de_clases-0A66C2?style=for-the-badge)](https://raw.githubusercontent.com/LautaroSantiago/Introduccion-Analisis-Datos-UTN/master/Material/cronograma.png)

</p>

### <a id="funcionamiento-bibliografia"></a><font color="#1A7F37">Bibliografía</font>

**Obligatoria**
- Chan, D., Badano, C., Rey, A. (2019). *Análisis inteligente de datos con lenguaje R* (pp. 1-73). edUTecNe. — se ven los dos primeros capítulos (introducción a la minería de datos e introducción al análisis de datos); es la referencia conceptual "de cabecera" de la materia, con ejemplos en R.
- McKinney, W. (2023). *Python para análisis de datos*. Ediciones Anaya Multimedia. (Trabajo original 2022) — el autor es el creador de Pandas; se usa más como referencia práctica de Python que conceptual.

**Optativa**
- Mitchell, T. (1997). *Machine Learning*. McGraw Hill.
- Szretter Noste, M. E. (2017). *Apunte de regresión lineal*. FCEyN UBA.
- Zenaida Hernández, M. (2012). *Métodos de análisis de datos* (apuntes). Universidad de La Rioja.

### <a id="funcionamiento-herramientas"></a><font color="#1A7F37">Herramientas</font>

`Python` · `R` · `SQL` · `Cassandra` · `Pandas` · `Google Colab`

---

## <font color="#8250DF">🗂️ Estructura del repositorio</font>

```
Introducción al Análisis de Datos
├── Material
│   ├── 0 - Funcionamiento.pdf
│   └── 1 - Clase 1.pdf
└── README.md
```

Cada nueva clase se agrega a `Material/` numerada en orden (`2 - Clase 2.pdf`, `3 - Clase 3.pdf`, ...).
