# 📊 Introducción al Análisis de Datos — Guía de estudio unificada (clases + libro)

**UTN Avellaneda · Tecnicatura Universitaria en Programación · 2do. cuatrimestre 2026**
**Docente:** Fernández, Luis N.
**Libro base:** *Análisis inteligente de datos con lenguaje R* — Débora Chan, Cristina Inés Badano, Andrea Alejandra Rey (edUTecNe, UTN, 1ª ed., 2019). Temática: minería de datos, componentes principales, contrastes de independencia, análisis de correspondencias, escalamiento multidimensional y métodos de clasificación supervisada y no supervisada.

<a id="indice"></a>

## 📑 Índice

> Hacé clic en cualquier tema para ir directo. Cada sección tiene un enlace **⬆️ Volver al índice** al inicio.

- **[🎯 PANEL DEL PARCIAL (leer primero)](#-panel-del-parcial-leer-primero)**
  - [Logística (dicha en clase)](#logística-dicha-en-clase)
  - [📩 Último aviso del docente (paro docente y marcha federal del 15/10)](#-último-aviso-del-docente-paro-docente-y-marcha-federal-del-1510)
  - [¿Qué temas entran?](#qué-temas-entran)
  - [Preguntas que mencionó explícitamente (las más probables)](#preguntas-que-mencionó-explícitamente-las-más-probables)
  - [Lo que dijo que NO va a tomar](#lo-que-dijo-que-no-va-a-tomar)
- **[1. 🧠 Conceptos fundamentales del análisis de datos (Clase 1 + Cap. 1)](#1--conceptos-fundamentales-del-análisis-de-datos-clase-1--cap-1)**
  - [1.1 Dato](#11-dato)
  - [1.2 Tipos de datos según su estructura](#12-tipos-de-datos-según-su-estructura)
  - [1.3 ¿De qué trata el análisis de datos? (el proceso)](#13-de-qué-trata-el-análisis-de-datos-el-proceso)
  - [1.4 Definiciones de análisis de datos](#14-definiciones-de-análisis-de-datos)
  - [1.5 Contexto histórico, Data Mining y Big Data](#15-contexto-histórico-data-mining-y-big-data)
  - [1.6 Análisis estadístico vs. Minería de datos 🎯 (cuadro clave)](#16-análisis-estadístico-vs-minería-de-datos--cuadro-clave)
  - [1.7 Tipos de variables 🎯](#17-tipos-de-variables-)
  - [1.8 Clasificación según cantidad de variables](#18-clasificación-según-cantidad-de-variables)
  - [1.9 Tecnologías (la "pata tecnológica")](#19-tecnologías-la-pata-tecnológica)
- **[2. 📐 Conceptos estadísticos fundamentales](#2--conceptos-estadísticos-fundamentales)**
  - [2.1 Ley de los grandes números (LGN) 🎯](#21-ley-de-los-grandes-números-lgn-)
  - [2.2 Teorema central del límite (TCL) 🎯](#22-teorema-central-del-límite-tcl-)
  - [2.3 Relación entre el TCL y el test de hipótesis 🎯](#23-relación-entre-el-tcl-y-el-test-de-hipótesis-)
- **[3. 🔢 NumPy — manipulación eficiente de vectores](#3--numpy--manipulación-eficiente-de-vectores)**
  - [3.1 ¿Qué es?](#31-qué-es)
  - [3.2 La clase `numpy.ndarray` 🎯](#32-la-clase-numpyndarray-)
  - [3.3 Atributos y métodos](#33-atributos-y-métodos)
  - [3.4 Experimento de la clase 🗣 (lista vs. NumPy)](#34-experimento-de-la-clase--lista-vs-numpy)
  - [3.5 Imágenes como arrays 🗣](#35-imágenes-como-arrays-)
- **[4. 🐼 Pandas — análisis de datos estructurados](#4--pandas--análisis-de-datos-estructurados)**
  - [4.1 ¿Qué es?](#41-qué-es)
  - [4.2 Estructuras básicas](#42-estructuras-básicas)
  - [4.3 Selección de columnas](#43-selección-de-columnas)
  - [4.4 Filtrado de filas](#44-filtrado-de-filas)
  - [4.6 Fechas y texto](#46-fechas-y-texto)
  - [4.7 Datos usados en clase 🗣](#47-datos-usados-en-clase-)
  - [4.8 Ejercicio de la Clase 2: base de microdatos de la EPH 🗣](#48-ejercicio-de-la-clase-2-base-de-microdatos-de-la-eph-)
- **[5. 🧹 Data cleaning — limpieza y preparación](#5--data-cleaning--limpieza-y-preparación)**
  - [5.1 Contexto (ETL) y etapas 🗣](#51-contexto-etl-y-etapas-)
  - [5.2 Valores duplicados](#52-valores-duplicados)
  - [5.3 Valores perdidos o "no respuesta" (datos faltantes)](#53-valores-perdidos-o-no-respuesta-datos-faltantes)
  - [5.4 Valores atípicos (outliers) e inconsistentes 🎯](#54-valores-atípicos-outliers-e-inconsistentes-)
- **[6. 🔄 Transformación de datos](#6--transformación-de-datos)**
  - [6.1 Transformaciones por variables (columnas)](#61-transformaciones-por-variables-columnas)
  - [6.2 Transformaciones por individuo (filas)](#62-transformaciones-por-individuo-filas)
- **[7. 📈 Análisis estadístico de datos](#7--análisis-estadístico-de-datos)**
  - [7.1 Organización de los datos](#71-organización-de-los-datos)
  - [7.2 Análisis de frecuencias](#72-análisis-de-frecuencias)
  - [7.3 Medidas descriptivas univariadas (una variable a la vez)](#73-medidas-descriptivas-univariadas-una-variable-a-la-vez)
  - [7.4 Análisis bivariado](#74-análisis-bivariado)
  - [7.5 Análisis multivariado](#75-análisis-multivariado)
  - [7.6 📖 Ejercitación del libro (Cap. 2)](#76--ejercitación-del-libro-cap-2)
- **[8. 🗂 Resumen rápido (tablas para repasar)](#8--resumen-rápido-tablas-para-repasar)**
  - [8.1 Qué hacer con cada problema de datos](#81-qué-hacer-con-cada-problema-de-datos)
  - [8.2 NumPy vs. Pandas](#82-numpy-vs-pandas)
  - [8.3 Medidas: de qué "familia" son](#83-medidas-de-qué-familia-son)
  - [8.4 Transformaciones](#84-transformaciones)
  - [8.5 Patrones de no respuesta (semáforo)](#85-patrones-de-no-respuesta-semáforo)
  - [8.6 Σ vs. R](#86-σ-vs-r)
- **[9. 🧩 Mnemotecnias](#9--mnemotecnias)**
- **[10. ✅ Preguntas de autoevaluación](#10--preguntas-de-autoevaluación)**
- **[11. 📋 Información de cursada](#11--información-de-cursada)**
  - [Aprobación y asistencia 🗣](#aprobación-y-asistencia-)
  - [Bibliografía 🗣](#bibliografía-)
  - [TP final 🗣](#tp-final-)
  - [Cronograma de clases y evaluaciones](#cronograma-de-clases-y-evaluaciones)
  - [Recursos y herramientas](#recursos-y-herramientas)
- **[12. 🚫 Anexo: Álgebra lineal y Análisis de Componentes Principales (Cap. 3 del libro)](#12--anexo-álgebra-lineal-y-análisis-de-componentes-principales-cap-3-del-libro)**
  - [12.1 Nociones previas de álgebra lineal](#121-nociones-previas-de-álgebra-lineal)
  - [12.2 Transformaciones lineales](#122-transformaciones-lineales)
- **[13. 📝 Modelos de examen (simulacros)](#13--modelos-de-examen-simulacros)**
  - [13.1 Cómo están armados (y por qué)](#131-cómo-están-armados-y-por-qué)
  - [13.2 Modelo 1](#132-modelo-1)
  - [13.3 Modelo 2](#133-modelo-2)
  - [13.4 Autochequeo rápido antes de rendir](#134-autochequeo-rápido-antes-de-rendir)
- **[14. Glosario](#14-glosario)**
  - [Pares que se confunden](#pares-que-se-confunden)
  - [Datos, análisis y minería de datos](#datos-análisis-y-minería-de-datos)
  - [Tecnologías](#tecnologías)
  - [NumPy y Pandas](#numpy-y-pandas)
  - [Ley de grandes números, TCL y test de hipótesis](#ley-de-grandes-números-tcl-y-test-de-hipótesis)
  - [Data cleaning](#data-cleaning)
  - [Transformaciones](#transformaciones)
  - [Estadística descriptiva](#estadística-descriptiva)
  - [Bivariado y multivariado](#bivariado-y-multivariado)
  - [Gráficos y exploración multivariada 📖🚫](#gráficos-y-exploración-multivariada-)
  - [Estadística robusta multivariada 📖](#estadística-robusta-multivariada-)
  - [Álgebra lineal y PCA 🚫](#álgebra-lineal-y-pca-)

### ⚡ Accesos rápidos (lo que más probablemente entra)

- [Último aviso del docente (paro y parcial)](#-último-aviso-del-docente-paro-docente-y-marcha-federal-del-1510)
- [Estadística vs. minería (cuadro clave)](#16-análisis-estadístico-vs-minería-de-datos--cuadro-clave)
- [Big Data: las 3 V (+2)](#big-data-)
- [Tipos de variables](#17-tipos-de-variables-)
- [NumPy y `ndarray`](#3--numpy--manipulación-eficiente-de-vectores)
- [Atípico vs. inconsistente](#54-valores-atípicos-outliers-e-inconsistentes-)
- [Z-score y transformaciones](#61-transformaciones-por-variables-columnas)
- [La mediana: ¿central o posición?](#-posición-)
- [Interpretar una matriz de correlación](#correlación-)
- [LGN vs. TCL](#2--conceptos-estadísticos-fundamentales)
- [Relación TCL ↔ test de hipótesis](#23-relación-entre-el-tcl-y-el-test-de-hipótesis-)
- [Ejercicios del libro (Cap. 2)](#76--ejercitación-del-libro-cap-2)
- [Cronograma de clases y evaluaciones](#cronograma-de-clases-y-evaluaciones)
- [Modelos de examen (simulacros)](#13--modelos-de-examen-simulacros)
- [Preguntas de autoevaluación](#10--preguntas-de-autoevaluación)

---

## 🔑 Referencias

| Ícono | Significado |
|---|---|
| 🎯 | El docente dijo que **entra / puede entrar / es pregunta de parcial** |
| 🗣️ | Información **agregada desde las clases** (no está en las diapositivas) |
| 📖 | Información **del libro** (Chan, Badano y Rey) que complementa o amplía las clases |
| ⚠️ | Aclaración para evitar confusiones |
| 💡 | Truco para memorizar |
| 🚫 | Lo que el docente dijo que **NO entra** (se conserva por completitud) |
| ➕ | **Complemento**: aparece en tus resúmenes o en las continuaciones de texto, pero **no figura en el PDF del libro** (Cap. 1, Cap. 2 y comienzo del Cap. 3). Útil, pero no lo cites como "del libro" |

---

# 🎯 PANEL DEL PARCIAL (leer primero)

[⬆️ Volver al índice](#indice)

## Logística (dicha en clase)

| Dato | Detalle |
|---|---|
| **Fecha** | **Viernes 2 de octubre** |
| **Lugar** | **Aula 308**, **presencial** (reconfirmado en el último aviso del docente) |
| **Formato** | **Escrito, a mano** (hoja y lapicera). Preguntas **teóricas a desarrollar + múltiple choice** |
| **Contenido** | **100 % teórico**: *no* hay cálculos ni hay que programar |
| **Traer** | **DNI**, **lapicera**, **dos hojas** |
| **Prohibido** | **Celulares** y cualquier IA (ChatGPT, Gemini, etc.). "Que hayan estudiado y comprendan con sus palabras" |
| **Modelo de parcial** | **No hay** oficial. Se estudia lo visto (en §13 hay dos simulacros armados a partir de lo que dijo) |
| **Horario** | Arranca ~10–20 min después de la hora (el docente sabe que muchos vienen del trabajo) |
| **Duración** | No debería insumir más de **media hora** (dicho en la Clase 5) |
| **Mismo día** | Se rinde el **mismo día que Legislación** (se toman juntos para minimizar los viajes de quienes cursan a distancia) |
| **Recuperatorio** | **16 de octubre** |
| **Constancia de examen** | El docente la firma **después** del parcial (se pide en el Departamento de Alumnos / administración); también da el certificado de alumno regular |
| **Aviso** | Último mensaje por el campus: ver el recuadro **Último aviso del docente** más abajo |

> ⚠️ **Modalidad (aclaración):** el cronograma inicial de la cátedra figuraba como *"teórico y virtual"* y en la Clase 1 se dijo *"probablemente presencial (se confirma más cerca de la fecha)"; si fuera virtual, con cámara prendida y compartiendo pantalla*. En las Clases 4 y 5 el docente **confirmó: presencial, escrito a mano**. Vale lo último.

## 📩 Último aviso del docente (paro docente y marcha federal del 15/10)

> Mensaje enviado a las divisiones que cursan los viernes (resumido).

- Hay **paro docente convocado** en reclamo de **recomposición salarial** y contra el **ajuste del gobierno a la universidad pública**, rumbo a la **marcha federal del 15/10**.
- El docente **comparte el reclamo**, pero como sabe que muchos se organizaron para asistir de forma presencial en esta fecha, **mantiene el parcial**.
- **Lugar: aula 308.**
- **Recomendación de estudio:** repasar **los dos primeros capítulos de Chan, Badano y Rey**, **los apuntes de las clases**, **el código visto** y **realizar los ejercicios**.

> ⚠️ **Cómo leer la recomendación:** "el código visto" es para estudiar y entender los conceptos; no cambia lo que dijo antes (parcial **100 % teórico, sin programar ni calcular**). **Mapa de estudio:** capítulos 1 y 2 del libro → §1, §5, §6 y §7 de esta guía; apuntes de clase → toda la guía; código visto → §3 a §6 y los Colab (§11); ejercicios → §4.8 (EPH) y §7.6 (ejercicios del Cap. 2).

## ¿Qué temas entran?
- **Todo hasta la clase del 25/09 inclusive** → los **5 temas**: Clase 1 (conceptos), NumPy/Pandas, Data cleaning, Transformación de datos y Análisis estadístico (univariado, bivariado, multivariado). *(Su último aviso recomienda repasar los **dos primeros capítulos** del libro, los apuntes, el código visto y los ejercicios.)*
- **Fuentes que pueden entrar:** los **dos primeros capítulos** de *Chan, Badano y Rey* (~70–73 págs.), los **ejercicios**, los **colabs** y los **apuntes/presentaciones**.
- 🚫 **NO entra:** **visualización / gráficos** (Unidad 4), **análisis de componentes principales y de correspondencias** (están en el libro pero "no entran en la materia").

## Preguntas que mencionó explícitamente (las más probables)

| # | Pregunta / tema | Dónde lo dijo | Dónde está en esta guía |
|---|---|---|---|
| 1 | 🎯 **Relación / diferencias entre análisis de datos y minería de datos** (a **desarrollar**, "seguro") | 25/09 y 11/09 | §1.6 |
| 2 | 🎯 **Ciencia de datos vs. análisis de datos**: qué es cada una, diferencias, características | 11/09 | §1.4–1.6 |
| 3 | 🎯 **Cuadro de doble entrada** estadística vs. minería de datos | 25/09 | §1.6 |
| 4 | 🎯 **Big Data: las 3 V (+2)** — "tema de parcial de acá a la China" | Clase 1 | §1.5 |
| 5 | 🎯 **Tipos de variables** — "pregunta recontra de parcial… si la contestan mal, van directo al dos" | 25/09 | §1.7 |
| 6 | 🎯 **¿Por qué es tan importante NumPy?** / **características e importancia de `ndarray`** | 04/09 | §3 |
| 7 | 🎯 **Diferencia entre valor inconsistente y valor atípico** ("pregunta muy común de parcial") | 11/09 | §5.4 |
| 8 | 🎯 **¿Qué es el Z-score y para qué sirve?** (cuántos desvíos estándar se aleja un registro de la media; detecta atípicos) | 11/09 y 25/09 | §5.4 y §6 |
| 9 | 🎯 **¿Qué tipo de medida es la mediana?** → *pregunta trampa*: **tendencia central Y posición** | 25/09 | §7.3 |
| 10 | 🎯 **Interpretar una matriz de correlación** ("a lo sumo les voy a pedir eso") | 25/09 | §7.4 |
| 11 | 🎯 **Interpretar un boxplot** — lo dijo el 11/09, pero el 25/09 aclaró que **gráficos no entran** → repasarlo por las dudas | 11/09 | §5.4 y §7.3 |
| 12 | Ley de los grandes números vs. Teorema central del límite (se **confunden**) + **vínculo TCL ↔ test de hipótesis** (tarea) | Clase 1 | §2 |

## Lo que dijo que NO va a tomar
- Código / programar / cálculos / "qué hace tal función de NumPy".
- ❌ "Qué es un dato" y la definición de Wikipedia *(no es pregunta de parcial)*. ⚠️ Igual conviene manejar la idea: el dato aislado no sirve, hay que contextualizarlo.
- R, Cassandra/NoSQL (herramientas/curiosidades, no para tomar).


# 1. 🧠 Conceptos fundamentales del análisis de datos (Clase 1 + Cap. 1)

[⬆️ Volver al índice](#indice)

## 1.1 Dato
- Representación de un **hecho**, **observación** o **característica** de un objeto, persona o evento (números, texto, fecha, símbolos…).
- Por sí solo **carece de contexto y significado** para tomar decisiones. Ejemplos: `38.5`, `"Azul"`, `2026-08-04`, `125`, `"Juan Pérez"`.
- 🗣️ **"El dato no habla por sí solo, hay que contextualizarlo."** El análisis de datos consiste en **darle contexto y contar una historia** a partir de los datos; para eso hay que cumplir **una serie de pasos**.
- 🗣️ **"En el análisis de datos hay grises, no hay blanco y negro."** No hay respuestas mágicas; depende del contexto y del significado que se le dé.
- 🗣️ Los datos **no se estudian de forma aislada**: se trabaja con datos organizados de alguna manera.

## 1.2 Tipos de datos según su estructura

| Tipo | Qué es | Ejemplos |
|---|---|---|
| **Estructurados** | **Tablas**: filas y columnas. **Columnas = variables, filas = registros** | Tabla ID/Nombre/Edad/Ciudad, bases de datos relacionales |
| **Semiestructurados** | Cierta organización sin tabla rígida | **JSON, XML, CSV**, respuestas de **APIs**, **logs** |
| **No estructurados** | Sin formato de tabla | Texto, imágenes, video, audio, PDF, emails, redes sociales |

- 🗣️ Los **LLM** trabajan con datos **no estructurados** (el lenguaje lo es); lo mismo la IA de sonido, imagen y video.
- 🗣️ **Este cuatrimestre se trabaja principalmente con datos estructurados**; la IA está muy ligada a los no estructurados.

## 1.3 ¿De qué trata el análisis de datos? (el proceso)

```
Recolección → Limpieza → Transformación → Exploración y visualización → Interpretación → Conocimiento accionable
```

- **Recolección:** bases de datos, archivos, encuestas.
- **Conocimiento accionable:** toma de decisiones, resolución de problemas, respuestas a preguntas.
- 🗣️ **Quién recolecta:** en general **no es el analista** (los datos vienen de sensores, páginas web, encuestadores, bases existentes). **Excepción:** **web scraping** (ej.: extraer precio, kilómetros y modelo de una web de venta de autos).
- 🗣️ **Las etapas no son estrictamente secuenciales**: hay **ida y vuelta** (ej.: en la visualización se puede descubrir que la limpieza estuvo mal y volver atrás).
- 🗣️ Los datos **no tienen valor en sí mismos**: lo tienen por el **trabajo que se hace sobre ellos**.
- 📖 **Preparación de los datos (libro):** trabajar con bases masivas exige planificación. Hay que considerar: (1) los **objetivos reales** del análisis; (2) **recursos tecnológicos y de tiempo** disponibles; (3) **organización y estructuración** de los datos en bruto; (4) **costos** del estudio; (5) **interpretación y redacción de informes** accesibles para la toma de decisiones.

## 1.4 Definiciones de análisis de datos
- **Wikipedia:** proceso de **inspeccionar, limpiar y transformar** datos para **resaltar información útil**, **sugerir conclusiones** y **apoyar la toma de decisiones**.
- 🗣️ **No hay una sola forma de analizar datos**; fue cambiando mucho a lo largo de la historia.

**Perspectiva académica / tradicional** (estadística clásica; texto de Hernández, U. de La Rioja): reduce el análisis a estadística **descriptiva** o **inferencial**.
- **Descriptiva:** analiza **los datos disponibles** (asume que son todos). 🗣️ Ej.: media, máximo y mínimo de una variable.
- **Inferencial:** a partir de una **muestra** (recorte del universo) genera **predicciones/generalizaciones para el universo**. 🗣️ Ej.: encuestas de imagen de candidatos: se entrevistan 1.000–3.000 casos para inferir lo que piensa toda la población votante.

**En la actualidad:**
- Se usan técnicas que **exceden** la estadística tradicional: **aprendizaje automático** y **minería de datos**; 🗣️ por ejemplo **árboles de decisión, ensambles, redes neuronales** ("no es un capricho: funcionan").
- Cita (Chan, Badano y Rey): el **análisis descriptivo sigue siendo el paso inicial** recomendado para comprender la estructura de los datos.
- 🗣️ La estadística tradicional era "cuadrada y rígida"; se flexibilizó y **aparecieron la ciencia de datos, la IA y el machine learning** (campo más ligado a la informática).

## 1.5 Contexto histórico, Data Mining y Big Data

**Origen de la estadística** 🗣️: surge hacia el **3.er milenio a. C.** en el **Estado egipcio**; el nombre viene de **"dar cuenta de la situación del Estado"** (censos: situación económica, social, laboral). Disciplina de ~5.000 años; la minería de datos (siglo XIX) es "casi nueva".

**Por qué cambió el panorama** (desde los **años 90**):
- Desarrollo tecnológico: procesadores cada vez más potentes.
- **Explosión de datos** de aplicaciones web (gráfico w3resource): **Business Transaction Data** crece casi linealmente; **Web Application Data** crece **exponencialmente**.
- 📖 Volúmenes masivos actuales: transacciones, redes móviles, sensores, internet. La estadística tradicional resulta **limitada** ante su tamaño y complejidad → paradigma del *Data Mining*. (En la posguerra la estadística clásica vivió su "edad de oro".)
  - 📖 El aumento abarca datos **colectados, almacenados, accesibles y distribuidos**. Su origen: transacciones bancarias, reservas de aerolíneas, llamadas y mensajes por celular, registros de atención de pacientes, sensores remotos, operaciones con tarjeta de crédito, búsquedas en internet y compras en supermercados. Son **huellas o rastros** que dejamos en nuestro accionar cotidiano.
  - 📖 Hasta hace pocos años la **única estrategia** para extraer información útil de una base era la estadística clásica. La minería de datos responde al análisis de **gigantescas bases de cierta complejidad**, donde la estadística clásica resulta un recurso **limitado**.
  - 📖 **Ciclo del nuevo escenario:** almacenamiento de cantidades ingentes de información → tecnología capaz de trabajar con diversidad de datos → análisis en "tiempo real" del conjunto → (vuelve al almacenamiento).
- Procesar esos datos genera **ganancias** o **conclusiones científicas útiles** → hacen falta **nuevas herramientas y tecnologías**.

### Orígenes de la minería de datos 📖
Raíces en el análisis de datos de grandes pensadores que aplicaron la estadística clásica (siglo XIX):

- **Adolphe Quetelet (1796-1874, física social):** demostró que el **delito es un fenómeno social que puede conocerse y determinarse estadísticamente**: se comete año a año con **absoluta regularidad y precisión**. Posibles causas: pobreza, clima, miseria, analfabetismo. *(Datos sociales.)*
- **Francis Galton (1822-1911, ciencias humanísticas):** primero en aplicar métodos estadísticos al estudio de la **herencia de la inteligencia**. Creó el concepto estadístico de **correlación** y de **regresión hacia la media**, introdujo el uso de **cuestionarios y encuestas** para obtener datos de comunidades humanas y desarrolló estudios **genealógicos, biográficos y antropométricos**. *(Datos biológicos.)*
- **Ronald Fisher (1890-1962, agronomía y genética):** desde 1919 estadístico en la estación agrícola de **Rothamsted Research**, donde desarrolló el **análisis de la varianza** aplicado a datos de cultivos. Aportes a la genética de poblaciones: el **principio de Fisher**, el modelo de selección sexual ***runaway*** y la **hipótesis del hijo sexy**. *(Datos agronómicos.)*

> 📖 **Idea central del libro:** estas bases gigantescas nos llevan a preguntarnos **más que el *qué*, el *por qué*** de las cosas. **El valor de la información no reside en los datos concretos, sino en la forma de correlacionarlos** para descubrir patrones y estructuras ocultas. El desafío es **tolerar la imprecisión y la confusión** ("aceptar el desorden natural del mundo") a cambio de "un sentido más completo de la realidad". La herramienta para ello es la minería de datos.

### Data Mining (minería de datos)
- Forma parte del proceso **KDD** (*Knowledge Discovery in Databases*, "descubrimiento de conocimiento en bases de datos"). El *Data Mining* es su **fase analítica**.
- **Meta:** extraer información útil, **patrones y/o relaciones sistemáticas de valor y anomalías** de una gran base de datos **sin conocimiento previo** de lo que se busca. 📖 No solo importa *qué* pasa sino **por qué** pasa.
- 📖 **Naturaleza multidisciplinaria:** confluyen técnicas de **bases de datos y computación, aprendizaje automático, visualización, inteligencia artificial, estadística, aprendizaje de máquina (incluyendo redes neuronales) y procesamiento de imágenes**.
- 📖 Sus soluciones se basan en implementar, **mediante programación**, interfaces de uso general y **algoritmos propios** que permiten una **exploración y organización eficiente** de la información y apoyan la **identificación de regularidades** para quienes deben tomar decisiones.
- 🗣️ **"Sin conocimiento previo" = aproximación empírica y exploratoria**: se llega a los datos "con la cabeza vacía", sin marco teórico ni hipótesis; **no** se dice "mi hipótesis es esta, veamos si se valida".
- 🗣️ **Metáfora de la minería:** el minero excava una montaña y **separa lo útil/valioso de lo que no lo es** → la **limpieza** es parte obvia del proceso.
- 📖 **Dominios de aplicación:** análisis y procesamiento de **imágenes y señales**, análisis **multidimensional de procesos**, análisis de **datos textuales**, ***web mining***, **detección de fraudes** y **bioinformática**. Estos desafíos demandaron **herramientas específicas** y nuevo software para grandes cantidades de datos.

### Big Data 🎯
| V | Significado |
|---|---|
| **Volumen** | Grandes cantidades de información |
| **Velocidad** | Requiere alta velocidad de procesamiento |
| **Variedad** | Información en muchas formas |
| **Veracidad** | (adicional) confiabilidad |
| **Valor** | (adicional) utilidad |

- 🗣️ **¿Por qué Big Data no se define con un número** (ej. >100.000 TB)? Porque la capacidad de procesamiento **crece constantemente** y cualquier cifra queda chica (hace 50 años una computadora ocupaba una habitación; hoy un celular procesa mucho más; se discute la computación cuántica). Por eso se pasó a un **concepto**.
- 🗣️ Los conceptos "de moda" cambian: ciencia de datos → minería de datos → big data → **inteligencia artificial**; están muy relacionados y la disciplina está en **evolución permanente**.

### Terminología de conectividad 📖
El análisis de datos moderno se alimenta del hiper-conectivismo actual:
- **M2M (Machine to Machine):** intercambio de información o comunicación en formato de datos entre **dos máquinas remotas**, sin intervención humana. Facilita el **control de fraudes, la reducción de costos, el ahorro de tiempo y el monitoreo en tiempo real** del negocio. 📖 Usos: gestión de flotas, alarmas domésticas, contadores de agua/gas/electricidad, telemantenimiento de ascensores, estaciones meteorológicas, terminales punto de venta y máquinas *vending*.
- **IoT (Internet of Things):** interconexión digital de **objetos cotidianos** mediante internet (heladeras, *wearables* como gafas y relojes inteligentes, cámaras, sensores de movimiento, básculas y monitores de presión inalámbricos). Término acuñado en **1999** por el investigador británico **Kevin Ashton** (MIT, cofundador y director ejecutivo del **Centro de Auto-ID**, con sensores e identificadores de radiofrecuencia **RFID**). 📖 El primer dispositivo "conectado" fue una **máquina de Coca-Cola** en la Universidad Carnegie a principios de los años 80 (se consultaba por internet si había una bebida fría). Inicialmente designaba una conexión **más avanzada que el tradicional M2M**.
- **WoT (Web of Things):** **enfoques, estilos arquitectónicos de software y patrones de programación** que permiten que objetos del mundo real formen parte de la ***World Wide Web***. "Cosas" = objetos físicos, objetos etiquetados (códigos de barra), redes de sensores inalámbricos, máquinas y productos electrónicos de consumo. Proporciona una **capa de aplicación que simplifica la creación de aplicaciones de IoT**.
- **IoE (Internet of Everything):** conexión inteligente entre **la gente, los dispositivos, los datos en proceso y las cosas**; filosofía en la que el futuro de la tecnología se compone de muchos tipos de dispositivos conectados a internet global (millones de objetos con sensores que detectan y evalúan su estado, conectados por redes públicas o privadas con diversos protocolos). Según los expertos, **reinventará las industrias en tres niveles: proceso de negocio, modelo de negocio y momento de negocio**.

## 1.6 Análisis estadístico vs. Minería de datos 🎯 (cuadro clave)

| # | Análisis estadístico (clásica) | Minería de datos |
|---|---|---|
| 1 | Procedimiento **hipotético-deductivo** | Procedimiento **inductivo** |
| 2 | Técnicas **confirmatorias** | Técnicas **exploratorias** |
| 3 | **Con** supuestos iniciales | **Sin** supuestos iniciales |
| 4 | Herramientas informáticas **opcionales / de apoyo** | Recursos informáticos **indispensables / uso intensivo** |

**Explicación dada en clase 🗣️:**
- **Hipotético-deductivo:** se plantea una hipótesis y se **contrasta con la realidad**. **Inductivo:** se **generaliza** a partir de los datos, **sin hipótesis ni conocimiento previo**; "llegamos a los datos y vemos qué pasa".
  - Epistemología: hasta hace unos años el hipotético-deductivo estaba "bien visto" y el inductivo "mal visto"; con enormes volúmenes de datos **se volvió a necesitar el inductivo**.
  - Lo inductivo "hay que agarrarlo con pinzas": toda generalización puede terminar **falseándose**.
- **Confirmatorias vs. exploratorias:** la estadística busca **aceptar o rechazar** una hipótesis; la minería **no quiere aceptar ni rechazar nada, explora**. Obliga a **convivir con el error** (imágenes de IA que fallan, **alucinaciones**); el error **se reduce pero nunca se elimina**.
- **Supuestos iniciales** = *supuestos estadísticos* (no hipótesis): condiciones matemáticas que deben cumplirse (ej.: la variable debe ser **normal** para aplicar cierta regresión). Los modelos de ML/IA intentan **no requerirlos**. Con datos estructurados la estadística tradicional y el ML funcionan; **la gran diferencia de la minería está en los datos no estructurados**.
- **Informática:** en el siglo XIX la minería surgió sin recursos informáticos; hoy son **indispensables** por el **gran volumen de datos**.
- 🗣️ **IA actual e inducción:** los modelos actuales **generalizan** (inductivo) y **no aplican el método hipotético-deductivo**, aunque "traten de dibujarlo". La **IA general (AGI)** sería capaz de razonar como un humano con ese método.

> 💡 **Estadística = DEductivo, COnfirmatorio, CON supuestos, informática opcional. Minería = INductivo, EXploratorio, SIN supuestos, informática indispensable.**

> 📖 **Nota sobre la última fila:** la Tabla 1.1 del libro dice *"herramientas informáticas opcionales"* para la estadística y *"difusión entre especialistas en Computación"* para la minería de datos. En clase se explicó como **recursos informáticos indispensables / uso intensivo**. Para el parcial usá la formulación de clase y, si querés, mencioná la del libro.

## 1.7 Tipos de variables 🎯

| Tipo | Característica | Ejemplos |
|---|---|---|
| **Categóricas (cualitativas)** | **No** se pueden ordenar; modalidades sin orden jerárquico | Nombre, ciudad, color, sexo ("no puedo decir que Buenos Aires es más que Córdoba") |
| **Ordinales (cuasicuantitativas)** | **Sí** se ordenan, **no** se establece distancia exacta entre modalidades | Atención: muy buena / buena / regular / mala; calificaciones; estadios de una enfermedad |
| **Cuantitativas discretas** | Numéricas; **entre dos valores consecutivos no hay intermedios** (conteo) | Cantidad de hijos (no existe 1,5 hijos) |
| **Cuantitativas continuas** | Numéricas; entre dos valores hay **infinitos** intermedios (medición) | Distancias, peso, tiempo |

- 📖 **Escalas subjetivas:** medición analógica o visual de variables de nivel subjetivo (dolor, bienestar, agrado, acuerdo-desacuerdo). Ej.: una línea entre 0 y 10 que une "sin dolor" y "dolor intolerable". Sirven para evaluar la **progresión de un mismo individuo**, pero por su carácter subjetivo hay que tener cuidado al **comparar entre individuos**. Otro ejemplo: satisfacción de clientes antes y después de una mejora. El análisis suele basarse en **rangos de scores**.
- 📖 **Más ejemplos del libro:** categóricas (color de cabello, tipo de auto, sexo); ordinales (calificación de examen A–E, estadío de una enfermedad I–IV); discretas (cantidad de hijos, materias aprobadas, dinero en una billetera; toman un conjunto **a lo sumo numerable** de valores, ligado a contar); continuas (peso, edad, duración de un llamado; ligado a medir).
- 🗣️ Según el tipo **cambian los conteos, medidas y estimaciones aplicables** (como el operador `+` que concatena strings pero suma enteros).
- 🗣️ ⚠️ **Error grave en el TP final:** aplicar técnicas de variables cuantitativas a categóricas → **"motivo de ir a recuperatorio"**.

## 1.8 Clasificación según cantidad de variables

| Tipo | Descripción | Ejemplos |
|---|---|---|
| **Univariado** | Una variable a la vez. **Tendencia central** (media, mediana, moda), **dispersión** (varianza, rango), **otras** (curtosis) | Media de edad del aula |
| **Bivariado** | Dos variables: relación, dependencia | Correlación, covarianza, regresión edad–peso |
| **Multivariado** | Más de dos variables | Clusterización de clientes, regresión múltiple |

## 1.9 Tecnologías (la "pata tecnológica")

El análisis de datos tiene **una pata tecnológica y una pata estadística**.

- **SQL:** permite la **persistencia** de los datos; diseñado con criterio de **persistencia y consistencia** (ej.: cuenta bancaria).
- **Bases NoSQL:** otros criterios. En **redes sociales** importa la **velocidad**, no toda la información. Algunas subsisten aunque se pierda un nodo/data center; una base que priorice consistencia "se cae hasta que vuelva el nodo".
- **Bases columnares (ej.: Cassandra) 🗣️:** SQL organiza por **filas**; las **columnares trabajan columna por columna**, criterio más útil para análisis de datos.
- **R:** lenguaje **especializado en análisis de datos** (enfoque estadístico); el libro usa ejemplos en R.
- **Python 🗣️:** fundado por **Guido van Rossum en 1989**. Filosofía: **legible y accesible** ("un programador pasa más tiempo leyendo que escribiendo código"). **Multiparadigma** (OO, funcional).
  - En los 90 era criticado (predominaban lenguajes muy optimizados). En 2000 ni aparecía en el ranking; ~2015 era 3.º (R 10.º); C cae. Alrededor de **2017** aparece el paper **"Attention Is All You Need"** → explota la IA y Python sube; hoy es **el lenguaje más usado** y **el de la IA y las redes neuronales**. R queda desplazado.
  - **NumPy** fue "la razón por la que Python es lo que es".
- 📖 **Otras herramientas (libro):** **WEKA** (colección de algoritmos en Java), SAS Enterprise Miner, Statistica Data Miner, SPSS Clementine (IBM), IBM Intelligent Miner, SPAD, SODAS. *Contexto actual:* computación en la nube (AWS, Google Cloud, Azure) y ecosistemas de Big Data como Apache Spark o Hadoop (procesamiento distribuido en tiempo real).
  - 📖 **Detalle del software de minería de datos citado en el libro:**
    - **SAS Enterprise Miner** (SAS Corporation, Cary, Carolina del Norte): modelos predictivos y descriptivos para grandes volúmenes de datos.
    - **R:** entorno y lenguaje libre de enfoque estadístico, nacido como reimplementación libre del lenguaje **S**. **Python:** lenguaje interpretado de sintaxis legible y **multiparadigma** (objetos, imperativa, funcional).
    - **Statistica Data Miner** (Dell): paquetes para manipulación y análisis de datos. **SPSS Clementine** (IBM): análisis de texto y minería de datos con **interfaz visual, sin programar**.
    - **ISL Decision Systems** (datos → decisiones de negocio: fraude, fidelidad de clientela, ventas, audiencia televisiva). **Salford Systems** (aprendizaje por máquina para modelos predictivos). **MineSet** (Silicon Graphics: analizar, minar y visualizar datos).
    - **WEKA** (libre, Java, algoritmos de aprendizaje de máquina). **SODAS** (*Symbolic Official Data Analysis System*: cada método es un ícono enlazado en cadena). **IBM Intelligent Miner** (modelado, evaluación y visualización). **SPAD** (*Système Portable pour l'Analyse de Données*: tratamiento exploratorio multivariado de grandes tablas). **T (Textual)** aplicado a datos simbólicos.
- Librerías del ecosistema Python: **Pandas, NumPy, Matplotlib/Seaborn** (gráficos), **TensorFlow, PyTorch** (deep learning), **scipy** (medidas estadísticas avanzadas).
- **Herramienta de la cursada 🗣️:** **Google Colab** (en la nube, notebooks con **Python + Markdown**). Hay que **"Guardar una copia en Drive"** para editar. En el TP se puede usar cualquier lenguaje/entorno.

---

# 2. 📐 Conceptos estadísticos fundamentales

[⬆️ Volver al índice](#indice)

## 2.1 Ley de los grandes números (LGN) 🎯
- **Jacob Bernoulli, siglo XVII.**
- La **frecuencia relativa** de un evento **converge a su probabilidad teórica** al **aumentar el número de ensayos**.
- En inferencia: al crecer la **muestra**, la **media muestral** se aproxima a la **esperanza (valor esperado) poblacional**.

**Lecturas del docente 🗣️:**
- **No se pueden sacar conclusiones definitivas de fenómenos masivos a partir de casos aislados** (velocidad promedio del ser humano ≠ velocidad de atletas olímpicos; hay que armar una muestra **representativa**).
- **Cuanto más grande la muestra, mejores las estimaciones**.
- Vínculo con IA: el salto de **GPT-2 a GPT-3** fue el **volumen de datos** de entrenamiento; "**a pequeña escala la IA no funciona**".
- Aplicación en clase (04/09): repetir el experimento lista vs. NumPy muchas veces y **promediar**.

## 2.2 Teorema central del límite (TCL) 🎯
- Desarrollado entre los **siglos XVIII y XIX**; reformulado **hasta el XX**.
- Dada una población con **cualquier distribución**, la **distribución de las medias muestrales tiende a una normal** al aumentar el tamaño de la muestra, **siempre que la varianza poblacional sea finita**.

**Ejemplo del docente 🗣️ (semillas, Fisher):** se compara una semilla original con una modificada genéticamente. Se toman muestras, se estima la **media de producción (toneladas)** de cada una y esas medias siguen una distribución normal. Como se conocen las propiedades de la normal, se **testea si una semilla rinde mejor que otra** usando media, desvío estándar y el **rechazo de la hipótesis nula**. Si las curvas están muy separadas se ve a simple vista; si se solapan no se puede afirmar.

| | Ley de los grandes números | Teorema central del límite |
|---|---|---|
| **Época** | Bernoulli, s. XVII | s. XVIII–XIX (reformulado hasta el XX) |
| **Dice** | La media muestral **se acerca** al valor esperado | La **distribución** de las medias muestrales **tiende a la normal** |
| **Condición** | Más ensayos / muestra más grande | Muestra grande + **varianza poblacional finita** |
| **Idea** | "**A dónde va** el número" | "**Qué forma tiene**" (campana) |

> 🎯 El docente advirtió que **se confunden ambos conceptos** en los exámenes. **Tarea:** investigar **(1)** qué es la LGN y **(2)** el **vínculo entre el TCL y el test de hipótesis**.

## 2.3 Relación entre el TCL y el test de hipótesis 🎯

> ⚠️ Desarrollo de la consigna que dejó el docente para investigar (no dictado textualmente en clase).

- El **test de hipótesis** necesita conocer **qué forma tiene la distribución de un estadístico** (por ejemplo, la media muestral) para poder calcular probabilidades y decidir si un resultado es "raro" o no.
- El **TCL garantiza esa forma**: sin importar cómo se distribuya la población original, la distribución de las medias muestrales se aproxima a una **normal** a medida que crece el tamaño de muestra (*n*).

**Cómo funciona el mecanismo (ejemplo de las semillas):**

1. Se plantea una **hipótesis nula (H₀)**, por ejemplo: "las dos semillas rinden igual".
2. Gracias al TCL, la media muestral sigue (aproximadamente) una normal → se puede calcular su desvío estándar (**error estándar**) y ubicar el resultado observado dentro de esa curva.
3. Se calcula qué tan probable es obtener la diferencia observada (o una más extrema) **si H₀ fuera cierta** → esto es el **p-valor**.
4. Si esa probabilidad es muy baja (por debajo de un umbral, típicamente **0,05**), se **rechaza H₀**: la diferencia es **estadísticamente significativa** y no se explica solo por azar muestral.

> **Idea clave:** no alcanza con comparar dos medias "a ojo". El TCL permite construir la distribución esperada de esas medias **bajo el supuesto de que no hay diferencia real**, y sobre esa normal se decide si la diferencia observada es lo bastante grande como para no ser producto del azar. Sin el TCL no habría base teórica para saber qué distribución usar. Es el fundamento de la mayoría de los tests paramétricos (**test t, test z, ANOVA**, etc.).

---

# 3. 🔢 NumPy — manipulación eficiente de vectores

[⬆️ Volver al índice](#indice)

> 🎯 **Pregunta de parcial:** *¿por qué es tan importante NumPy? ¿Cuáles son las características y la importancia de `ndarray`?* (**No** toma funciones de memoria ni código; sí la **importancia conceptual**).

## 3.1 ¿Qué es?
**NumPy = Numerical Python.** Sirve sobre todo para variables **cuantitativas** (discretas y continuas), pero **optimiza** los procedimientos más allá de lo numérico.

**Características generales:**
- Desarrollada en **C** (lenguaje de **bajo nivel**), orientada a **arrays multidimensionales** y gran cantidad de información.
- Recursos para **matemática, álgebra lineal** y diversas disciplinas científicas.
- **Código abierto**, **multiplataforma**, **optimizada**, **sintaxis de alto nivel**.

**¿Por qué importa que esté en C? 🗣️**
- C es **tipado y compilado** y permite **manipular la memoria** con mucha más precisión (Python, de alto nivel, no).
- Resultado: operaciones matemáticas y algebraicas **más veloces y optimizadas** con grandes volúmenes.
- Las **dos ventajas** que se buscan en informática: **mayor velocidad** y **menor espacio en memoria** (relacionadas pero distintas).

**Casos de uso:** Big Data, estadística avanzada, álgebra lineal, procesamiento del lenguaje natural, procesamiento de imágenes.

**Ecosistema 🗣️ (todas usan NumPy "por detrás"):** computación cuántica, **Pandas**, procesamiento de señales, imágenes, **grafos y redes (NetworkX)**, astronomía, psicología cognitiva, bioinformática, inferencia bayesiana, análisis matemático, química, geografía, arquitectura, ingeniería. **Deep learning/ML: TensorFlow y PyTorch**.
**Casos de estudio:** primeras imágenes de **agujeros negros**, **ondas gravitacionales**, análisis deportivo, posiciones de animales con aprendizaje profundo.

> 💡 Aunque uses Pandas y no NumPy directamente, **NumPy sienta las bases**.

## 3.2 La clase `numpy.ndarray` 🎯
**Principal clase** y **base de todas las operaciones matemáticas numéricas** de NumPy.

| Lista de Python | `ndarray` |
|---|---|
| **Mutable y heterogénea**: se puede cambiar un entero por un flotante, tupla, set o lista → hay que reservar espacio de más | **Tamaño fijo** una vez instanciado |
| Creada priorizando **legibilidad** (la optimización quedó en segundo plano) | **Todos los elementos del mismo tipo** (y tamaño) |
| Puede recorrer memoria innecesariamente por posibles cambios futuros | Memoria **contigua** y reservada **estrictamente** para esos elementos |
| — | Excepción: un **vector de objetos** permite distinto tipo/tamaño |

- 🗣️ `ndarray` es un **"parche"** a un problema de Python: combina **lo mejor de dos mundos** (alto nivel legible + ventajas del bajo nivel de C).
- **Facilita operaciones matemáticas avanzadas** y es **ampliamente usada por otros paquetes**.

## 3.3 Atributos y métodos

| Atributo | Devuelve |
|---|---|
| `ndim` | Nº de **dimensiones** (fijo) |
| `shape` | **Tupla** con elementos por dimensión |
| `dtype` | **Tipo de datos** (ej. `int64`) |
| `size` | **Cantidad total** de elementos |
| `itemsize` | **Bytes** por elemento |
| `data` | El **buffer** con los elementos |
| `T` | **Transpuesta** |

| Método / función | Qué hace |
|---|---|
| `flatten()` | Pasa a **una dimensión** |
| `reshape()` | **Cambia la forma** |
| `sum()`, `mean()`, `std()` | Suma, media, desvío estándar |
| `zeros()`, `ones()`, `empty()` | Arrays de ceros, unos, valores sin inicializar |
| `arange()` | Como `range()` pero **permite decimales** |
| `linspace()` | **Intervalos regulares** |
| `sort()` | Ordena (ascendente por defecto) |
| `concatenate()`, `expand_dims()` | Concatenar, agregar dimensiones |

🗣️ **Para qué sirve `flatten`:** trabajar en **una dimensión es más veloz**; muchos algoritmos de IA **apilan las columnas de una matriz** en un vector. `reshape`/`flatten` cambian el tamaño **sin "barbaridades" en memoria**.

> ⚠️ `empty()` no inicializa: contiene "basura" de memoria. Por convención `import numpy as np`.

## 3.4 Experimento de la clase 🗣 (lista vs. NumPy)
- Elevar al cuadrado **1.000.000 de elementos**: lista ≈ **0,0457 s** vs. NumPy ≈ **0,0013 s** → **≈ 32,8 veces más rápido** (otras corridas: 27×, 85×; en Colab ~**50×**).
- **Conclusiones:** (1) NumPy **es más rápido**; (2) **LGN**: con más corridas el promedio se acerca a la diferencia real; (3) **TCL**: la distribución de los resultados tendría **forma de campana**.
- **Consignas de clase:** (1) repetir el experimento y **promediar los resultados de todo el grupo** para ver cómo el promedio se acerca a la diferencia real (LGN); (2) **graficar la densidad** de los resultados y comprobar si se aproxima a una **campana de Gauss** (TCL).
- **Memoria:** para 10.000 elementos, la lista ≈ **360.056 bytes** y el array ≈ **80.000 bytes** (`int64`, 8 bytes × 10.000).

## 3.5 Imágenes como arrays 🗣
- **Blanco y negro:** una sola **matriz**. **Color:** **tres matrices** superpuestas (**RGB**); ej.: amarillo = rojo + verde. Una imagen de 5×5 = 25 píxeles.
- Por eso NumPy es clave en **procesamiento de imágenes**; la IA que genera imágenes **opera matemáticamente con matrices**.

---

# 4. 🐼 Pandas — análisis de datos estructurados

[⬆️ Volver al índice](#indice)

## 4.1 ¿Qué es?
- Librería para **DataFrames** (estructuras tabulares). Creada por **Wes McKinney** (2008), autor de *Python para análisis de datos* (bibliografía obligatoria).
- 🗣️ Intentó **imitar a R**. Trabaja con **datos estructurados**. **Usa `ndarray`** de NumPy para las variables numéricas.
- **Código abierto, multiplataforma, optimizada, sintaxis de alto nivel.**
- 🗣️ Maneja también variables **ordinales, fechas y texto**, y permite **unir tablas**. Convención: `import pandas as pd`.

**Funciones más usadas:** `read_csv()`, `read_excel()`, `read_json()`, `DataFrame()`, `to_datetime()`, `merge()`.

## 4.2 Estructuras básicas

| Estructura | Descripción |
|---|---|
| **Series** | Vector **unidimensional etiquetado**, de cualquier tipo, basado en `ndarray` |
| **DataFrame** | Estructura **bidimensional** (tabla), construida sobre Series |

🗣️ **Series = dos vectores 1D en paralelo:** **valores** (usa `ndarray`) y **etiquetas/índice** (tipo `Index`, propio de Pandas, **no** ndarray).

- **Atributos de Series:** `index`, `values`, `name` (opcional), `is_unique` + la mayoría de los de ndarray (**no** `data`, `itemsize`, `strides`).
- **Métodos de Series:** casi todos los de ndarray (**excepto `flatten` y `reshape`**) + `head()`, `describe()`, `dropna()`, `apply()`…
- 🗣️ **¿Por qué no `flatten`/`reshape`?** No se pueden unificar **etiquetas con valores** ni **columnas de distinto tipo**; estadísticamente **no es correcto** porque el tratamiento de una variable cualitativa, ordinal o cuantitativa **es distinto**.
- 🗣️ `describe()` devuelve: **conteo, media, desvío estándar, mínimo, Q1, mediana, Q3, máximo**.
- **Atributos de DataFrame:** `shape`, `columns`, `dtypes` (🗣️ tipo de las **columnas**; texto y diccionarios figuran como **`object`**). **Métodos:** `to_csv()`, `to_excel()`, `head()`, `info()`, `groupby()`.

## 4.3 Selección de columnas

| Por **nombre** | Por **posición** (`iloc`) |
|---|---|
| `df.id` o `df["id"]` | `df.iloc[:, 1]` |
| `df[["id", "damage"]]` | `df.iloc[:, 1:4]` |

## 4.4 Filtrado de filas

| Por posición | Según condiciones |
|---|---|
| `df.iloc[2, :]` | `df.loc[df.damage == 3, ["id","damage"]]` |
| | `df.query("damage > 2")` (🗣️ estilo **SQL**) |

- 🗣️ **A la izquierda las filas, a la derecha las columnas.** `:` = "todas".
- ⚠️ Python cuenta desde **0** y el final del rango **no se incluye**: `iloc[:,1]` es la **2.ª** columna; `iloc[:,1:4]` son las posiciones 1, 2 y 3; `iloc[2,:]` es la **3.ª** fila.

## 4.5 Índices: `loc` vs `iloc`
- Los **índices simplifican el acceso** y permiten **filtrar** (ej.: si el análisis es sobre Avellaneda, no sirven datos de Lanús, Tigre o La Matanza).
- **`loc` = nombres/etiquetas · `iloc` = posiciones numéricas.**

## 4.6 Fechas y texto
- `pd.to_datetime()` + accesor **`dt`** → año, mes, día.
- Accesor **`str`** → `lower()`, `upper()`, `split()`, `replace()`, `splice()`\*…
  > ⚠️ \*La diapositiva dice `splice()`; probablemente sea un error tipográfico de `strip()`.

## 4.7 Datos usados en clase 🗣
- **Kaggle** (y `kagglehub`): comunidad de IA y ML con **~734.000 datasets**, notebooks, modelos preentrenados y **competencias** con premios (algoritmos de Netflix salieron de competencias así).
- Dataset de **League of Legends** (ID, nombre, título, dificultad, daño, etc.). Otras librerías con datasets: Keras.
- 📖 El libro usa datasets de R como `iris` y `mtcars` (ver códigos en §5–§7).

## 4.8 Ejercicio de la Clase 2: base de microdatos de la EPH 🗣
**Consigna (PDF de ejercicios):**
1. Abrir con Pandas la base de microdatos de la **Encuesta Permanente de Hogares (EPH, INDEC), 3.er trimestre de 2024** ([descarga: EPH_usu_3_Trim_2024_txt.zip](https://www.indec.gob.ar/ftp/cuadros/menusuperior/eph/EPH_usu_3_Trim_2024_txt.zip)).
2. Analizar el DataFrame y responder: ¿cuántas **columnas** tiene? ¿cuántas **filas**? ¿qué **tipos** de columnas tiene?
3. ¿Se puede detectar alguna **columna índice**?

- El zip trae dos archivos: `usu_hogar_T324.txt` y `usu_individual_T324.txt`.
- **Objetivo:** empezar a observar el dataset con el que se trabaja en el **TP final**. Los ejercicios de cada clase se retoman al principio de la clase siguiente.

---

# 5. 🧹 Data cleaning — limpieza y preparación

[⬆️ Volver al índice](#indice)

> **Data cleaning = paso previo al análisis.**

## 5.1 Contexto (ETL) y etapas 🗣
- Proceso **ETL**: **cargar, transformar y volver a guardar** los datos.
- Etapas: **1** Recolección → **2** Almacenamiento → **3 Limpieza y preprocesamiento** → **4** Análisis → **5** Visualización y/o modelado. 💡 **RALAV**.
- 🗣️ El analista normalmente **empieza en la etapa 3**, pero **las etapas están interconectadas**.
- 🗣️ Los datos reales **tienen problemas**. Los **atípicos/inconsistentes** no dan indicio previo (en el 99 % de los casos parecen normales).
- **Trabajo del analista:** **detectar** los problemas, **identificar qué sucede** y, si corresponde, **plantear una solución**.

**Problemas más comunes:** **valores nulos, duplicados y atípicos/inconsistentes.**

## 5.2 Valores duplicados
- **Problema:** **sobrerrepresentación** → **conclusiones sesgadas**. **Solución:** dejar **uno solo** → `df.drop_duplicates()`.
- 🗣️ **Ojo con los "grises"** (ejemplo: DataFrame con ID, nombre y localidad; 7 registros; 2 repetidos):
  - **Juan** con el **mismo ID** pero distinta localidad (¿doble carga o persona distinta?).
  - **María** en la misma localidad: puede haber **dos personas distintas**.
  - **Consultar a quien hizo el relevamiento**; si no, **definir un criterio** (por **ID**, o por **nombre + localidad**). En pandas se eligen la/s columna/s.

## 5.3 Valores perdidos o "no respuesta" (datos faltantes)
- 🗣️ **No respuesta parcial:** registros con **campos vacíos**. Problema **subestimado**, sobre todo en **encuestas de opinión pública** y en la inferencia tradicional; en ML/modelado sí se le presta atención.
- 📖 En R se marcan como `NA`. En el análisis **univariado** los faltantes simplemente se omiten; en el **multivariado**, **un solo dato faltante puede obligar a descartar toda la fila**, reduciendo mucho el tamaño muestral.
- Puede llevar a **conclusiones incorrectas** con tasa de no respuesta alta. 🗣️ **Umbrales orientativos:**

| Tasa de no respuesta | Nivel |
|---|---|
| **> 5 %** | Empezar a tenerla en cuenta |
| **> 10 %** | Importante |
| **> 30 %** | **Grave** (a veces se descarta la variable) |

💡 **5 – 10 – 30**. Lo clave es **detectar el patrón**.

### Patrones de la no respuesta

| ¿Se puede soslayar? | Patrón | Descripción |
|---|---|---|
| ✅ Sí | **Completamente aleatoria** | Sin patrón ni asociación con otras variables. **No introduce sesgo** |
| ❌ No | **Aleatoria** | Hay azar, pero **condicionada por otras variables** del dataset |
| ❌ No | **No aleatoria** | La no respuesta se explica **por la propia variable** de interés |

**Ejemplos 🗣️ (sensor de temperatura):**
- **Completamente aleatoria:** el sensor manda datos por 4G/5G y a veces se cae la señal.
- **Aleatoria:** falla más con **humedad** (relacionada con la temperatura) → **temperatura media subestimada**.
- **No aleatoria:** falla cuando **sube la temperatura** (la propia variable).

**Ejemplo numérico 🗣️ ("semáforo"):** encuesta de **1.000 casos**, **200 no respuestas** = **20 %**. Ingreso medio por grupo etario: 16–25: **$500.000**; 26–40: **$800.000**; 40–65: **$1.200.000**; 65+: **$1.100.000**.

| Semáforo | Escenario | No respuesta por grupo etario | Lectura |
|---|---|---|---|
| 🟢 **Verde** | Completamente aleatoria | 19 % · 20,5 % · 18,8 % · 20,3 % (≈20 %; se podría hacer un chi-cuadrado) | Sin sesgo claro |
| 🟡 **Amarillo** | **Aleatoria** (asociada a la **edad**) | 15 % · 18 % · 23 % · 30 % | Faltan justamente ingresos altos → **media de ingreso sesgada hacia abajo**. Hay que **tratarla** |
| 🔴 **Rojo** | **No aleatoria** (asociada al **ingreso**) | Mayor no respuesta en el grupo de mayor ingreso (40–65) | **Problema circular:** la causa de la no respuesta es lo que quiero estimar |

- 🗣️ **Clave:** en la **aleatoria** puedo **apoyarme en otras variables** para corregir; en la **no aleatoria** no.
- 🗣️ **No hay técnica infalible** que diga el patrón: es una **definición conceptual del analista**. Los nombres "aleatoria / no aleatoria" no son los mejores (hay azar en ambos); "no aleatoria" alude a que **depende de sí misma**.
- 🗣️ Hay que ver **las variables del dataset y la variable objetivo**, no solo grupos artificiales.
- 🗣️ **Supuesto del muestreo:** casos con características semejantes **tienden a comportarse parecido** (dos personas de Puerto Madero se parecen más entre sí que con uno de Florencio Varela).

### Tratamientos

| Caso | Solución |
|---|---|
| **Completamente aleatoria** | **Eliminar** registros → `df.dropna()` |
| **Aleatoria o no aleatoria** | Depende de tasa y características: **imputación**, **reponderación**, modelos |

**Alternativas complementarias ➕** *(el PDF del libro no incluye una sección de datos faltantes; esto viene de las continuaciones de texto):*
1. **Listwise deletion (eliminación por casos):** borrar la fila; recomendable solo si la proporción de individuos con faltantes es muy baja (p. ej. < 5 %).
2. **Imputación por media/mediana:** simple, pero **subestima la varianza y altera las covarianzas**.
3. **Imputación múltiple y métodos basados en modelos:** K-vecinos más cercanos, máxima verosimilitud, etc.

```r
# Ejemplo complementario ➕ (el Código 2.19 del libro es otro: gráfico de control multivariado)
library(mice)
colSums(is.na(mis_datos))                     # faltantes por variable
datos_completos <- na.omit(mis_datos)         # listwise deletion
datos_imputados <- mice(mis_datos, m = 5, method = "pmm", seed = 123)
base_final <- complete(datos_imputados)
```

**Técnicas de imputación 🗣️:**
- **Medias condicionadas** (la más **básica**): armar **grupos**, calcular la media de cada uno y **asignarla**.
- **Modelos de aprendizaje automático:** predecir con **muchas variables** (edad, sexo, nivel educativo, localidad, ocupación…).
- **Hot deck:** buscar otro caso con **las mismas características exactas** en algunas variables y **elegir uno al azar**. Las variables usadas deben **estar relacionadas con la variable a imputar** (para ingreso sirven **ocupación** y **nivel educativo**; el **apellido** no).
- **Reponderación** (ver ponderadores).

### Ponderadores 🗣 (se usan en el TP final)
- **Ponderador = cuántos casos de la población representa cada elemento muestral = población / muestra.**

| Grupo | Población | Muestra | Ponderador |
|---|---|---|---|
| 1 | 1.000.000 | 200 | **5.000** |
| 2 | 900.000 | 190 | ≈ **4.737** |
| 3 | 800.000 | 210 | ≈ **3.810** |
| 4 | 500.000 | 195 | ≈ **2.564** |
| 5 | 300.000 | 205 | ≈ **1.463** |

- **Estimaciones más precisas:** en el grupo de **menor ponderador** (universo más chico; un atípico mueve menos). No depende solo de la LGN sino del **tamaño del universo**.
- **Reponderación:** con 10 % de no respuesta, los 200 casos pasan a **180** y deben representar **todo el universo** → ponderador **1.000.000 / 180 ≈ 5.555**. Se ajustan para que los **respondentes representen también a los no respondentes**.
- Se puede complejizar: subdividir por sexo y edad (8 × 5 = **40 ponderadores**); el INDEC usa **muestreo complejo polietápico** (ponderador = producto de probabilidades de selección de cada etapa).
- **EPH** (microdatos del TP): trae **varios ponderadores**; hay que saber **cuándo usar cada uno**.

**Conclusión:** **decisión metodológica** del analista, sencilla o compleja según objetivos y características de la no respuesta. **No hay respuesta automática.**

## 5.4 Valores atípicos (outliers) e inconsistentes 🎯

| | **Atípico** | **Inconsistente** |
|---|---|---|
| **Definición** | Dato **alejado del patrón general**, pero **posible/válido** | Dato **sin coherencia** con el conjunto o con el conocimiento previo |
| **Tratamiento** | **No necesariamente** se excluye ni modifica; se **inspecciona** y depende del **objetivo** | **Se corrige o se elimina**; **nunca** se usa |
| **Ejemplos** | Persona de **105 años**; propiedad en Avellaneda **cerca del río**; salario del **jugador mejor pago del fútbol argentino** | Persona de **250 años**; punto **fuera del territorio** de análisis; valor de **tipo distinto** |

**Ejemplos en clase 🗣️:**
- **250 años:** probablemente error de carga (un cero de más); distorsiona la media.
- **Mapa (Properati):** análisis de **Avellaneda**. **Inconsistentes:** puntos en CABA, La Matanza, Lanús (mal cargados) → **se excluyen**. **Atípicos:** puntos **dentro** de Avellaneda cerca del río, alejados de la masa; válidos, se decide según el objetivo.
- **Depende del objetivo:** el salario de un futbolista de élite no sirve para estimar cuánto pedir en una entrevista, pero **sí** para un **estudio de mercado de alta gama**.
- 105 años: no es común pero **es posible**.

> 💡 **Atípico = raro pero posible (se analiza). Inconsistente = imposible o incoherente (se corrige o se borra).**

### ¿Cómo detectar atípicos?
1. **Boxplot** (univariado) 🗣️: los atípicos aparecen como **puntos alejados de la caja**.
2. **Z-score** 🎯: **cuántos desvíos estándar se aleja cada registro de la media**. *Mayor Z-score = más atípico*. Ej.: edad media **46,9**, desvío **23,4** → la persona de 100 años tiene **Z ≈ 2,38**. 📖 **Regla de los tres desvíos:** para $t_i = (x_i - \bar{x})/s$, como en una normal es muy baja la probabilidad $P(|Z| > 3)$, se señala como outlier a los valores con $|t_i| > 3$.
3. **Rango intercuartílico (IQR):** **Q3 − Q1**, la caja del boxplot.
4. **Aprendizaje automático.**

#### 📖 Detalle del boxplot (libro)
La caja se construye con los cuartiles y permite evaluar:
1. **Tendencia central:** la línea dentro de la caja es la **mediana (Q2)**.
2. **Dispersión:** la altura de la caja es el **RI = Q3 − Q1**.
3. **Asimetría:** si la mediana está centrada o desplazada, y el largo relativo de los bigotes.
4. **Atípicos:** los bigotes llegan al mínimo y máximo que **no superen 1,5 × RI**; lo que excede se grafica como punto individual.

```r
# Ejemplo complementario ➕ (el Código 2.9 del libro es otro: boxplot comparativo de laboratorios con ggplot2)
boxplot(iris$Sepal.Length ~ iris$Species,
        main = "Longitud del sépalo según Especie",
        xlab = "Especie", ylab = "Longitud del sépalo",
        col = c("palegreen1", "paleturquoise", "plum2"), border = "gray30")
```

📖 **Más del libro sobre el boxplot (Tukey, 1915-2000):** se dibuja una **caja** entre el primer y tercer cuartil con la **mediana** adentro; los **bigotes** llegan hasta el dato más alejado que esté **a lo sumo a 1,5 × RI** del extremo de la caja. Se llama **outlier moderado** al dato a más de **1,5 × RI** y menos de **3 × RI** de la caja, y **outlier severo** al que está a más de **3 × RI**. Sirve para apreciar **posición, dispersión, asimetría y puntos anómalos**, y es especialmente útil para **comparar varios conjuntos**.

**Cómo leer la asimetría en el boxplot:** simétrica → mediana en el centro de la caja y bigotes de largo similar. Asimetría **positiva (a derecha)** → mediana más cerca de Q1 y/o bigote inferior más corto; es probable que aparezcan atípicos altos. Asimetría **negativa (a izquierda)** → situación inversa.

**Ejemplo 2.8 del libro (n = 13):** datos {14, 18, 24, 26, 35, 39, 43, 45, 56, 62, 68, 92, 198}. Mediana = 43, Q1 = 25, Q3 = 65, RI = 40. Límites: Q3 + 1,5·RI = **125** y Q1 − 1,5·RI = **−35**. Valor adyacente superior = **92** (mayor dato menor que 125) y adyacente inferior = **14**. Como 198 > Q3 + 3·RI = **185**, es un **outlier severo**.

**Cómo tratar los outliers (libro):** deben **inspeccionarse con cuidado**. Si **no hay evidencia de error y su valor es posible, no deben eliminarse**: pueden alertar de anomalías de un tratamiento o patología, grupos especiales de clientes, etc. Su presencia puede indicar que **la escala elegida no es la adecuada**. Con varios outliers su influencia puede **enmascararse** (se compensa el efecto de unos con otros). Con outliers conviene usar **medidas robustas**, porque la media y la varianza son buenos resúmenes solo cuando no los hay.

**Ejemplo 2.9 (boxplots comparativos):** siete laboratorios miden el contenido calórico de un alimento cuyo valor verdadero es **4 kcal**. Conclusiones del libro: los laboratorios **1 y 3** son los más precisos; el **3 y el 6** presentan atípicos altos; todos salvo el 1 y el 3 muestran asimetría; el laboratorio **2** tiene asimetría negativa y el **7** positiva en los valores centrales. **Se elegiría el laboratorio 1**, porque entre los de mediana próxima al valor verdadero es el más preciso (menor amplitud de la caja).

> ⚠️ La interpretación del boxplot fue mencionada el 11/09 como pregunta habitual, pero el 25/09 dijo que **gráficos no entran**. Por las dudas, sabé qué es la caja, los cuartiles y los puntos atípicos.

### 📖 Estadística robusta en dimensión múltiple (libro, Cap. 2)
Las medidas clásicas (media, varianza, covarianza de Pearson) son **muy sensibles a atípicos**; en varias dimensiones son difíciles de detectar y provocan:
1. **Enmascaramiento (*masking*):** un grupo de outliers distorsiona tanto el centroide y la matriz de covarianza que **esconde a otros outliers** verdaderos (solo se revelan al eliminar los primeros).
2. **Inundación (*swamping*):** las estimaciones distorsionadas hacen que **observaciones normales parezcan outliers**. 📖 En el libro: una observación es outlier **solo en presencia de otras**; si se quitaran, dejaría de serlo.

**Herramientas robustas:**
- **Distancia de Mahalanobis:** a diferencia de la euclídea, **pondera por la matriz de covarianzas** (se ajusta a la forma y correlación de la nube de puntos); mide la lejanía respecto al centro.

  $$d_m(X, Y) = \sqrt{(X - Y)^t \, \Sigma^{-1} \, (X - Y)}$$

- **Vector de medianas:** reemplazo robusto del vector de medias (centroide). 📖 Propuesta de la bibliografía: sustituir el vector de medias por el de medianas y calcular la matriz de covarianza con las **k observaciones de menor distancia de Mahalanobis** a ese vector. Estimar robustamente Σ equivale a **estimar la covarianza de una buena parte de los datos**.
- **MVE (Minimum Volume Ellipsoid):** busca el **elipsoide de menor volumen** que cubra *m* de las *n* observaciones (ej. $m = n/2$); se calcula por **remuestreo**. 📖 Es **eficiente, equivariante ante transformaciones afines, de bajo sesgo y con alto punto de ruptura**, por lo que sirve para detectar atípicos multivariados.
- **MCD (Minimum Covariance Determinant):** busca el subconjunto de tamaño $m$ (de $n$ datos) cuya **matriz de covarianzas tenga el menor determinante**. Se implementa con el algoritmo **FAST-MCD** (Rousseeuw y Van Driessen; `cov.rob(..., method = "mcd")`, paquete `MASS`). 📖 Como la matriz de covarianzas es la base de muchos métodos multivariados, se la usó para desarrollar **técnicas robustas multivariadas**.
- **LOF (Local Outlier Factor):** medida basada en **densidad** con los *k* vecinos más cercanos (paquete `DMwR`, `lofactor`).

**Control univariado vs. multivariado 📖 (Ej. 2.13):** en el control univariado (límites en una variable, por ejemplo 1 y 3 para cajas producidas por una máquina) se ve si un dato **excede o está por debajo de las especificaciones**, pero **no se aprecia si la forma es la adecuada**. El gráfico de dispersión con **elipse de confianza** (normal bivariada) detecta puntos que siguen el patrón general pero se alejan del centro, y puntos que están **dentro del rango de ambas variables pero rompen la forma de la interacción** del grupo (en el ejemplo, el punto (11,6; 3,3)).

**Ejemplo 2.16 (datos `stack.x`, n = 21):** distancias de Mahalanobis según la estimación de Σ. Con **MVE y MCD** (idénticas) las observaciones 1, 2, 3 y 21 tienen distancias grandes (**30,56; 31,78; 17,62; 13,38**), mientras que con la **covarianza clásica** valen apenas **5,08; 5,40; 2,54; 4,74** → la estimación clásica **enmascara** los outliers. Con **LOF** (*k* = 5) también se señalan las observaciones atípicas.

---

# 6. 🔄 Transformación de datos

[⬆️ Volver al índice](#indice)

> "En algunas ocasiones, para **optimizar el análisis** de la información, es conveniente **realizar transformaciones a los datos**. Pueden ser **por filas o por columnas** (por **individuos** o por **variables**)." (Chan, Badano y Rey, 2019)

**Objetivos más usuales:** (1) hacer **comparables las magnitudes**; (2) **modificar la escala** de medición; (3) **satisfacer alguna propiedad estadística** (necesaria para ciertos modelos). 📖 Neutralizan diferencias de escala o sesgos de medición y garantizan comparabilidad antes de aplicar algoritmos multivariados.

> 📖 **Qué hay en el PDF del libro (Sec. 2.5):** se desarrollan la **estandarización (puntajes Z)** y la **transformación por individuo (jueces)**. Los demás tipos marcados con ➕ (centrado, raíz cuadrada, Box-Cox, perfiles, norma euclídea) provienen de tus resúmenes o de las continuaciones; min-max y logarítmica vienen de las clases.

## 6.1 Transformaciones por variables (columnas)
Evitan que variables con mayor magnitud o varianza **dominen** el análisis (ej. PCA o clustering), sobre todo con unidades distintas (kg, m, miles de pesos). 📖 En el libro el objetivo es **hacer comparables los valores** asignados a los distintos individuos u objetos (por ejemplo, jueces con tendencia a puntuaciones muy altas o muy bajas).

| Nombre | Fórmula | Para qué |
|---|---|---|
| **Centrado** ➕ (*mean centering*) | $x'_{ij} = x_{ij} - \bar{x}_j$ | Traslada el origen al **centro de gravedad** de la nube; media 0, **conserva la varianza** |
| **Z-score** (estandarización / tipificación) | $z_{ij} = \dfrac{x_{ij} - \bar{x}_j}{s_j}$ (en clase: $Z = (X-\mu)/\sigma$) | **Media 0 y varianza 1**; adimensional; **exagera las distancias** → útil para **detectar atípicos** |
| **Min-max** (máx-mín) | $x'_{ij} = \dfrac{x_{ij} - \min(X_j)}{\max(X_j) - \min(X_j)}$ | Lleva a **[0, 1]** conservando proporcionalidad de distancias |
| **Logarítmica** | $x' = \log(x + c)$ (en clase: $\log(X+1)$) | **Reduce la influencia de atípicos**; corrige asimetría a derecha |
| **Raíz cuadrada** ➕ | $x' = \sqrt{x}$ | Útil para **conteos** (Poisson) |
| **Box-Cox** ➕ | familia de potencias λ | Halla la mejor potencia λ para **normalizar** la variable |

- 📖 **Consideración robusta del Z-score:** asume que media y desvío representan bien centralidad y dispersión. Con fuerte asimetría o atípicos se distorsionan; alternativa: **mediana** en lugar de la media y **MAD** o **IQR** en lugar del desvío.
- ➕ Asimetría positiva (variables económicas o biológicas) → transformaciones no lineales (log, raíz, Box-Cox) para acercar a la normal.
- 🗣️ **La min-max "no es una normalización"** en el sentido de la distribución normal; es una transformación máximo–mínimo.
- 🗣️ **Log natural:** el exponente al que hay que elevar *e* para obtener ese número; es la **inversa de la exponencial**.
- 🗣️ **Ejemplo del efecto sobre valores 4 y 10:**
  - Original: el 10 es **2,5 veces** el 4.
  - **Logarítmica:** 10 ≈ **2,4**, 4 ≈ **1,6** → el 10 vale solo ≈ **50 % más** (los atípicos **pierden influencia**).
  - **Min-max:** 10 = **1**, 4 ≈ **0,33** → el 10 vale **el triple**.
  - **Z-score:** separa mucho los valores (el 4 negativo, el 10 ≈ +1,4).
- 🗣️ La log se usa en modelos que funcionan mejor con ciertas distribuciones (ChatGPT suele sugerirla para el TP y "tiene lógica, no es un capricho").

```r
# Ejemplo complementario ➕ (el Código 2.18 del libro es otro: gráfico de control univariado)
datos_estandarizados <- scale(mtcars[, 1:4])   # media 0, varianza 1
apply(datos_estandarizados, 2, mean)
apply(datos_estandarizados, 2, sd)
```

**Transformaciones de tipo de variable:**

| Transformación | Ejemplo |
|---|---|
| **Cuantitativa → ordinal** | Edad en años → "joven", "adulto", "anciano" |
| **Ordinal/categórica → cuantitativa** | Asignar valores numéricos (arbitrarios o por algoritmos) |
| **String → datetime** | Texto a fecha (`to_datetime`) |

🗣️ Hoy **se puede transformar cualquier cosa**: los modelos de IA **transforman palabras en vectores** y hacen transformaciones algebraicas.

## 6.2 Transformaciones por individuo (filas)
Homogeneizan a los individuos, neutralizando tendencias subjetivas o diferencias de tamaño. ➕ Frecuentes en ecología (abundancia de especies), química (composición de mezclas) y análisis de texto.

**a) Neutralización de jueces (clase + libro):**

$$T(x) = \begin{cases} \dfrac{x - \bar{x}}{x_{max} - \bar{x}} & \text{si } x > \bar{x} \\[2mm] \dfrac{x - \bar{x}}{\bar{x} - x_{min}} & \text{si } x < \bar{x} \end{cases}$$

- Se usa la media, máximo y mínimo **del individuo (juez)**; deja valores **relativos a su propia media**. Las puntuaciones superiores a la media resultan **positivas** (escala: tramo superior) y las inferiores **negativas** (escala: tramo inferior).
- 🗣️ **Jurados** (Polino vs. Moria Casán; Charlie Sheen en EE. UU.): un jurado "duro" (1, 2, 4) y uno "generoso" (6, 7, 10) usan criterios distintos; transformados a la misma escala, **el 2 de Polino es "más valioso" que el 7 de Moria Casán**.
- 🗣️ Otro ejemplo: notas de **Matemática** (exigente) vs. **Legislación** (más "fácil").
- 📖 Los jueces pueden puntuar sistemáticamente alto/bajo o usar rangos distintos (1–10 vs. 4–7).

**b) Relativización por el total (perfiles) ➕:** convierte frecuencias absolutas en **composiciones proporcionales** (la suma de la fila es 1). Ej.: una muestra de suelo más grande tiene conteos mayores en todas las especies; al relativizar se compara la composición.

$$x'_{ij} = \frac{x_{ij}}{\sum_{j=1}^{p} x_{ij}}$$

**c) Normalización vectorial (norma euclídea) ➕:** todos los vectores-individuo quedan de **longitud 1** (proyectados sobre una hiperesfera unitaria).

$$x'_{ij} = \frac{x_{ij}}{\sqrt{\sum_{j=1}^{p} x_{ij}^2}}$$

---

# 7. 📈 Análisis estadístico de datos

[⬆️ Volver al índice](#indice)

## 7.1 Organización de los datos
Hay que **ordenar y organizar** la base para facilitar la **comprensión e interpretación**; los **datos crudos** pueden resultar **inabordables** (miles de filas, cientos de columnas). 🗣️ La **estadística es la herramienta**; se empieza con una **primera exploración por análisis de frecuencias**.

## 7.2 Análisis de frecuencias

| Datos | Cómo |
|---|---|
| **Cualitativos** | **Conteo** de veces que se repite cada categoría |
| **Cuantitativos** | Si la variable **no es discreta** hay que usar **intervalos de clase** (ej.: 0–16, 17–30, 31–50, 51–65, 65+) |

- Tablas de distribución de frecuencias **absolutas, relativas y porcentuales**.
- 📖 **Cómo se calculan:** la frecuencia absoluta $f_i$ es la cantidad de observaciones de cada clase y se cumple $f_1 + \dots + f_m = n$. **Relativa** = $f_i / n$; **porcentual** = $f_i / n \times 100$. La **frecuencia absoluta acumulada** es $F_k = \sum_{i=1}^{k} f_i$.
- 📖 **Ejemplos del libro:**
  - *Cualitativa (Ej. 2.1, autos vendidos en una concesionaria):* utilitario 6, familiar 10, cupé 7, camioneta 12, sedán 17.
  - *Discreta (Ej. 2.2, ventas mensuales de alta gama en 24 meses):* en 2 meses se vendió 1 vehículo, en 3 meses 2, en 7 meses 3, en 4 meses 4 y en 8 meses 5.
  - *Continua (Ej. 2.3, gramos de proteínas por día, n = 32):* intervalos [7,9), [9,11), [11,13), [13,15), [15,17) con frecuencias 6, 10, 4, 7, 5. La relativa de [11,13) es 4/32 = 0,125 (12,5 %); los porcentajes son 18,75; 31,25; 12,5; 21,88 y 15,62. Los porcentajes dan una idea de la **concentración** que la frecuencia absoluta no muestra.
- 🗣️ **Ejemplo (League of Legends, 172 personajes):** 49 luchadores (**28,5 %**), 37 magos (**21,5 %**), 28 marksman, 24 tanques, 17 asesinos, 17 apoyo.
- 🗣️ El conteo ("contar cabezas") es **la forma más primitiva** de estadística, pero sirve de primera aproximación.

## 7.3 Medidas descriptivas univariadas (una variable a la vez)

### 🔹 Tendencia central 🎯
- **Resúmenes**: representan un conjunto de valores **con un solo valor** ("hay información que se escapa").
- **Media aritmética** (suma / cantidad): promedio clásico, **muy sensible a extremos (no robusta)**. **Mediana** (valor central con datos ordenados; divide al 50 %): **robusta**. **Moda** (valor o intervalo de mayor frecuencia).
- **Media geométrica** 🗣️: **multiplica** los valores y calcula la **raíz enésima**; útil con **valores extremos altos**: da un valor **más bajo** que la aritmética.
- **Media podada (alfa-podada)** 🗣️📖: **quita un porcentaje de extremos** (ej. 5 % más bajo y 5 % más alto) y calcula la media (`trim_mean` de scipy).

**Ejemplo de clase 🗣️ (Riot Points de LoL):**

| Medida | Valor |
|---|---|
| Media aritmética | **711,73** |
| Media geométrica | **662** |
| Media podada | **740** |
| Mediana | **790** |
| Moda | **880** |
| Q1 / Q3 | 585 / 880 |

- **Lectura:** la media podada **es más alta** que la aritmética → **atípicos hacia abajo**. Asimetría **−1,08**. Orden: **media < mediana < moda**.
- 🗣️ Casi todo es categórico; solo **Riot Points y Blue Essence** podrían tratarse como continuas.
- 🗣️ Un ingreso muy alto (ej. $15–20 millones) es **real** y no se quiere excluir, pero se puede usar media geométrica para que no condicione tanto. "Un analista debe conocer estas herramientas."

### 🔹 Posición 🎯
Dividen el conjunto ordenado **en partes iguales** (**estadísticos de orden**; cuantiles).

| Medida | Divide en… | Cortes |
|---|---|---|
| **Mediana** | 2 partes | 1 |
| **Cuartiles** | 4 partes | 3 (Q1, Q2, Q3) |
| **Quintiles** | 5 partes | 4 |
| **Deciles** | 10 partes | 9 |
| **Percentiles** | 100 partes | 99 |

> 🎯 **PREGUNTA TRAMPA:** *"¿Qué tipo de medida es la mediana?"* → **AMBAS: tendencia central Y posición**.

**La mediana es robusta 🗣️:** no se ve afectada por valores extremos (da igual que el mayor sea 9.990 o 15.000 millones); **más robusta que la media e incluso que la geométrica**; sirve en **muestras pequeñas**.

### 🔹 Dispersión 🎯
Indican la **variabilidad**; la mayoría cuantifica la **concentración de datos alrededor de una medida de posición o de tendencia central**.

| Medida | Descripción |
|---|---|
| **Rango** | Máximo − mínimo (sensible a extremos) |
| **Varianza** | Suma de diferencias de cada valor con **la media**, **al cuadrado** (sensible a extremos) |
| **Desvío estándar** | **Raíz cuadrada** de la varianza → vuelve a las **unidades originales** |
| **Coeficiente de variación** | Desvío estándar / media; **compara dispersión entre conjuntos con distintas medias o unidades** |
| **Rango intercuartílico (IQR / RI)** | **Q3 − Q1** (robusta, basada en posición) |
| **MAD** | **Mediana de los desvíos absolutos respecto de la mediana** (robusta); 📖 normalizada como **MADN** |

- 🗣️ Varianza, desvío y coeficiente de variación son **transformaciones de la misma medida**.
- 🗣️ **Varianza poblacional: sobre N. Varianza muestral: sobre N − 1** → resultado **más alto** que **evita subestimar la dispersión**.

### 🔹 Forma: asimetría y curtosis
- **Asimetría:** indica si la distribución es **simétrica, de asimetría positiva (a derecha) o negativa (a izquierda)** respecto de la media.
  - **Negativa:** pocos valores extremos a la izquierda; **moda > mediana > media**; al recortar extremos la media se acerca a la mediana y a la moda.
  - **Coeficiente de Fisher(–Pearson)** (el de los Riot Points: −1,08). **Coeficiente de Pearson:** (media − moda) / desvío estándar. **Coeficiente de Bowley:** usa **cuartiles**.
- **Curtosis:** grado de **apuntamiento**: **leptocúrtica, mesocúrtica, platicúrtica**.
- 🗣️ **Reflexión clave:** **los datos no "hablan solos"**. Las estimaciones **se construyen** con metodologías y **definiciones arbitrarias**; distintas metodologías dan distintos resultados. Hay que tomar los datos "con pinzas".

### 📖 Propiedades, fórmulas y ejemplos resueltos del libro (Sec. 2.2)

**Media aritmética:** $\bar{x} = \frac{1}{n}\sum_{i=1}^{n} x_i$. Es de cálculo sencillo, solo se puede calcular para **escalas cuantitativas**, **preserva la dependencia lineal** (si $y = ax + b$ entonces $\bar{y} = a\bar{x} + b$), **no puede aplicarse a datos censurados** y es muy sensible a extremos (no robusta).

**Mediana:** $\tilde{x} = x_{((n+1)/2)}$ si *n* es impar; $\tilde{x} = \frac{x_{(n/2)} + x_{(n/2+1)}}{2}$ si *n* es par. Se calcula para escalas **al menos ordinales**, preserva la dependencia lineal y **no es sensible a extremos** (robusta).

**Moda:** observación de mayor frecuencia. **No es muy estable** (una sola observación puede cambiarla) y **puede no ser única** (bimodales o multimodales), caso en que informa poco.

**Ejemplo 2.4 (libro):** {12, 12, 15, 18, 23} → mediana 15, media 16, moda 12. {12, 12, 15, 17, 25, 25} → mediana 16, media 17,67 y **dos modas** (12 y 25). Para una tabla de frecuencias con valores 2, 3, 7, 8 y $f_i$ = 10, 15, 20, 5 (n = 50): mediana = (3 + 7)/2, media = 4,9, moda = 7. Para valores 1, 5, 6, 8 con $f_i$ = 10, 14, 21, 4 (n = 49): mediana = 6, media ≈ 4,86, moda = 6.

**Media α-podada:** promedio de los datos centrales recortando el α % de los valores más grandes y el α % de los más chicos. Sus posiciones extremas son la **media aritmética (α = 0 %)** y la **mediana (α = 50 %)**. *Ej. 2.5:* con n = 20 datos, la podada al 10 % (sacando 2 de cada extremo) da **10,125**.

**Cuantiles:** valores que subdividen los datos en partes con igual cantidad de observaciones; **pueden o no coincidir con valores observados**. Cuartiles (25 % cada parte; **Q2 = mediana**), deciles (D) y percentiles (P). El mínimo $x_{(1)}$ y el máximo $x_{(n)}$ son estadísticos de orden.

**Rango:** $x_{(n)} - x_{(1)}$. De cálculo sencillo pero **poco informativo**: tres conjuntos pueden tener el mismo rango y distinta concentración alrededor del centro.

**Varianza muestral:** $s_x^2 = \frac{1}{n-1}\sum_{i=1}^{n}(x_i - \bar{x})^2$ (el denominador $n-1$ da una **estimación más precisa de la varianza poblacional**, sobre todo con *n* chico). Solo para variables cuantitativas; si $y = ax + b$, entonces $s_y^2 = a^2 s_x^2$; sus **unidades son el cuadrado** de las originales; es muy sensible a extremos. **Desvío estándar:** $s_x = \sqrt{s_x^2}$ (vuelve a las unidades originales).

**Coeficiente de variación (CV):** desvío / media, usualmente en %. Es **dispersión relativa** (las anteriores son absolutas). Se usa cuando las medias o las unidades de los conjuntos son distintas; si las medias son parecidas y comparten unidad, alcanza con comparar desvíos. 📖 **Si la media no es una buena medida de centro, tampoco lo son varianza, desvío ni CV** → usar RI y MAD.

**RI** = Q3 − Q1 (rango del 50 % central). **MAD:** mediana de los desvíos absolutos respecto de la mediana. *Ej. 2.6:* {2, 3, 5, 8, 13, 27} → mediana 6,5; desvíos −4,5; −3,5; −1,5; 1,5; 6,5; 20,5; en valor absoluto ordenados 1,5; 1,5; 3,5; 4,5; 6,5; 20,5 → **MAD = (3,5 + 4,5)/2 = 4**. **MADN = MAD / 0,6745**, normalización para que sea comparable con el desvío estándar (en una **normal** coinciden); 0,6745 sale de que $\Phi(w) = 0{,}75$ en $w = 0{,}6745$.

**Asimetría de Fisher:** $sk_F = \dfrac{\sqrt{n}\sum (x_j - \bar{x})^3}{[\sum (x_j - \bar{x})^2]^{3/2}}$. En distribuciones simétricas (como la normal) ≈ 0 y **media = mediana = moda**; la media es "arrastrada" por los extremos. Asimetría negativa: media < mediana < moda. Positiva: moda < mediana < media. **Pearson:** $sk_P = (\bar{x} - Mo)/s_x$, **menos usual** porque requiere distribución unimodal. **Bowley:** $\frac{q_3 + q_1 - 2\tilde{x}}{q_3 - q_1}$, usa cuartiles y se emplea cuando media y desvío **no son representativos**.

**Curtosis:** $k = \dfrac{n\sum (x_j - \bar{x})^4}{[\sum (x_j - \bar{x})^2]^2}$. Describe el **apuntamiento** y el comportamiento de las **colas**. En la normal **k ≈ 3**; **leptocúrtica** k > 3, **platicúrtica** k < 3. **Una mayor curtosis no implica mayor varianza, ni viceversa.**

### 📖 Gráficos univariados (libro; 🚫 visualización no entra)
- **Histograma:** discreto y **depende de los intervalos de clase (bins)**; el código 2.8 lo genera variando la cantidad de clases.
- ➕ **Curva de densidad suavizada (KDE):** estimación continua y suavizada de la distribución subyacente, menos dependiente de los bins *(no figura en el PDF del libro)*.
- ➕ **Tallo y hojas (stem-and-leaf):** **no pierde los datos originales**; separa cada número en "tallo" y "hoja"; se imprime en consola como histograma rotado *(no figura en el PDF del libro)*.

```r
# Ejemplo complementario ➕ (el Código 2.10 del libro es otro: diagrama de mosaicos)
densidad <- density(iris$Sepal.Length)
hist(iris$Sepal.Length, prob = TRUE, main = "Histograma y Curva de Densidad",
     xlab = "Longitud del sépalo", ylab = "Densidad",
     col = "lightsteelblue", border = "white")
lines(densidad, lwd = 2, col = "indianred1")

# Ejemplo complementario ➕
stem(iris$Sepal.Length)
```

📖 **Otros gráficos univariados del libro (Sec. 2.2.5):**
- **Diagrama circular:** para variables **cualitativas y cuasicuantitativas**; muestra la proporción de cada categoría (también "tortas anidadas" para dos variables).
- **Gráfico de barras:** para variables cualitativas; **aventaja al circular** porque permite apreciar la **distribución conjunta de más de una variable** (barras **superpuestas** o **adyacentes**).
- **Gráfico de bastones:** para la distribución de frecuencias de una variable **discreta**.
- **Histograma y polígono de frecuencias:** para variables **continuas**. El polígono une los **puntos medios de las bases superiores** de los rectángulos; si el ancho de las bases se redujera indefinidamente, **tendería a la curva de densidad**. En R, `hist` grafica frecuencias absolutas; con `prob=TRUE`, relativas. **Demasiadas clases** → histograma irregular; **muy pocas** → sobresuavizado.
- **¿Cuántos intervalos?** Reglas para el número *k*: **Dixon y Kronmal (1965)** $\lfloor 10\log(n)\rfloor$; **Velleman (1976)** $\lfloor 2\sqrt{n}\rfloor$; **Sturges (1926)** $\lfloor 1+\log_2(n)\rfloor$. Reglas para el **ancho** $h_n$: **Scott (1979)** $3{,}49\, s\, n^{-1/3}$ y **Freedman–Diaconis (1981)** $2R\, n^{-1/3}$ (*s* = desvío estándar, *R* = rango intercuartil).

## 7.4 Análisis bivariado
- **Dos variables de forma conjunta**: una **independiente** y una **dependiente**; también hay análisis **simétricos**. Ej.: peso según altura, desocupación según aglomerado, ingreso según ocupación.
- 🗣️ **Tabla de frecuencias de doble entrada** (ej.: tipo de héroe × tipo de rango: 14 asesinos cuerpo a cuerpo, 47 luchadores cuerpo a cuerpo, 35 magos a distancia…).
- 📖 **Gráfico de dispersión (scatterplot):** eje X e Y, cada punto una observación conjunta $(x_i, y_i)$; permite ver si hay relación lineal, no lineal, directa, inversa o independencia.

```r
# Ejemplo complementario ➕ (el Código 2.12 del libro es el dispersograma)
plot(iris$Sepal.Length, iris$Petal.Length, main = "Relación entre Longitud de Sépalo y Pétalo",
     xlab = "Longitud del Sépalo", ylab = "Longitud del Pétalo", pch = 19, col = "royalblue")
```

### Covarianza
- Variabilidad **conjunta**; asociación **lineal**; **no estandarizada** → depende de la **escala**.
- Clase: `cov(x,y) = Σ(xᵢ − x̄)(yᵢ − ȳ) / (N − 1)`. 📖 Libro: $s_{ik} = \frac{1}{n}\sum_{j=1}^{n}(x_{ji}-\bar{x}_i)(x_{jk}-\bar{x}_k)$ (la diferencia $n$ vs. $n-1$ es la de varianza poblacional vs. muestral).
- 🗣️ Es la **misma fórmula que la varianza**, con dos variables distintas; si se reemplaza *y* por *x* se obtiene la **varianza**.
- Signo (📖): $s_{ik} > 0$ asociación lineal **positiva**; $< 0$ **negativa**; $= 0$ **ausencia** de asociación lineal.
- 🗣️ **Defecto:** difícil de interpretar (valores como −17, −0,15, −459 o 331.556 según la escala).

**Propiedades 📖:**
- $Cov(X, X) = Var(X)$.
- Distributiva: $Cov(X_1 + X_2, Y) = Cov(X_1, Y) + Cov(X_2, Y)$.
- Con matrices: $Cov(AX, BY) = A \cdot Cov(X, Y) \cdot B^t$.
- **Dependencia lineal:** si una variable es función lineal exacta de otra (ej. $Y = -2X + 3$), $\det(\Sigma) = 0$ → **matriz singular** (información redundante).
- **Dependencia de unidades:** $Cov(aX, cY) = ac \cdot Cov(X,Y)$.

### Correlación 🎯
| Variables | Medida |
|---|---|
| Numéricas | **Pearson**: **estandariza la covarianza** → valores **entre −1 y 1**; asociación **lineal** (no capta relaciones cuadráticas, cúbicas…) |
| Numéricas (alternativa) | **Spearman**: usa **rangos** → menos sensible a extremos |
| **Categóricas** | **V de Cramer** |
| **Numérica + categórica** | **t de Student** o **coeficiente eta** |

📖 $r_{ik} = \dfrac{s_{ik}}{\sqrt{s_{ii}}\sqrt{s_{kk}}}$: es la **covarianza de las variables estandarizadas (puntajes Z)**. $|r_{ik}| \le 1$; con $r_{ik} = \pm 1$ los datos yacen exactamente sobre una **recta**. Cercano a 1: fuerte asociación lineal positiva; cercano a −1: fuerte negativa; cercano a 0: ausencia de relación lineal.

**Cómo interpretar una matriz de correlación 🎯🗣️:**
- Valores de **−1 a 1**. **Positivo** = crecen juntas; **negativo = correlación inversa** (uno crece, el otro decrece), **NO** significa "no hay correlación"; **cerca de 0 = falta de asociación**.
- La **diagonal siempre vale 1**.
- Se visualiza con **mapa de calor (heatmap, Seaborn)**; 📖 en R, **correlogramas** (`corrplot`): **azul = positiva, rojo = negativa**, intensidad proporcional a la magnitud.
- **Ejemplo (LoL):** asociación positiva más fuerte: **Blue Essence – Riot Points (0,84)** (dos monedas para el precio de los personajes). Casi sin asociación: **utility–difficulty (0,02)**, **control–ID**.
- **Clusterización** 🗣️: reordena las variables de modo que las de alta correlación quedan juntas (arriba a la izquierda); es un anticipo de los modelos de clustering que se ven más adelante en la cursada.
- **Correlación no implica causalidad:** una correlación alta (0,84 entre dos variables que miden el precio de un personaje en dos monedas del juego) tiene sentido lógico en ese caso puntual, pero en general hay que ser cuidadoso al inferir causalidad a partir de una correlación.

### 📖 Ejemplos del libro: correlación, singularidad, traza y correlograma
- **Propiedades de la correlación muestral:** $|r_{ik}| \le 1$; $r_{ik} = 1$ → datos sobre una **recta de pendiente positiva**; $r_{ik} = -1$ → recta de pendiente **negativa**; $0 < r_{ik} < 1$ → datos **alrededor** de una recta de pendiente positiva; $-1 < r_{ik} < 0$ → alrededor de una de pendiente negativa; $r_{ik} = 0$ → **no hay asociación lineal**. **Tanto $s_{ik}$ como $r_{ik}$ son muy sensibles a outliers**; con outliers conviene usar otras medidas de asociación.
- **Ejemplo 2.14:** $X$ con $\mu_X = 4$, $\sigma_X^2 = 2$ e $Y = -2X + 3$ → $\mu_Y = -5$, $\sigma_Y^2 = 8$, $Cov(X, Y) = -2\,Var(X) = -4$. La matriz $\Sigma = \begin{pmatrix} 2 & -4 \\ -4 & 8 \end{pmatrix}$ tiene **determinante nulo** (matriz **singular**), porque una variable es función lineal de la otra (**linealmente dependientes**). La correlación es $\begin{pmatrix} 1 & -1 \\ -1 & 1 \end{pmatrix}$; **tr(Σ) = 10** y **tr(Corr) = 2**.
- **Ejemplo 2.15:** si $A = \begin{pmatrix} 2 & 3 \\ -4 & 8 \end{pmatrix}$, entonces $tr(A) = 2 + 8 = 10$. La traza es un número real (puede ser positivo, negativo o nulo), pero en Σ y en R es **no negativa/positiva**.
- **Correlograma (datos de IMC infantil):** EDAD–PESO 0,73; EDAD–TALLA 0,84; EDAD–IMC 0,45; PESO–TALLA 0,87; PESO–IMC 0,87; TALLA–IMC 0,54. La variable CC se **modificó** (máx − CC) para que correlacione **negativamente** con las demás: EDAD–CC −0,64; PESO–CC −0,92; TALLA–CC −0,73; IMC–CC −0,88. Se aprecia: azul = positiva, rojo = negativa; mayor intensidad = más cerca de ±1; EDAD, PESO, TALLA e IMC correlacionan positivamente; es **más intensa** la correlación PESO–TALLA que EDAD–PESO, e IMC–CC que EDAD–CC.

## 7.5 Análisis multivariado
- **Más de dos variables** a la vez. **Registros = filas (n)**; **variables = columnas (p)**.
- **Matriz de covarianzas Σ** 📖: simétrica; **diagonal = varianzas** ($s_{ii}$), fuera de la diagonal las covarianzas. **Matriz de correlaciones R** 📖: simétrica con **unos en la diagonal**.
- **Traza** 📖 $tr(A) = \sum a_{ii}$ (suma de la diagonal):
  - **$tr(\Sigma)$** = suma de todas las varianzas → **variabilidad total** ("magnitud" del problema).
  - **$tr(R) = p$** (número de variables), porque la diagonal son unos.
- **Complejidad** (cantidad de parámetros): **`2p + p·(p − 1)/2`** → *p* medias + *p* varianzas + *p(p−1)/2* covarianzas. Ej.: p = 4 → 8 + 6 = **14**; p = 5 → **20**.
- 🗣️ Al **agregar variables el análisis se vuelve más costoso** (tiempo, memoria, energía). El docente lo describió como "medio exponencial"; ⚠️ matemáticamente el término dominante es **cuadrático** (*p²*).
- **Técnicas avanzadas** (final del cuatrimestre): **componentes principales**, **correspondencias** (🚫 no entran), **clusterización**, **modelado** ("poquito").

### 📖 Información multivariada del libro (Sec. 2.3 y 2.4)
- **Matriz de datos:** tabla con *p* variables (columnas) observadas sobre *n* individuos (filas); $x_{ij}$ es el valor de la variable *j* en el individuo *i*. *Ej. 2.10 (galletitas):* p = 5 (valor energético, carbohidratos, proteínas, grasas, sodio) y n = 17 marcas; $x_{23} = 10$ son los gramos de proteínas cada 100 g de la Marca 2.
- **Objetivo:** el análisis multivariante estudia **cada variable aisladamente y también las relaciones entre ellas**. En el caso univariado se estiman 2 parámetros (centralidad y dispersión); con *p* variables hay que aproximar **$2p + p(p-1)/2 = (p^2 + 3p)/2$** parámetros.

| Variables | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|---|---|---|---|---|---|---|---|---|---|
| **Parámetros** | 5 | 9 | 14 | 20 | 27 | 35 | 44 | 54 | 65 |

- **Objetivos del análisis exploratorio (libro):** conocer los datos; descubrir regularidades; verificar la existencia de estructuras ocultas; entender los patrones descubiertos; resumir información; hallar asociaciones de variables; detectar anomalías.
- **Vector de medias y matriz Σ:** $\bar{x} = (\bar{x}_1, \dots, \bar{x}_p)$ y $\hat{\Sigma} = \frac{1}{n}(X - \bar{X})^t (X - \bar{X})$, de tamaño $p \times p$, **simétrica**, con las **varianzas en la diagonal** y las covarianzas fuera de ella. Propiedades: $\hat{\Sigma}$ estima la matriz poblacional; es **semidefinida positiva** (autovalores ≥ 0); si $Y = XA + B$, entonces $\Sigma_Y = A^t \Sigma_X A$; el vector de medias respeta las transformaciones lineales.
- **Ejemplo 2.12:** $X = \begin{pmatrix} 10 & 4 \\ 15 & 1 \\ 20 & 7 \end{pmatrix}$ → $\bar{x} = (15, 4)$ y $\hat{\Sigma} = \frac{1}{3}\begin{pmatrix} 50 & 15 \\ 15 & 18 \end{pmatrix} = \begin{pmatrix} 16{,}67 & 5 \\ 5 & 6 \end{pmatrix}$.
- **Formas de presentar datos multivariados (🚫 visualización no entra, pero conviene conocerlas):**
  - **Tabla de clasificación cruzada:** distribución conjunta de dos variables. Ej.: 1.441 clientes que compran un auto 0 km según si tuvieron en cuenta la **garantía** y el **consumo** (garantía NO: 258 no consideran consumo y 280 sí, total 538; garantía SÍ: 184 y 719, total 903; totales 442 y 999).
  - **Gráfico de mosaicos:** para **dos variables categóricas** / distribuciones conjuntas. Ej.: es menor la proporción que tuvo en cuenta el consumo entre quienes consideraron la garantía (se interpreta mirando las áreas).
  - **Diagrama de dispersión:** con `mtcars`, peso vs. millas por galón coloreado por **cilindrada** (4, 6, 8); permite ver características individuales, posición de los grupos y relación entre variables por grupo.
  - **Dispersograma (matriz de dispersión de a pares):** vínculo entre pares de variables cuantitativas (EDAD, PESO, TALLA, IMC, CC), en general y por sexo.
  - **Coordenadas paralelas:** **ejes paralelos**, uno por atributo, **escalados** a igual altura; **cada individuo es una línea** que une sus valores. Permite apreciar similitud entre observaciones y comparar subgrupos (ej. iris: setosa se diferencia de virginica y versicolor).
  - **Perfiles multivariados:** **medias o medianas** de cada variable por grupo. Ej.: galletitas dulces vs. saladas tienen composición media similar, excepto el **sodio**.
  - **Curvas de nivel:** unen puntos de igual densidad; ejemplo con la **normal bivariada**.
  - **Gráficos de estrellas:** para **variables todas cuantitativas**; cada variable es un radio de la estrella. Ej. `mtcars`: Mazda y Mazda Wag son similares, y también Merc D y Merc.
  - **Caras de Chernoff:** características cuantitativas asociadas a rasgos de una cara (ej. galletitas saladas: similares las marcas 8, 9 y 11, y las 5 y 6).

## 7.6 📖 Ejercitación del libro (Cap. 2)

> El docente recomendó **realizar los ejercicios**. Estos son los 7 del capítulo 2 (los datos de varios están en links del libro).

**Datos del Ejercicio 1 (Tabla 2.13, candidatas a recepcionista; 2 jueces × 3 tópicos):**

| Candidata | J1 Cordialidad | J1 Presencia | J1 Idioma | J2 Cordialidad | J2 Presencia | J2 Idioma |
|---|---|---|---|---|---|---|
| Mariana | 80 | 90 | 70 | 60 | 78 | 80 |
| Maia | 80 | 90 | 60 | 65 | 90 | 65 |
| Sabrina | 90 | 60 | 50 | 70 | 60 | 50 |
| Daniela | 80 | 50 | 50 | 70 | 58 | 40 |
| Alejandra | 70 | 60 | 50 | 55 | 70 | 65 |
| Carla | 90 | 85 | 60 | 80 | 90 | 40 |

1. **Transformaciones de datos.** (a) Promedio por juez de cada aspirante: ¿a quién elegiría cada juez? ¿Hay coincidencia? (b) Promedio de cada aspirante con todos los aspectos y ambos jueces. (c) Transformar para que **cada una de las seis variables tenga media 0 y dispersión 1**: ¿cuál es el objetivo? (d) Transformar para que **cada candidata tenga, para cada juez, media 0 y dispersión 1**: ¿objetivo? (e) Graficar los perfiles multivariados de cada candidata con ambas transformaciones: ¿qué se observa?
2. **Tipos de variables y limpieza** (1.500 individuos; ID, Nacionalidad, Edad, Sexo [1/2], Estatura, Interés de conexión [1 a 7], Tiempo de uso diario en minutos, Temperatura media anual de la zona, Autos en la manzana, Cigarrillos mientras usa internet). (a) Clasificar las variables y hacer un gráfico de coordenadas paralelas de las numéricas. (b) Tabla de frecuencias de Sexo: ¿algún valor llama la atención? ¿qué tipo de error podría ser? (c) Ordenar por Edad: ¿valores extraños? (d) Tabla de frecuencias de Interés. (e) Proceder igual con Temperatura, Autos y Cigarrillos. (f) **Eliminar los valores imposibles** (probable error de tipeo) y detallar los que llaman la atención pero **no deben eliminarse necesariamente**. (g) ¿Para qué variables tiene sentido la **media**? ¿Y la **mediana**? (h) ¿Cuáles parecen simétricas? Confirmar con boxplot. (i) Calcular el **RI** y detectar **valores salvajes moderados y severos**.
3. **Gráficos univariados y multivariados** (49 gorriones; Largo, Alas, Cabeza, Pata, Cuerpo, Sobrevida [1 vivo / −1 muerto]). (a) Tipo de cada variable. (b) Informe univariado de cada una. (c) Histograma, ensayando el número de intervalos e indicando el criterio. (d) **Boxplot comparativo** por sobrevida: ¿alguna variable toma valores muy distintos en ambos grupos? Analizar outliers. (e) Gráficos bivariados coloreados por supervivencia: ¿alguna regularidad explica la supervivencia? (f) Matriz de dispersión: ¿pares relacionados? ¿la asociación difiere por grupo?
4. **Gráficos de estrellas** (26 razas de perros; Tamaño, Peso, Velocidad, Inteligencia, Afectividad, Agresividad, Función). (a) Estrella por raza con tamaño, peso, velocidad, inteligencia y afectividad. (b) Ídem por función. (c) Ídem por agresividad. (d) Si dos estrellas son similares, ¿se puede decir que las razas son parecidas?
5. **Matriz de covarianzas** (base de gorriones). (a) Dimensión *n* × *p*. (b) Vector de medias, matrices de varianzas-covarianzas y de correlaciones: ¿qué características tienen? (c) Qué representan $m_{11}$ y $m_{31}$ de Σ. (d) Qué representan $m_{22}$ y $m_{13}$ de R. (e) Relacionar $m_{21}$, $m_{11}$ y $m_{22}$ de Σ con $m_{12}$ de R. (f) Crear la variable **Diferencia** = largo total − largo del húmero. (g) Recalcular vector de medias y matrices con la nueva base y relacionarlas con las anteriores. (h) Hallar las **trazas** de las cuatro matrices: ¿qué trazas **no** aumentan al agregar una variable? Explicar.
6. **Propiedades de la matriz de covarianzas** (datos de la Tabla 2.13). (a) Vector de medias e interpretación. (b) Σ y R de las puntuaciones del juez 1 y del juez 2 por separado, y del conjunto total. (c) ¿La suma de las dos primeras submatrices da la matriz del grupo total? Si no, ¿por qué? (d) ¿Se cumple esa relación para las trazas, el vector de medias y los vectores de medianas?
7. **Medidas de posición y escala robustas** (base del ejercicio 2). (a) Con las variables numéricas, agregar **5 observaciones que no sean atípicas en forma univariada pero sí multivariada** y detectarlas con medidas robustas. (b) Agregar **4 outliers enmascarados** y detectar su presencia con estrategias robustas.

---

# 8. 🗂 Resumen rápido (tablas para repasar)

[⬆️ Volver al índice](#indice)

## 8.1 Qué hacer con cada problema de datos
| Problema | Solución |
|---|---|
| **Duplicados** | `drop_duplicates()` (definir criterio: ID o combinación de columnas; consultar la fuente) |
| **Nulos completamente aleatorios** | `dropna()` / listwise deletion |
| **Nulos aleatorios / no aleatorios** | Imputación (medias condicionadas, hot deck, modelos ML) o **reponderación** |
| **Atípicos** | Detectar (boxplot, Z-score, IQR; multivariado: Mahalanobis, MCD/MVE, LOF); **no necesariamente** excluir |
| **Inconsistentes** | **Corregir o eliminar** siempre |

## 8.2 NumPy vs. Pandas
| | NumPy | Pandas |
|---|---|---|
| Estructura | `ndarray` (multidimensional) | `Series` (1D etiquetada) y `DataFrame` (2D) |
| Tipos | **Un solo tipo** por array | Distinto tipo **por columna** |
| Base | Escrita en **C** | Usa **ndarray** para valores numéricos |
| Enfoque | Cálculo numérico, álgebra | Datos tabulares/estructurados |
| `flatten`/`reshape` | Sí | No (no se pueden aplanar Series/DF) |

## 8.3 Medidas: de qué "familia" son
| Familia | Medidas |
|---|---|
| **Tendencia central** | Media, **mediana**, moda (+ geométrica, podada) |
| **Posición** | **Mediana**, cuartiles, quintiles, deciles, percentiles |
| **Dispersión** | Rango, varianza, desvío, coef. de variación, **IQR**, **MAD** |
| **Forma** | Asimetría (Fisher–Pearson, Pearson, Bowley), curtosis |
| **Asociación** | Covarianza, correlación (Pearson, Spearman), V de Cramer, t de Student, eta |

## 8.4 Transformaciones
| Transformación | Fórmula |
|---|---|
| Centrado | x − x̄ |
| Z-score | (X − μ)/σ |
| Min-max | (X − Xmin)/(Xmax − Xmin) |
| Logarítmica | log(X + 1) |
| Por individuo (jueces) | (x−x̄)/(xmax−x̄) si x>x̄; (x−x̄)/(x̄−xmin) si x<x̄ |
| Perfiles / norma euclídea | x/Σx · x/√Σx² |

## 8.5 Patrones de no respuesta (semáforo)
| Color | Tipo | Se explica por… | Solución |
|---|---|---|---|
| 🟢 | Completamente aleatoria | Nada (azar/factor externo) | Eliminar |
| 🟡 | Aleatoria | **Otra variable** del dataset | Imputar / reponderar usando esa variable |
| 🔴 | No aleatoria | **La propia variable objetivo** | Problema circular, el más grave |

## 8.6 Σ vs. R
| | Covarianzas Σ | Correlaciones R |
|---|---|---|
| Diagonal | Varianzas | Unos |
| Unidades | Dependen de las unidades | Adimensional (−1 a 1) |
| Traza | Suma de varianzas | Igual a p |

---

# 9. 🧩 Mnemotecnias

[⬆️ Volver al índice](#indice)

- **5 V de Big Data:** **V**olumen, **V**elocidad, **V**ariedad + **V**eracidad y **V**alor.
- **Estadística vs. minería:** *DE-CO-CON-opcional* vs. *IN-EX-SIN-indispensable*.
- **Variables:** Categórica → Ordinal → Discreta → Continua ("no ordena → ordena → cuenta → mide").
- **Etapas:** **R**ecolectar → **A**lmacenar → **L**impiar → **A**nalizar → **V**isualizar (**RALAV**).
- **Problemas de limpieza:** **N**ulos, **D**uplicados, **A**típicos/inconsistentes.
- **Atípico vs. inconsistente:** "raro pero real" vs. "imposible".
- **Umbrales de no respuesta:** **5 – 10 – 30**.
- **La mediana es doble agente:** central **y** posición.
- **Posición:** 2 · 4 · 5 · 10 · 100.
- **N−1:** "exagera" la dispersión para no subestimarla.
- **Media podada > aritmética** ⇒ atípicos hacia **abajo** (asimetría negativa).
- **loc = etiquetas · iloc = posiciones.**
- **Correlación:** diagonal = 1; negativo ≠ "nada"; 0 = sin asociación.
- **n = filas · p = columnas.**
- **LGN = a dónde va · TCL = qué forma tiene.**
- **Ponderador = población / muestra.**
- **Masking = esconde outliers · Swamping = inunda de falsos outliers.**

---

# 10. ✅ Preguntas de autoevaluación

[⬆️ Volver al índice](#indice)

*(Tapá las respuestas y contestá de memoria. Las marcadas 🎯 son las que el docente mencionó.)*

1. 🎯 **¿Qué relación/diferencias hay entre análisis estadístico y minería de datos?** → Cuadro §1.6 (deductivo vs. inductivo, confirmatorio vs. exploratorio, con vs. sin supuestos, informática opcional vs. indispensable) + explicación.
2. 🎯 **¿Cuáles son las 3 V del Big Data y cuáles se suelen agregar? ¿Por qué no se define con un número?** → Volumen, velocidad, variedad (+ veracidad, valor). La capacidad de procesamiento crece y cualquier cifra queda chica.
3. 🎯 **Tipos de variables y ejemplo de cada una.** → Categórica, ordinal, discreta, continua.
4. **¿Qué es KDD y qué busca la minería de datos?** → Descubrimiento de conocimiento en bases de datos; patrones, relaciones y anomalías sin conocimiento previo.
5. **Estadística descriptiva vs. inferencial.** → Datos disponibles vs. muestra → universo.
6. 🎯 **¿Por qué es importante NumPy y qué caracteriza a `ndarray`?** → C/bajo nivel, memoria contigua, tamaño fijo, un solo tipo, más velocidad y menos memoria; base de Pandas y otras librerías; "parche" que une alto y bajo nivel.
7. **¿Por qué una lista de Python es más lenta/pesada que un array?** → Es mutable y heterogénea; reserva memoria de más.
8. **¿Qué es una Series y qué es un DataFrame? ¿Por qué no tienen `flatten`?** → §4.2.
9. **`loc` vs. `iloc`.** → Etiquetas vs. posiciones.
10. 🎯 **Diferencia entre valor atípico e inconsistente y cómo se trata cada uno.** → §5.4.
11. 🎯 **¿Qué es el Z-score y para qué sirve?** → Cuántos desvíos estándar se aleja un registro de la media; detecta atípicos.
12. **¿Cómo se detectan atípicos?** → Boxplot, Z-score, IQR, ML (multivariado: Mahalanobis, MCD/MVE, LOF).
13. **Patrones de no respuesta: ¿cuáles son y cuál es el más grave? ¿por qué?** → Completamente aleatoria, aleatoria, no aleatoria; la no aleatoria por el problema circular.
14. **¿Qué es un ponderador y cómo se calcula? ¿Qué es reponderar?** → Población/muestra; ajustarlo para que los respondentes representen a los no respondentes.
15. **Técnicas de imputación.** → Medias condicionadas, hot deck, modelos de ML (📖 también media/mediana, KNN, imputación múltiple).
16. **¿Qué hace la transformación logarítmica con los atípicos? ¿Y el Z-score?** → La log les quita influencia; el Z-score exagera distancias.
17. 🎯 **¿Qué tipo de medida es la mediana?** → Tendencia central **y** posición.
18. **¿Por qué la mediana es más robusta que la media?** → No depende de los valores extremos.
19. **Si la media podada es mayor que la aritmética, ¿qué indica?** → Atípicos hacia abajo (asimetría negativa).
20. **Varianza poblacional vs. muestral.** → /N vs. /(N−1) (evita subestimar la dispersión).
21. **¿Qué es el IQR y qué es el MAD?** → Q3−Q1; mediana de los desvíos absolutos respecto de la mediana.
22. **Covarianza vs. correlación de Pearson.** → La covarianza depende de la escala; la correlación la estandariza (−1 a 1). Ambas miden asociación lineal.
23. 🎯 **¿Cómo se interpreta una matriz de correlación?** → Diagonal = 1; signo = sentido; cerca de 0 = sin asociación; negativo = inversa.
24. **¿Qué medida usás para dos variables categóricas? ¿y numérica + categórica?** → V de Cramer; t de Student o eta.
25. **¿Qué representan n y p? ¿Cuántos parámetros hay con p = 5?** → n filas, p columnas; 2·5 + 5·4/2 = **20**.
26. 🎯 **Diferencia entre LGN y TCL. ¿Relación del TCL con el test de hipótesis?** → §2.
27. **¿Por qué Python se volvió el lenguaje de la IA?** → Legibilidad, NumPy, ecosistema (Pandas, TensorFlow, PyTorch), auge de la IA (*Attention Is All You Need*).
28. **¿Qué es ETL?** → Cargar, transformar y volver a guardar.
29. **¿Diferencia entre bases SQL y columnares?** → SQL por filas y consistencia; columnares por columnas y velocidad/disponibilidad.
30. 📖 **¿Qué son masking y swamping?** → Outliers que esconden a otros / observaciones normales clasificadas como outliers.
31. 📖 **¿Qué ventaja tiene Mahalanobis sobre la distancia euclídea?** → Pondera por la matriz de covarianzas y respeta la forma de la nube.
32. 📖 **¿Cuánto vale la traza de R? ¿Y qué representa la de Σ?** → p; suma de varianzas (variabilidad total).
33. 📖 **¿Quiénes son Quetelet, Galton y Fisher y qué aportaron?** → §1.5.
34. 📖 **Diferencia entre M2M, IoT, WoT e IoE.** → §1.5.
35. 📖 **¿Qué dice la regla de los tres desvíos? ¿Cuándo un outlier del boxplot es moderado y cuándo severo?** → $|t_i| > 3$ con $t_i = (x_i - \bar{x})/s$; moderado entre 1,5 y 3 × RI de la caja; severo a más de 3 × RI.
36. 📖 **¿Por qué la matriz de covarianzas de X e Y = −2X + 3 es singular?** → Son linealmente dependientes: Σ = [[2, −4], [−4, 8]] tiene determinante 0.
37. 📖 **¿Cuántos parámetros hay que estimar con *p* variables? ¿Y con p = 5?** → $2p + p(p-1)/2 = (p^2+3p)/2$; con p = 5, **20**.
38. 📖 **En una distribución con asimetría negativa, ¿cómo se ordenan media, mediana y moda?** → media < mediana < moda (en la positiva, al revés).
39. 📖 **Si la media no representa bien el centro, ¿qué medidas de dispersión usar?** → Rango intercuartílico y MAD (o MADN), no varianza, desvío ni CV.

---

# 11. 📋 Información de cursada

[⬆️ Volver al índice](#indice)

## Aprobación y asistencia 🗣
- **16 clases** (sin feriados); **4** dedicadas a parciales. Asistencia mínima **75 %** (**3 faltas** sobre 12 clases). **Hay que ponerse "presente" en el campus en cada clase.**
- **Regularizar:** **4 o más** en **ambos** parciales. **Promocionar:** **6 o más en ambos**.
- **Primer parcial:** teórico (2 de octubre). **Segundo parcial:** **trabajo práctico final** (entrega **virtual**; segunda mitad de la cursada; la defensa "se verá").
- **Integrador (11 de diciembre):** solo para quienes **no regularizaron**; **nota máxima 4**; **única** fecha para regularizar. También es fecha de **final** para quienes regularizaron (quienes promocionan no rinden final).
- El docente **tiende a adherir a los paros docentes** (única causa de cambios en el cronograma; la clase del 18/09 no se dictó).
- **Modalidad:** clases con código en **Python y R**; **libre elección de lenguaje/IDE** y **no se evalúa código**. El código visto en clase se comparte por **Google Colab** (hay que hacer copia propia para modificarlo).
- Materia de último cuatrimestre, de manejo flexible pero **exigiendo marcar asistencia en cada clase**.
- El profesor **no graba las clases**; sube el contenido de las diapositivas al campus.
- **Aprobación:** 6 o más en ambos parciales, o final en caso de no lograrlo.

## Bibliografía 🗣
| Texto | Uso |
|---|---|
| 🎯 Chan, D., Badano, C., Rey, A. (2019). ***Análisis inteligente de datos con lenguaje R*** (pp. 1-73). edUTecNe (UTN FRBA) | **Obligatoria y de cabecera.** Se ven los **dos primeros capítulos** (introducción a la minería de datos e introducción al análisis de datos). Ejemplos en **R**, pero "lo fundamental son los conceptos" |
| McKinney, W. (2023). ***Python para análisis de datos***. Ediciones Anaya Multimedia (trabajo original 2022) | Obligatoria. El autor creó Pandas; se usa más como **referencia práctica de Python** que conceptual |
| Mitchell, T. (1997). ***Machine Learning***. McGraw Hill | Optativa (modelado; clásico de **machine learning**) |
| Szretter Noste, M. E. (2017). ***Apunte de regresión lineal***. FCEyN, UBA | Optativa (modelado) |
| Zenaida Hernández, M. (2012). ***Métodos de análisis de datos*** (apuntes). Universidad de La Rioja | Optativa: perspectiva **estadística tradicional** |

- Apuntes y ejercicios en el campus: **"Materiales y exámenes unificados"**, carpeta *Apunte Fernández*, *Funcionamiento*.
- **Ejercicios:** cortos (~media hora por semana); sirven para parciales y TP. Clase 2: **levantar una base de microdatos**, la **EPH** (se usará en el TP).

## TP final 🗣
- Se trabaja con la **EPH** y **ponderadores** (hay varios; saber cuándo usar cada uno).
- Cualquier lenguaje/entorno: se evalúa **lo que obtienen con el código** y **aplicar bien los conceptos**.
- ⚠️ Aplicar técnicas de variables cuantitativas a categóricas → recuperatorio.
- Después del primer parcial (sin IA) en el segundo/TP **sí pueden usar IA**.

## Cronograma de clases y evaluaciones

*(Se va actualizando a medida que avanza la cursada; las clases que no se dictaron figuran como pendientes.)*

| Fecha | Clase / instancia | Estado |
|---|---|---|
| 21/8 | **Clase 1** — Conceptos fundamentales del análisis de datos | Dada |
| 28/8 | Sin clase | — |
| 4/9 | **Clase 2** — NumPy y Pandas (se dieron juntas por la falta de clase del 28/8) | Dada |
| 11/9 | **Clase 4** — Data cleaning y transformación de datos | Dada |
| 18/9 | No se dictó (paro docente) | — |
| 25/9 | **Clase 5** — Análisis exploratorio y estadística descriptiva | Dada |
| Sin fecha | **Clase 6** — Visualización de datos (prevista para el 25/9; se corrió para después del parcial) | Pendiente |
| **2/10** | 🟣 **Primer parcial teórico** (se mantiene pese al paro docente; **aula 308**) | — |
| 9/10 | **Clase 7** — Análisis de datos con R | Pendiente |
| **16/10** | 🟣 Recuperatorio del primer parcial | — |
| 23/10 | **Clase 8** — Integración de fuentes / SQL con pandas / Cassandra | Pendiente |
| 30/10 | **Clase 9** — Conceptos básicos del modelado de datos | Pendiente |
| 6/11 | **Clase 10** — Modelos de clasificación | Pendiente |
| 13/11 | **Clase 11** — Modelos de regresión | Pendiente |
| 20/11 | **Clase 12** — Modelos de clustering | Pendiente |
| **27/11** | 🟣 **Defensa del TP final** (segundo parcial; informe con bases de la EPH del INDEC) | — |
| **4/12** | 🟣 Recuperatorio del TP final | — |
| **11/12** | 🟢 Examen integrador (nota máx. 4) para quienes no regularizaron, y última instancia de finales | — |

> ⚠️ **Numeración:** el docente cuenta la clase del 11/9 como su "Clase 3" (por la fusión de NumPy y Pandas del 4/9), por eso en el campus los ejercicios pueden figurar como *"Ejercicios Clase 3-4"*. Otros archivos de ejercicios: *"Ejercicios Clase 2-1"* y *"ejercicios clase 4-6"*. Se encuentran en el campus, en *Materiales y exámenes → Ejercicios*.

## Recursos y herramientas

- **Herramientas de la materia:** `Python` · `R` · `SQL` · `Cassandra` · `Pandas` · `Google Colab`.
- **Colab (acceso directo):** [cuaderno de la materia](https://colab.research.google.com/drive/1x-5Rp6Erfq18CL7-0ANoI4189KSpoTMt?usp=sharing) · [Colab de la Clase 4 (data cleaning)](https://colab.research.google.com/drive/1_gDF8pJL1nT8uR4utQ8N-Lx-4gwa8EPS?usp=sharing).
- **Base de datos del TP:** [EPH 3.er trimestre 2024 (INDEC)](https://www.indec.gob.ar/ftp/cuadros/menusuperior/eph/EPH_usu_3_Trim_2024_txt.zip).

---

# 12. 🚫 Anexo: Álgebra lineal y Análisis de Componentes Principales (Cap. 3 del libro)

[⬆️ Volver al índice](#indice)

> 🚫 **El docente dijo que PCA y correspondencias NO entran en la materia.** Se conserva completo por si querés profundizar o para etapas posteriores.

> *"La vida es el arte de obtener conclusiones suficientes a partir de premisas insuficientes."* — Samuel Butler

## 12.1 Nociones previas de álgebra lineal
Para entender PCA se interpretan las variables como vectores en un espacio n-dimensional ($\mathbb{R}^n$).

**Vectores y operaciones:** $v = (v_1, \dots, v_n)$ es un segmento orientado desde el origen. **Suma:** $v + w = (v_1 + w_1, \dots, v_n + w_n)$. **Producto por escalar:** $\alpha v = (\alpha v_1, \dots, \alpha v_n)$.

**Combinación lineal:** $u$ es combinación lineal de $v$ y $w$ si existen $\alpha, \beta$ tales que $u = \alpha v + \beta w$. Las combinaciones de un vector forman una **recta**; las de dos de distinta dirección, un **plano**. Estadísticamente permite **crear nuevas variables** sin añadir dimensionalidad.

**Ejemplo (natación):** 14 nadadores, 4 tramos ($v_1..v_4$). $w_1 = \tfrac12 v_1 + \tfrac12 v_2$ (promedio de los dos primeros tramos), $w_2 = \tfrac12 v_3 + \tfrac12 v_4$ (promedio de los dos últimos), $w_3 = w_1 - w_2$ (diferencia). Todas pertenecen al espacio generado por las 4 originales.

**Dependencia e independencia lineal:**
- **Linealmente dependientes (l.d.):** el vector nulo se expresa como combinación lineal con algún coeficiente no nulo (al menos un vector es combinación del resto). **Variable redundante** (ej. altura en cm y en metros); dos vectores l.d. están sobre la misma recta.
- **Linealmente independientes (l.i.):** ningún vector es combinación de los otros; cada variable aporta **información única**.
- 📖 **Detalles del libro (Cap. 3.1):** el **vector nulo siempre** es combinación lineal de cualquier conjunto (todos los escalares en cero). Las combinaciones de un único vector son sus **múltiplos** (misma recta). Si dos vectores no nulos del plano **no tienen la misma dirección**, cualquier otro vector del plano es combinación de ellos. Ej. de vectores en $\mathbb{R}^2$: $u = (3, 0)$, $v = (1, 3)$, $w = (-2, 1)$. Dos vectores como $v = (a, a)$ y $-v = (-a, -a)$ son l.d. (su suma con escalares 1 da el nulo).
- 📖 **Lectura estadística:** que **tres variables sean l.d.** significa que la información de una es combinación lineal de las otras dos; que dos sean l.d. significa que una es **múltiplo** de la otra (la estatura en cm y en metros).

**Espacio generado y bases:**
- **$gen(T)$:** todos los vectores que se forman combinando los de $T$ (un vector genera una recta; dos independientes, un plano).
- **Base:** conjunto de vectores l.i. que genera todo el espacio; su cantidad es la **dimensión**. Base canónica de $\mathbb{R}^2$: $e_1 = (1, 0)$, $e_2 = (0, 1)$.

## 12.2 Transformaciones lineales
Se transforma el espacio original en otro (incluso de distinta dimensión). Las más frecuentes: **proyecciones, rotaciones y reflexiones (simetrías)**.

**Proyecciones (Ej. 3.2):** reducen dimensión "aplastando" los datos sobre un subespacio (ej. 3D a 2D). El objetivo condiciona la proyección:
- **PCA:** maximiza la **varianza** (la mayor "sombra" o dispersión).
- **Análisis discriminante:** **discrimina mejor las clases**, aunque sacrifique varianza.
- La proyección óptima **no es única**.

**Simetrías (Ej. 3.3):** reflexión respecto al eje de abscisas, $T: \mathbb{R}^2 \to \mathbb{R}^2$:

$$T(x, y) = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} x \\ -y \end{pmatrix}$$

**Involución** ($T \circ T = \text{id}$): con $M_E(T)$ la matriz en la base canónica,

$$M_E(T)^2 = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = I$$

Aplicar la transformación dos veces devuelve cada punto a su posición original.

---

# 13. 📝 Modelos de examen (simulacros)

[⬆️ Volver al índice](#indice)

> ⚠️ **Aclaración importante:** el docente dijo que **no hay modelo de parcial oficial** ("es estudiar más o menos lo que vimos y poder responder"). Estos dos simulacros los armé **a partir de lo que él mismo adelantó** (formato, temas y preguntas mencionadas). Sirven para practicar, no son el examen real.

## 13.1 Cómo están armados (y por qué)

| Lo que dijo el docente | Cómo se refleja en los modelos |
|---|---|
| Escrito, **hoja y lapicera**, sin celular ni IA | Se responde a mano y **con tus palabras** |
| **Preguntas teóricas a desarrollar + múltiple choice** | Cada modelo tiene **8 ítems de opción múltiple + 3 preguntas de desarrollo** |
| **100 % teórico**: sin cálculos ni código | No hay cuentas ni "qué hace tal función"; solo conceptos |
| Dura **no más de media hora** ("en general responden rápido") | Modelos cortos: ~10 min de múltiple choice + ~20 min de desarrollo |
| Seguro entra **análisis de datos vs. minería de datos** (a desarrollar) y **ciencia de datos vs. análisis de datos** | Una es el desarrollo 1 del Modelo 1 y la otra el desarrollo 1 del Modelo 2 |
| **Tipos de variables** ("recontra de parcial"), **mediana** (trampa), **Z-score**, **atípico vs. inconsistente**, **importancia de NumPy/`ndarray`**, **Big Data (3 V + 2)**, **interpretar matriz de correlación** | Todas aparecen al menos una vez entre los dos modelos |
| **Gráficos NO entran**, **PCA y correspondencias NO entran** | No hay preguntas de boxplot ni de visualización, ni de componentes principales |

> 💡 **Cómo usarlos:** tapá las claves, respondé **a mano** y cronometrate (30 min por modelo). Después comparás con la clave y con los "puntos que tu respuesta debería incluir". Las respuestas modelo están en bloques desplegables: hacé clic en **▶** para verlas.

---

## 13.2 Modelo 1

**Instrucciones:** hoja y lapicera · sin celular ni IA · tiempo sugerido: 30 minutos.

### Parte A — Opción múltiple (marcá **una** opción)

**1.** ¿Qué tipo de medida es la **mediana**?
- a) Solo una medida de tendencia central
- b) Solo una medida de posición
- c) Una medida de tendencia central **y** de posición
- d) Una medida de dispersión

**2.** La variable "calificación de la atención recibida" con valores *muy buena, buena, regular, mala, muy mala* es una variable:
- a) Categórica (cualitativa sin orden)
- b) Ordinal
- c) Cuantitativa discreta
- d) Cuantitativa continua

**3.** ¿Cuál **no** es una de las "V" asociadas al Big Data?
- a) Volumen
- b) Velocidad
- c) Veracidad
- d) Vectorización

**4.** Respecto de un `ndarray` de NumPy, es correcto que:
- a) Es mutable y puede mezclar tipos de datos libremente, igual que una lista
- b) Tiene tamaño fijo, todos sus elementos son del mismo tipo y ocupa memoria contigua
- c) Está escrito íntegramente en Python
- d) Solo puede tener una dimensión

**5.** Una persona que figura con **250 años** en una base de datos de edades es un valor:
- a) Atípico válido, que hay que conservar siempre
- b) Inconsistente, que debe corregirse o eliminarse
- c) Atípico, que depende del objetivo del análisis
- d) Un dato faltante

**6.** El **Z-score** de un registro indica:
- a) Cuántos casos representa ese registro en la población
- b) Qué porcentaje de datos hay por debajo de ese registro
- c) Cuántos desvíos estándar se aleja ese registro de la media
- d) La diferencia entre el máximo y el mínimo

**7.** En una matriz de correlación, un coeficiente de **−0,80** entre dos variables indica:
- a) Que no hay asociación entre ellas
- b) Una asociación lineal inversa fuerte
- c) Una asociación lineal directa fuerte
- d) Que una variable causa a la otra

**8.** Un procedimiento **inductivo, exploratorio y sin supuestos iniciales** corresponde a:
- a) La estadística clásica
- b) La minería de datos
- c) Ambas por igual
- d) Ninguna de las dos

### Parte B — Desarrollo

**1.** Desarrollá la **relación y las diferencias entre el análisis (estadístico) de datos y la minería de datos**. Incluí el cuadro comparativo y explicá cada punto.

**2.** Enumerá y definí los **tipos de variables**. Da un ejemplo de cada una y explicá por qué importa distinguirlas.

**3.** ¿Por qué es importante **NumPy**? Explicá las características de la clase **`ndarray`** y en qué se diferencia de una lista de Python.

<details>
<summary><strong>✅ Clave del Modelo 1 (hacé clic para desplegar)</strong></summary>

**Parte A:** 1-**c** · 2-**b** · 3-**d** · 4-**b** · 5-**b** · 6-**c** · 7-**b** · 8-**b**

- **1-c:** la mediana es la "pregunta trampa": divide el conjunto ordenado en dos partes iguales (posición) y es un valor central (tendencia central).
- **3-d:** las V son Volumen, Velocidad, Variedad (+ Veracidad y Valor).
- **5-b:** 250 años es imposible → inconsistente. (Una persona de 105 años sí sería atípica pero posible.)
- **7-b:** el signo negativo es asociación **inversa**, no "ausencia de asociación" (esa la marca un valor cercano a 0). Además, correlación no implica causalidad (descarta d).

**Parte B — puntos que tu respuesta debería incluir:**

**B1 (análisis estadístico vs. minería de datos)**
- Ambas sirven para analizar datos; la minería es parte del proceso **KDD** (descubrimiento de conocimiento en bases de datos): extraer patrones, relaciones y anomalías de grandes bases **sin conocimiento previo**.
- Cuadro: **hipotético-deductivo vs. inductivo** · **confirmatorias vs. exploratorias** · **con supuestos iniciales vs. sin supuestos iniciales** · **herramientas informáticas opcionales vs. indispensables**.
- Explicación: en la estadística se plantea una hipótesis y se contrasta con la realidad (aceptar/rechazar); en la minería se generaliza a partir de los datos y se explora, conviviendo con el error. Los supuestos son condiciones estadísticas (ej. normalidad), no hipótesis. La informática es indispensable por el volumen de datos.
- Contexto: la minería surge en el siglo XIX (Quetelet, Galton, Fisher) y hoy se vuelve necesaria por los volúmenes masivos de datos.

**B2 (tipos de variables)**
- **Categóricas:** no se ordenan (nombre, ciudad). **Ordinales:** se ordenan pero sin distancia entre valores (calificación de atención). **Cuantitativas discretas:** sin valores intermedios entre dos consecutivos, conteo (cantidad de hijos). **Cuantitativas continuas:** infinitos valores intermedios, medición (distancia, peso).
- Importa porque según el tipo **cambian los conteos, medidas y estimaciones aplicables** (no se calcula una media de una variable categórica).

**B3 (NumPy y `ndarray`)**
- NumPy (Numerical Python) está desarrollada en **C** (bajo nivel, tipado y compilado, manipula mejor la memoria): más **velocidad** y **menos memoria**.
- `ndarray`: **tamaño fijo**, **todos los elementos del mismo tipo** (excepto un vector de objetos), **memoria contigua** reservada estrictamente. La lista es mutable y heterogénea, priorizó la legibilidad y reserva memoria de más.
- Importancia: es la base de Pandas, TensorFlow, PyTorch, etc.; combina lo mejor de dos mundos (legibilidad de alto nivel + rendimiento de C); fue clave para que Python se volviera el lenguaje del análisis de datos y la IA.

</details>

---

## 13.3 Modelo 2

**Instrucciones:** hoja y lapicera · sin celular ni IA · tiempo sugerido: 30 minutos.

### Parte A — Opción múltiple (marcá **una** opción)

**1.** Si la **media podada** es **mayor** que la media aritmética, esto sugiere que:
- a) Hay valores atípicos hacia arriba (asimetría positiva)
- b) Hay valores atípicos hacia abajo (asimetría negativa)
- c) La distribución es perfectamente simétrica
- d) Hay datos duplicados

**2.** La **varianza muestral** se calcula dividiendo por:
- a) N
- b) N − 1
- c) N + 1
- d) La media

**3.** Según los umbrales vistos en clase, una tasa de no respuesta mayor al **30 %** se considera:
- a) Irrelevante
- b) Algo a tener en cuenta
- c) Importante
- d) Grave

**4.** Una no respuesta **no aleatoria** es la que:
- a) No tiene relación con ninguna variable del dataset
- b) Se explica por otra variable del dataset distinta de la de interés
- c) Se explica por la propia variable de interés, lo que genera un problema circular
- d) Se soluciona siempre con `dropna()`

**5.** En Pandas, `loc` e `iloc` se diferencian en que:
- a) `loc` usa posiciones numéricas e `iloc` usa etiquetas
- b) `loc` usa etiquetas e `iloc` usa posiciones numéricas
- c) `loc` es para filas e `iloc` solo para columnas
- d) No hay diferencia

**6.** Un **ponderador** se calcula como:
- a) Muestra / población
- b) Población / muestra
- c) Media / desvío estándar
- d) Q3 − Q1

**7.** ¿Cuál de estas afirmaciones sobre la **ley de los grandes números** y el **teorema central del límite** es correcta?
- a) La LGN dice que la distribución de las medias muestrales tiende a la normal
- b) El TCL dice que la media muestral se acerca al valor esperado
- c) La LGN dice que la media muestral se acerca al valor esperado al crecer la muestra, y el TCL que la distribución de las medias muestrales tiende a la normal
- d) Son el mismo concepto con distinto nombre

**8.** La **covarianza** se diferencia de la **correlación de Pearson** en que:
- a) La covarianza está estandarizada y va de −1 a 1
- b) La correlación depende de la escala de las variables
- c) La covarianza depende de la escala/unidad de medida, mientras que la correlación la estandariza
- d) La correlación mide solo asociaciones no lineales

### Parte B — Desarrollo

**1.** Desarrollá el concepto de **ciencia de datos** y de **análisis de datos**: qué es cada una, qué características tienen y qué diferencias/relaciones hay entre ambas.

**2.** Explicá la diferencia entre un **valor atípico** y un **valor inconsistente**. Da un ejemplo de cada uno, cómo se **detectan** (incluí qué es el **Z-score** y para qué sirve) y cómo se **tratan**.

**3.** Se analizaron tres variables en 200 personas que practican un instrumento. La matriz de correlación resultante es:

| | Horas de práctica | Errores cometidos | Edad |
|---|---|---|---|
| **Horas de práctica** | 1,00 | −0,78 | 0,03 |
| **Errores cometidos** | −0,78 | 1,00 | 0,10 |
| **Edad** | 0,03 | 0,10 | 1,00 |

Interpretá la matriz: qué significan los valores de la diagonal, cómo se lee cada par de variables y qué cuidados hay que tener al concluir.

<details>
<summary><strong>✅ Clave del Modelo 2 (hacé clic para desplegar)</strong></summary>

**Parte A:** 1-**b** · 2-**b** · 3-**d** · 4-**c** · 5-**b** · 6-**b** · 7-**c** · 8-**c**

- **1-b:** la media podada sube porque se quitan extremos bajos → los atípicos estaban hacia abajo (en la clase: media 711,73 < podada 740, asimetría −1,08).
- **2-b:** dividir por N−1 da un valor algo más alto y evita **subestimar** la dispersión con una muestra.
- **3-d:** 5 % (empezar a tenerla en cuenta) · 10 % (importante) · 30 % (grave).
- **4-c:** la "no aleatoria" depende de la propia variable de interés (ej. los de mayor ingreso son los que no responden la pregunta de ingreso) y no hay otra variable para corregirla.
- **6-b:** ponderador = cuántos casos de la población representa cada caso muestral (población / muestra).

**Parte B — puntos que tu respuesta debería incluir:**

**B1 (ciencia de datos vs. análisis de datos)**

> ⚠️ El docente **no dictó una definición formal de "ciencia de datos"**; la trató como uno de los conceptos "de moda" muy relacionados con los demás. Por eso conviene responder **con tus palabras** apoyándote en lo que sí se dijo (ver §1.3–1.6).

- **Análisis de datos:** proceso de **inspeccionar, limpiar y transformar** datos para resaltar información útil, sugerir conclusiones y apoyar la toma de decisiones; "darle contexto a los datos y contar una historia". Etapas: recolección → limpieza → transformación → exploración/visualización → interpretación → conocimiento accionable (con ida y vuelta entre etapas). Desde la mirada tradicional se reduce a estadística **descriptiva** (datos disponibles) o **inferencial** (de una muestra al universo); hoy **excede** ese campo con aprendizaje automático y minería de datos.
- **Ciencia de datos:** concepto más nuevo, surgido cuando la estadística tradicional ("cuadrada y rígida") se flexibilizó ante los grandes volúmenes de datos; está más ligado a la **informática**, al **machine learning**, la minería de datos y la IA.
- **Relación / diferencias:** son conceptos **muy relacionados entre sí**, que cambian con las modas (ciencia de datos → minería de datos → big data → IA) en una disciplina en **evolución permanente**. El análisis de datos es el proceso general; la ciencia de datos suma técnicas computacionales y de aprendizaje automático para datos masivos y no estructurados. En ambos: "hay grises, no hay blanco y negro"; el dato no habla solo, hay que contextualizarlo.

**B2 (atípico vs. inconsistente)**
- **Atípico:** alejado del patrón general pero **plausible/válido** (persona de 105 años; salario de un futbolista de élite; propiedad de Avellaneda cerca del río). **No necesariamente se excluye**: se inspecciona y depende del **objetivo** del análisis.
- **Inconsistente:** sin coherencia con el conjunto o con el conocimiento previo (persona de 250 años; propiedad "de Avellaneda" con coordenadas fuera del territorio). **Se corrige o se elimina**; nunca se usa.
- **Detección de atípicos:** **Z-score** = cuántos desvíos estándar se aleja un registro de la media (fórmula (X − media)/desvío); **mayor Z-score → más atípico** (ej.: edad media 46,9, desvío 23,4: 100 años → Z ≈ 2,38). También el **rango intercuartílico (IQR = Q3 − Q1)** y técnicas de aprendizaje automático.

**B3 (matriz de correlación)**
- La **diagonal vale 1**: cada variable consigo misma. La matriz es **simétrica**.
- **Práctica–Errores = −0,78:** asociación lineal **inversa y fuerte** (a más horas de práctica, menos errores). El signo negativo **no** significa "no hay correlación".
- **Práctica–Edad = 0,03** y **Errores–Edad = 0,10:** valores **cercanos a 0** → **poca o ninguna asociación lineal**.
- Cuidados: Pearson mide solo asociación **lineal** (puede haber relaciones no lineales que no capta); **correlación no implica causalidad**.

</details>

---

## 13.4 Autochequeo rápido antes de rendir

- [ ] Sé el **cuadro estadística vs. minería** de memoria (DE-CO-CON-opcional vs. IN-EX-SIN-indispensable).
- [ ] Puedo explicar **ciencia de datos vs. análisis de datos** con mis palabras.
- [ ] Sé las **5 V** del Big Data y por qué no se define con un número.
- [ ] Distingo **categórica / ordinal / discreta / continua** con ejemplos.
- [ ] Sé por qué **NumPy** es importante y qué caracteriza a `ndarray`.
- [ ] Distingo **atípico vs. inconsistente** y sé qué es el **Z-score**.
- [ ] Sé que la **mediana es central y de posición**.
- [ ] Puedo **interpretar una matriz de correlación** (diagonal, signo, cercano a 0, no causalidad).
- [ ] Distingo **LGN vs. TCL** y sé cómo se vincula el TCL con el test de hipótesis.
- [ ] Repasé los **capítulos 1 y 2 del libro**, los apuntes, el código visto y los **ejercicios** (recomendación del docente).
- [ ] Llevo **DNI, lapicera y dos hojas**; sin celular.

---

# 14. Glosario

[⬆️ Volver al índice](#indice)

> Términos agrupados por tema. La columna **Ver** indica la sección de la guía donde se desarrolla. Los marcados 🎯 son los que el docente mencionó como posible pregunta de parcial, 🚫 los que **no entran**, 📖 los del libro y ➕ los complementos que **no figuran en el PDF del libro**.

## Pares que se confunden

| Par | Diferencia en una línea |
|---|---|
| Estadística vs. minería de datos 🎯 | Deductivo, confirmatoria, con supuestos, informática opcional **vs.** inductivo, exploratoria, sin supuestos, informática indispensable |
| Descriptiva vs. inferencial | Describe **los datos disponibles** **vs.** generaliza de una **muestra** al universo |
| LGN vs. TCL 🎯 | "A dónde va" la media muestral (al valor esperado) **vs.** "qué forma tiene" la distribución de las medias (normal) |
| Atípico vs. inconsistente 🎯 | Raro pero **posible** (se analiza) **vs.** **imposible/incoherente** (se corrige o elimina) |
| Categórica vs. ordinal | Sin orden **vs.** con orden pero sin distancia entre valores |
| Discreta vs. continua | Sin valores intermedios (conteo) **vs.** infinitos intermedios (medición) |
| Tendencia central vs. posición | La **mediana** es **ambas** 🎯; media y moda solo central; cuartiles/deciles/percentiles solo posición |
| Varianza poblacional vs. muestral | Divide por **N** **vs.** por **N − 1** (evita subestimar la dispersión) |
| Covarianza vs. correlación 🎯 | Depende de la escala/unidades **vs.** estandarizada entre −1 y 1 |
| Negativo vs. "sin correlación" | −0,8 es asociación **inversa fuerte**; la ausencia de asociación es un valor **cerca de 0** |
| No respuesta completamente aleatoria vs. aleatoria vs. no aleatoria | Sin patrón (no sesga) **vs.** explicada por **otra** variable **vs.** explicada por la **propia** variable de interés (la más grave) |
| Imputación vs. reponderación | **Rellenar** el valor faltante **vs.** **ajustar el ponderador** para que los que respondieron representen a los que no |
| `loc` vs. `iloc` | Etiquetas/nombres **vs.** posiciones numéricas |
| Series vs. DataFrame | Vector 1D etiquetado **vs.** tabla 2D construida sobre Series |
| Lista de Python vs. `ndarray` | Mutable, heterogénea, más lenta y pesada **vs.** tamaño fijo, un solo tipo, memoria contigua |
| SQL vs. columnares | Por **filas** y consistencia **vs.** por **columnas** y velocidad |
| Masking vs. swamping 📖 | Outliers que **esconden** a otros **vs.** normales que **parecen** outliers |
| PCA vs. discriminante 🚫 | Maximiza la **varianza** **vs.** maximiza la **separación de clases** |

## Datos, análisis y minería de datos

| Término | Definición breve | Ver |
|---|---|---|
| **Dato** | Representación de un hecho, observación o característica; solo, carece de contexto | §1.1 |
| **Registro / variable** | Fila (individuo/caso) / columna (característica medida) de una tabla | §1.2 |
| **Datos estructurados / semiestructurados / no estructurados** | Tablas / JSON, XML, CSV, logs, APIs / texto, imagen, audio, video | §1.2 |
| **Análisis de datos** | Inspeccionar, limpiar y transformar datos para resaltar información útil, sugerir conclusiones y apoyar decisiones | §1.3–1.4 |
| **Conocimiento accionable** | Resultado final del proceso: decisiones, solución de problemas, respuestas | §1.3 |
| **Web scraping** | Extraer datos de una web; excepción en que el analista sí recolecta | §1.3 |
| **Ciencia de datos** | Concepto "de moda", muy relacionado con minería de datos, machine learning e IA; más ligado a la informática (no hay definición formal dictada) | §1.4–1.5 |
| **Estadística descriptiva / inferencial** | Datos disponibles / de una muestra al universo | §1.4 |
| **Población (universo) / muestra** | Conjunto total / recorte que se observa; debe ser representativo | §1.4, §2.1 |
| **KDD** | *Knowledge Discovery in Databases*: proceso de descubrimiento de conocimiento; el Data Mining es su fase analítica | §1.5 |
| **Data Mining (minería de datos)** | Extraer patrones, relaciones y anomalías de grandes bases **sin conocimiento previo**; multidisciplinaria | §1.5 |
| **Big Data / las 5 V** 🎯 | Volumen, velocidad, variedad (+ veracidad, valor); se define como concepto, no por una cifra | §1.5 |
| **Machine Learning (aprendizaje automático)** | Modelos que aprenden de los datos (árboles, ensambles, redes neuronales); intentan no requerir supuestos | §1.4, §1.6 |
| **Inteligencia artificial / AGI** | Campo más amplio; la IA general razonaría con el método hipotético-deductivo (los modelos actuales generalizan, inductivo) | §1.6 |
| **Alucinación** | Error de un modelo de IA que genera algo falso; el error se reduce pero no se elimina | §1.6 |
| **LLM** | Modelo de lenguaje; trabaja con datos no estructurados | §1.2 |
| **Método hipotético-deductivo / inductivo** | Contrastar una hipótesis con la realidad / generalizar desde los datos | §1.6 |
| **Técnicas confirmatorias / exploratorias** | Aceptar o rechazar una hipótesis / explorar sin aceptar ni rechazar | §1.6 |
| **Supuestos estadísticos** | Condiciones matemáticas que deben cumplirse (ej. normalidad); no son hipótesis | §1.6 |
| **M2M / IoT / WoT / IoE** 📖 | Máquinas entre sí / objetos en internet / objetos en la Web / personas-procesos-datos-cosas | §1.5 |
| **Quetelet · Galton · Fisher** 📖 | Regularidad estadística del delito · correlación, regresión y encuestas · análisis de la varianza (Rothamsted) | §1.5 |
| **RFID / Kevin Ashton** 📖 | Identificadores por radiofrecuencia; Ashton acuñó "IoT" en 1999 (MIT, Centro de Auto-ID) | §1.5 |
| **Univariado / bivariado / multivariado** | Una / dos / más de dos variables | §1.8 |

## Tecnologías

| Término | Definición breve | Ver |
|---|---|---|
| **SQL** | Base relacional por filas; prioriza persistencia y consistencia | §1.9 |
| **NoSQL** | Prioriza velocidad y disponibilidad sobre la consistencia total | §1.9 |
| **Base columnar (Cassandra)** | Trabaja columna por columna; útil para análisis | §1.9 |
| **ETL** | Cargar, transformar y volver a guardar los datos | §5.1 |
| **Python** | Legible, multiparadigma (Guido van Rossum, 1989); lenguaje de la IA | §1.9 |
| **R** | Lenguaje especializado en análisis de datos | §1.9 |
| **Google Colab** | Notebooks en la nube con Python + Markdown; hay que guardar una copia en Drive | §1.9 |
| **Kaggle** | Plataforma con datasets, notebooks y competencias | §4.7 |
| **EPH** | Encuesta Permanente de Hogares (INDEC); base de microdatos del TP con varios ponderadores | §4.8, §5.3 |

## NumPy y Pandas

| Término | Definición breve | Ver |
|---|---|---|
| **NumPy** 🎯 | *Numerical Python*: escrita en C, manipula arrays multidimensionales con más velocidad y menos memoria | §3 |
| **`ndarray`** 🎯 | Clase base de NumPy: tamaño fijo, un solo tipo, memoria contigua | §3.2 |
| **`ndim`, `shape`, `dtype`, `size`, `itemsize`, `T`** | Dimensiones, forma, tipo, cantidad de elementos, bytes por elemento, transpuesta | §3.3 |
| **`flatten()` / `reshape()`** | Pasar a una dimensión / cambiar la forma (no existen en Series ni DataFrame) | §3.3, §4.2 |
| **`arange` / `linspace`** | `range` con decimales / intervalos regulares | §3.3 |
| **RGB** | Imagen a color = tres matrices superpuestas (rojo, verde, azul) | §3.5 |
| **Pandas** | Librería de DataFrames creada por Wes McKinney (2008); usa `ndarray` por dentro | §4.1 |
| **Series / DataFrame** | Vector 1D etiquetado / tabla 2D | §4.2 |
| **Index (índice)** | Etiquetas de filas; simplifica el acceso y el filtrado | §4.5 |
| **`loc` / `iloc`** | Acceso por etiquetas / por posiciones | §4.5 |
| **`query()`** | Filtra filas con sintaxis estilo SQL | §4.4 |
| **`describe()`** | Conteo, media, desvío, mínimo, Q1, mediana, Q3, máximo | §4.2 |
| **`drop_duplicates()` / `dropna()`** | Elimina duplicados / elimina filas con nulos | §5.2–5.3 |
| **`to_datetime()`, accesores `dt` y `str`** | Convierte a fecha; accede a año/mes/día; aplica funciones de texto | §4.6 |
| **`groupby()` / `merge()`** | Agrupa por columna / une tablas | §4.2 |

## Ley de grandes números, TCL y test de hipótesis

| Término | Definición breve | Ver |
|---|---|---|
| **Ley de los grandes números** 🎯 | Con más ensayos/muestra, la frecuencia relativa o la media muestral converge a su valor teórico (Bernoulli, s. XVII) | §2.1 |
| **Teorema central del límite** 🎯 | La distribución de las medias muestrales tiende a la normal si la varianza poblacional es finita | §2.2 |
| **Distribución normal** | Curva de campana de Gauss | §2.2 |
| **Hipótesis nula (H₀)** | Afirmación de "no hay diferencia" que se busca rechazar | §2.3 |
| **Error estándar** | Desvío estándar de la media muestral | §2.3 |
| **p-valor** | Probabilidad de obtener el resultado observado (o más extremo) si H₀ fuera cierta | §2.3 |
| **Significancia (0,05)** | Umbral típico para rechazar H₀ | §2.3 |
| **Test t / test z / ANOVA** | Tests paramétricos que se apoyan en el TCL | §2.3 |

## Data cleaning

| Término | Definición breve | Ver |
|---|---|---|
| **Valor duplicado** | Registro repetido; sobrerrepresenta y sesga; se define un criterio (ID o combinación de columnas) | §5.2 |
| **Valor nulo / `NA`** | Campo vacío | §5.3 |
| **No respuesta parcial** | Registro con algunos campos vacíos | §5.3 |
| **Tasa de no respuesta (5–10–30)** | >5 % a considerar, >10 % importante, >30 % grave | §5.3 |
| **Completamente aleatoria / aleatoria / no aleatoria** | Ver tabla de pares; semáforo verde / amarillo / rojo | §5.3, §8.5 |
| **Problema circular** | En la no aleatoria, falta justo la información necesaria para corregir | §5.3 |
| **Listwise deletion** ➕ | Borrar toda la fila con faltantes; solo si son muy pocos (~<5 %) | §5.3 |
| **Imputación** | Reemplazar el faltante por un valor estimado | §5.3 |
| **Medias condicionadas** | Imputar la media del grupo; la técnica más básica | §5.3 |
| **Hot deck** | Copiar el valor de un caso similar elegido al azar; las variables deben relacionarse con la imputada | §5.3 |
| **Imputación múltiple / KNN** ➕ | Métodos basados en modelos para predecir el faltante | §5.3 |
| **Ponderador** | Casos de la población que representa cada caso muestral = población / muestra | §5.3 |
| **Reponderación** | Ajustar ponderadores para compensar la no respuesta | §5.3 |
| **Muestreo polietápico** | Diseño del INDEC; ponderador = producto de probabilidades de selección | §5.3 |
| **Valor atípico (outlier)** 🎯 | Alejado del patrón pero plausible | §5.4 |
| **Valor inconsistente** 🎯 | Sin coherencia con el conjunto o el conocimiento previo | §5.4 |
| **Z-score** 🎯 | Cuántos desvíos estándar se aleja un registro de la media; mayor Z = más atípico | §5.4, §6.1 |
| **Boxplot (gráfico de cajas)** | Caja = IQR, línea = mediana, puntos = atípicos (más allá de 1,5 × RI) | §5.4 |
| **Outlier moderado / severo** 📖 | A más de 1,5 × RI / a más de 3 × RI de la caja | §5.4 |
| **Regla de los tres desvíos** 📖 | Outlier si \|t\| > 3 con t = (x − media)/s | §5.4 |
| **Valor adyacente (VAS / VAI)** 📖 | Mayor dato menor que Q3 + 1,5·RI / menor dato mayor que Q1 − 1,5·RI | §5.4 |
| **Control univariado vs. multivariado** 📖 | Límites en una variable vs. elipse de confianza que detecta puntos que rompen la forma de la interacción | §5.4 |

## Transformaciones

| Término | Definición breve | Ver |
|---|---|---|
| **Transformación por variables / por individuos** | Sobre columnas / sobre filas | §6 |
| **Centrado** ➕ | Restar la media; media 0, conserva la varianza | §6.1 |
| **Estandarización (Z-score)** | (x − media)/desvío; media 0, varianza 1 | §6.1 |
| **Min-max** | Lleva a [0, 1]; no es una "normalización" a la campana | §6.1 |
| **Logarítmica** | log(x + 1); reduce la influencia de atípicos y corrige asimetría a derecha | §6.1 |
| **Raíz cuadrada / Box-Cox** ➕ | Útil para conteos / busca la mejor potencia λ para normalizar | §6.1 |
| **Neutralización de jueces** | Normaliza por la media, máximo y mínimo de cada individuo | §6.2 |
| **Perfiles (relativización por el total)** ➕ | Cada fila suma 1 | §6.2 |
| **Norma euclídea** ➕ | Cada vector-individuo queda de longitud 1 | §6.2 |

## Estadística descriptiva

| Término | Definición breve | Ver |
|---|---|---|
| **Frecuencia absoluta / relativa / porcentual** | Conteo / proporción / proporción × 100 | §7.2 |
| **Intervalos de clase** | Agrupamiento de variables cuantitativas (ej. 0–16, 17–30…) | §7.2 |
| **Frecuencia acumulada (Fᵢ)** 📖 | Suma de las frecuencias absolutas hasta la categoría *k* | §7.2 |
| **Estadísticos de orden** 📖 | Datos ordenados x₍₁₎ ≤ … ≤ x₍ₙ₎; el mínimo y el máximo son casos particulares | §7.3 |
| **Media aritmética** | Suma / cantidad; no robusta | §7.3 |
| **Media geométrica** | Raíz enésima del producto; menos afectada por extremos altos | §7.3 |
| **Media podada (alfa-podada)** | Media tras quitar un % de extremos | §7.3 |
| **Mediana** 🎯 | Valor central; robusta; central y de posición | §7.3 |
| **Moda** | Valor de mayor frecuencia | §7.3 |
| **Cuantiles** | Cuartiles (4), quintiles (5), deciles (10), percentiles (100) | §7.3 |
| **Robustez** | Poca sensibilidad a valores extremos | §7.3 |
| **Rango** | Máximo − mínimo | §7.3 |
| **Varianza / desvío estándar** | Dispersión alrededor de la media / su raíz (unidades originales) | §7.3 |
| **Coeficiente de variación** | Desvío / media; compara dispersión entre conjuntos | §7.3 |
| **IQR (rango intercuartílico)** | Q3 − Q1 | §7.3 |
| **MAD / MADN** | Mediana de desvíos absolutos respecto de la mediana / versión normalizada | §7.3 |
| **Asimetría** | Simétrica, positiva (a derecha) o negativa (a izquierda) | §7.3 |
| **Coeficientes de Fisher–Pearson, Pearson y Bowley** | Asimetría con la media / (media − moda)/desvío / con cuartiles | §7.3 |
| **Curtosis** | Apuntamiento: leptocúrtica, mesocúrtica, platicúrtica | §7.3 |
| **Histograma / polígono de frecuencias** 📖🚫 | Histograma para continuas; el polígono une los puntos medios de las barras. (KDE y tallo y hojas ➕ no figuran en el PDF) | §7.3 |

## Bivariado y multivariado

| Término | Definición breve | Ver |
|---|---|---|
| **Tabla de doble entrada** | Frecuencias de dos variables cruzadas | §7.4 |
| **Gráfico de dispersión** 📖 | Un punto por observación (xᵢ, yᵢ) | §7.4 |
| **Covarianza** | Variabilidad conjunta lineal; depende de la escala | §7.4 |
| **Correlación de Pearson** 🎯 | Covarianza estandarizada (−1 a 1); solo asociación lineal | §7.4 |
| **Correlación de Spearman** | Basada en rangos; menos sensible a extremos | §7.4 |
| **V de Cramer / t de Student / eta** | Categórica–categórica / numérica–categórica | §7.4 |
| **Matriz de correlación** 🎯 | Diagonal = 1, simétrica; signo = sentido; cerca de 0 = sin asociación | §7.4 |
| **Correlograma / heatmap** | Visualiza la matriz por color (azul positivo, rojo negativo) | §7.4 |
| **Correlación ≠ causalidad** | Una asociación alta no prueba que una variable cause la otra | §7.4 |
| **Clustering** | Agrupar variables o casos similares | §7.4 |
| **n y p** | Filas (registros) y columnas (variables) | §7.5 |
| **Nº de parámetros** | 2p + p(p − 1)/2 (medias, varianzas y covarianzas) | §7.5 |
| **Matriz Σ / matriz R** 📖 | Covarianzas (diagonal = varianzas) / correlaciones (diagonal = 1) | §7.5 |
| **Traza tr(Σ) / tr(R)** 📖 | Suma de varianzas / igual a p | §7.5 |
| **Matriz singular** 📖 | det(Σ) = 0 por dependencia lineal (información redundante) | §7.4 |
| **Matriz semidefinida positiva** 📖 | Σ tiene todos los autovalores ≥ 0 | §7.5 |
| **Vector de medias** 📖 | Media de cada variable (columna) | §7.5 |

## Gráficos y exploración multivariada 📖🚫

| Término | Definición breve | Ver |
|---|---|---|
| **Diagrama circular / de barras / de bastones** | Cualitativas y ordinales / cualitativas (conjuntas: superpuestas, adyacentes) / discretas | §7.3 |
| **Reglas de Sturges, Velleman, Dixon–Kronmal** | Número *k* de intervalos del histograma según *n* | §7.3 |
| **Reglas de Scott y Freedman–Diaconis** | Ancho de los intervalos según el desvío estándar / el rango intercuartil | §7.3 |
| **Tabla de clasificación cruzada** | Distribución conjunta de dos variables | §7.5 |
| **Gráfico de mosaicos** | Distribuciones conjuntas de variables categóricas | §7.5 |
| **Dispersograma** | Matriz de dispersión de a pares | §7.5 |
| **Coordenadas paralelas** | Ejes paralelos escalados; cada individuo es una línea | §7.5 |
| **Perfiles multivariados** | Medias o medianas de cada variable por grupo | §7.5 |
| **Curvas de nivel** | Puntos de igual densidad (normal bivariada) | §7.5 |
| **Gráfico de estrellas** | Un radio por variable cuantitativa; compara individuos o grupos | §7.5 |
| **Caras de Chernoff** | Variables asociadas a rasgos de una cara | §7.5 |
| **Tukey** | Propuso el boxplot (1915-2000) | §5.4 |

## Estadística robusta multivariada 📖

| Término | Definición breve | Ver |
|---|---|---|
| **Masking / swamping** | Outliers que esconden a otros / normales que parecen outliers | §5.4 |
| **Distancia de Mahalanobis** | Pondera por Σ⁻¹; respeta la forma de la nube | §5.4 |
| **Vector de medianas** | Reemplazo robusto del vector de medias | §5.4 |
| **MVE** | Elipsoide de menor volumen que cubre una submuestra mayoritaria | §5.4 |
| **MCD / FAST-MCD** | Subconjunto cuya matriz de covarianzas tiene el menor determinante / algoritmo eficiente | §5.4 |
| **LOF** | *Local Outlier Factor*: anomalías locales por densidad con los k vecinos más cercanos | §5.4 |

## Álgebra lineal y PCA 🚫

| Término | Definición breve | Ver |
|---|---|---|
| **Combinación lineal** | u = αv + βw; crea nuevas variables sin agregar dimensiones | §12.1 |
| **Linealmente dependientes (l.d.)** | Al menos un vector es combinación del resto: variable redundante | §12.1 |
| **Linealmente independientes (l.i.)** | Ninguno es combinación de los demás: información única | §12.1 |
| **Espacio generado** | Todo lo que se forma combinando linealmente un conjunto de vectores | §12.1 |
| **Base y dimensión** | Conjunto l.i. que genera el espacio; su tamaño es la dimensión | §12.1 |
| **Base canónica** | Versores e₁ = (1, 0), e₂ = (0, 1)… | §12.1 |
| **Proyección** | Reduce la dimensión "aplastando" los datos sobre un subespacio | §12.2 |
| **PCA** | Proyección que maximiza la varianza | §12.2 |
| **Análisis discriminante** | Proyección que separa mejor las clases | §12.2 |
| **Simetría / involución** | Reflexión; T∘T = id, es decir M² = I | §12.2 |

---

*Fin de la guía unificada · ¡Éxitos en el parcial del viernes 2 de octubre! 🚀*
