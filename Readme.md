Introducción al Análisis de Datos  
Apuntes de cursada y material de clase de la materia **Introducción al Análisis de Datos** (Tecnicatura Universitaria en Programación, UTN Facultad Regional Avellaneda). El objetivo del repositorio es centralizar lo que se va viendo en cada clase, dejar registro de los conceptos y consignas del profesor, y servir de referencia rápida para repasar antes de los parciales.  
**Cursada:** 2do. cuatrimestre 2026  
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANUlEQVR4nO3OMQ2AABAAsSPBCj7fFwtCmJHAjAU2QtIq6DIzW7UHAMBfnGt1V8fHEQAA3rsexOkF3va0dq8AAAAASUVORK5CYII=)  
🧭 Índice  
- [**Funcionamiento de la materia**](#anchor-1 "#anchor-1")  
  - [Modalidad y criterios de evaluación](#anchor-2 "#anchor-2")  
  - [Exámenes](#anchor-3 "#anchor-3")  
  - [Cronograma de clases](#anchor-4 "#anchor-4")  
  - [Bibliografía](#anchor-5 "#anchor-5")  
  - [Herramientas](#anchor-6 "#anchor-6")  
- [**Clase 1 — 21/8 · Conceptos fundamentales del análisis de datos**](#anchor-7 "#anchor-7")  
  - [Dato y tipos de datos](#anchor-8 "#anchor-8")  
  - [¿De qué trata el análisis de datos?](#anchor-9 "#anchor-9")  
  - [Data Mining y Big Data](#anchor-10 "#anchor-10")  
  - [Análisis estadístico vs. Minería de datos](#anchor-11 "#anchor-11")  
  - [Tipos de variables](#anchor-12 "#anchor-12")  
  - [Clasificación del análisis según cantidad de variables](#anchor-13 "#anchor-13")  
  - [Evolución tecnológica del lenguaje dominante](#anchor-14 "#anchor-14")  
  - [Ley de los grandes números](#anchor-15 "#anchor-15")  
  - [Teorema central del límite](#anchor-16 "#anchor-16")  
  - [Relación entre el TCL y el test de hipótesis](#anchor-17 "#anchor-17")  
  - [Notas de la clase](#anchor-18 "#anchor-18")  
- [**Clase 2 — 28/8 · Numpy***(pendiente)*](#anchor-19 "#anchor-19")  
- [**🟣 2/10 · Primer parcial teórico**](#anchor-20 "#anchor-20")  
- [**Clase 7 — 9/10 · Análisis de datos con R***(pendiente)*](#anchor-21 "#anchor-21")  
- [**🟣 16/10 · Recuperatorio primer parcial**](#anchor-22 "#anchor-22")  
- [**Clase 8 — 23/10 · Integración de fuentes / SQL con pandas / Cassandra***(pendiente)*](#anchor-23 "#anchor-23")  
- [**Clase 9 — 30/10 · Conceptos básicos del modelado de datos***(pendiente)*](#anchor-24 "#anchor-24")  
- [**Clase 10 — 6/11 · Modelos de clasificación***(pendiente)*](#anchor-25 "#anchor-25")  
- [**Clase 11 — 13/11 · Modelos de regresión***(pendiente)*](#anchor-26 "#anchor-26")  
- [**Clase 12 — 20/11 · Modelos de clustering***(pendiente)*](#anchor-27 "#anchor-27")  
- [**🟣 27/11 · Defensa TP final**](#anchor-28 "#anchor-28")  
- [**🟣 4/12 · Recuperatorio TP final**](#anchor-29 "#anchor-29")  
- [**🟢 11/12 · Instancia de finales y última instancia de recuperatorio**](#anchor-30 "#anchor-30")  
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANklEQVR4nO3OQQmAABRAsSfYxZo/jzlMYQLPJrCCNxG2BFtmZquOAAD4i3Ot7mr/egIAwGvXA4q7Bc870TqdAAAAAElFTkSuQmCC)  
🗓️ Funcionamiento de la materia  
[![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAADUlEQVR4nGP4//8/AwAI/AL+p5qgoAAAAABJRU5ErkJggg==)  
](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/LautaroSantiago/Introduccion-Analisis-Datos-UTN/master/Material/0%20-%20Funcionamiento.pdf "https://docs.google.com/viewer?url=https://raw.githubusercontent.com/LautaroSantiago/Introduccion-Analisis-Datos-UTN/master/Material/0%20-%20Funcionamiento.pdf")  
Modalidad y criterios de evaluación  
- **Modalidad:** clases con código en Python y R. Libre elección de lenguaje/IDE —  **no se evalúa código**. El código visto en clase se comparte por Google Colab (hay que hacer copia propia para poder modificarlo).  
- **Asistencia:** se exige 75% (máximo 3 faltas en el cuatrimestre).  
- **Regularidad:** 4 o más en ambos parciales.  
- **Aprobación:** 6 o más en ambos parciales, o final en caso de no lograrlo.  
Exámenes  
| | | |  
|-|-|-|  
| **Instancia** | **Fecha** | **Detalle** |   
| Primer parcial | 2/10 | Teórico y virtual |   
| Recuperatorio 1er parcial | 16/10 | — |   
| Segundo parcial (TP final) | — | Informe utilizando las bases de la Encuesta Permanente de Hogares (INDEC) |   
| Defensa TP final | 27/11 | — |   
| Recuperatorio TP final | 4/12 | — |   
| Finales / última instancia de recuperatorio | 11/12 | Examen integrador (nota máx. 4) para quienes no regularizaron |   
   
Cronograma de clases  
Cada clase se despliega individualmente con su desarrollo completo adentro. Se va actualizando a medida que avanza la cursada — las que todavía no se dictaron dicen *"pendiente"*.  
**Clase 1 — 21/8 · Conceptos fundamentales del análisis de datos**  
[![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAADUlEQVR4nGP4//8/AwAI/AL+p5qgoAAAAABJRU5ErkJggg==)  
](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/LautaroSantiago/Introduccion-Analisis-Datos-UTN/master/Material/1%20-%20Clase%201.pdf "https://docs.google.com/viewer?url=https://raw.githubusercontent.com/LautaroSantiago/Introduccion-Analisis-Datos-UTN/master/Material/1%20-%20Clase%201.pdf")  
*Dato y tipos de datos*  
**Dato:** representación de un hecho, una observación o una característica de un objeto, persona o evento, expresada mediante números, texto, fecha, símbolos o cualquier otro formato. Por sí solo, un dato carece de contexto y significado suficiente para tomar decisiones. *Ejemplos: 38.5, "Azul", 2026-08-04, 125, "Juan Pérez".*  
**Tipos de datos según su estructura:**  
- **Estructurados:** organizados en tablas (filas/columnas). Ej: bases de datos relacionales.  
- **Semiestructurados:** XML, JSON, CSV, logs, APIs.  
- **No estructurados:** texto libre, imágenes, audio, video, redes sociales.  
*¿De qué trata el análisis de datos?*  
Proceso de **recolección** (bases de datos, archivos, encuestas) →  **limpieza** →  **transformación** →  **exploración y visualización** →  **análisis e interpretación** →  **conocimiento accionable** (toma de decisiones, resolución de problemas, respuestas a preguntas).  
***Definición (Wikipedia):*** * "El análisis de datos es un proceso que consiste en inspeccionar, limpiar y transformar datos con el objetivo de resaltar información útil, para sugerir conclusiones y apoyo en la toma de decisiones."*  
**Perspectiva académica:** una visión más ligada a la estadística reduce el análisis de datos a estadística descriptiva (analiza los datos disponibles) o inferencial (a partir de una muestra de un universo, genera predicciones/definiciones generales para ese universo). En la práctica actual, el analista de datos excede ese campo tradicional y recurre también al aprendizaje automático y la minería de datos.  
*Data Mining y Big Data*  
- La minería de datos (*data mining*) surge en el siglo XIX con el análisis de los datos sociales de Quetelet, biológicos de Galton y agronómicos de Fisher.  
- Forma parte del proceso conocido como **KDD** (*Knowledge Discovery in Databases* — descubrimiento de conocimiento a partir de los datos): el objetivo es extraer información de una gran base de datos, sin disponer de conocimiento previo, para construir patrones y/o relaciones sistemáticas de valor, así como anomalías.  
- **Big Data — las 5 "V":** Volumen, Velocidad y Variedad como las tres centrales; Veracidad y Valor como las dos adicionales a tener en cuenta.  
*Análisis estadístico vs. Minería de datos*  
| | |  
|-|-|  
| **Análisis estadístico** | **Minería de datos** |   
| Procedimiento hipotético deductivo | Procedimiento inductivo |   
| Técnicas confirmatorias | Técnicas exploratorias |   
| Supuestos iniciales | Sin supuestos iniciales |   
| Herramientas informáticas opcionales | Recursos informáticos indispensables |   
   
*Tipos de variables*  
- **Categóricas:** cualitativas, no se pueden ordenar.  
- **Ordinales:** se pueden ordenar, pero no se puede establecer distancia entre valores.  
- **Cuantitativas discretas:** numéricas; entre dos valores consecutivos no poseen valores intermedios.  
- **Cuantitativas continuas:** numéricas; entre dos valores poseen infinitos valores intermedios.  
*Clasificación del análisis según cantidad de variables*  
| | |  
|-|-|  
| **Univariado** | **Bivariado o multivariado** |   
| Análisis de una sola variable a la vez. | Se analizan dos o más variables, a nivel de su relación, dependencia o patrones. |   
| Medidas de tendencia central (media, mediana, moda) o de dispersión (varianza, rango) u otras (curtosis). | Ej: clusterización de clientes de una empresa, regresión entre edad y peso. |   
| Ejemplo: media etaria del aula. |   |   
   
*Evolución tecnológica del lenguaje dominante*  
Históricamente **C** fue el lenguaje más usado. Con el tiempo,  **R** creció fuerte hasta ubicarse en el top 10, siendo un lenguaje enfocado exclusivamente en análisis de datos, mientras C fue perdiendo terreno. En 2017 aparece el paper *"Attention Is All You Need"*, que impulsa la explosión de la inteligencia artificial. Desde entonces, **Python** asciende hasta convertirse en el lenguaje más usado, superando a R, por ser el lenguaje de la IA y del procesamiento de grandes volúmenes de datos.  
*Ley de los grandes números*  
Formulada originalmente por **Jacob Bernoulli** en el siglo XVII: la frecuencia relativa de un evento tiende a converger hacia su probabilidad teórica a medida que aumenta el número de ensayos. En el contexto de la estadística inferencial: a medida que crece el tamaño de una muestra tomada de una población, la media muestral tiende a aproximarse cada vez más al valor esperado (esperanza matemática) de la población.  
- **Implicancia práctica:** no se pueden sacar conclusiones definitivas sobre fenómenos masivos a partir de casos aislados; hace falta una muestra representativa y lo suficientemente grande.  
- **Vínculo con la IA:** el salto de capacidad entre modelos (ej. GPT-2 a GPT-3) se explica en gran parte por el volumen de datos de entrenamiento — es una cuestión de escala, no solo conceptual.  
*Teorema central del límite*  
Desarrollado originalmente entre los siglos XVIII y XIX, y reformulado hasta el siglo XX. Establece que, dada una población con cualquier distribución, la distribución de las medias muestrales tiende a una distribución normal a medida que aumenta el tamaño de la muestra, siempre que la varianza poblacional sea finita.  
- Permite, conociendo las propiedades de la distribución normal, testear si una diferencia observada entre dos grupos (ej. rendimiento de dos semillas, una original y una modificada genéticamente) es significativa o no.  
*Relación entre el TCL y el test de hipótesis*  
*(Consigna del profesor para investigar.)*  
El test de hipótesis necesita saber qué forma tiene la distribución de un estadístico (por ejemplo, la media muestral) para poder calcular probabilidades y decidir si un resultado es "raro" o no. El **Teorema Central del Límite** es lo que garantiza esa forma: dice que, sin importar cómo se distribuya la población original, la distribución de las medias muestrales se aproxima a una normal a medida que crece el tamaño de la muestra (n).  
Eso es lo que habilita todo el mecanismo del test de hipótesis:  
1. Se plantea una **hipótesis nula (H₀)** (ej: "las dos semillas rinden igual").  
2. Gracias al TCL, se sabe que la media muestral sigue (aproximadamente) una distribución normal, con lo cual se puede calcular su desvío estándar (error estándar) y ubicar el resultado observado dentro de esa curva.  
3. Se calcula qué tan probable es obtener la diferencia observada (o una más extrema) **si H₀ fuera cierta** — esto es el  **p-valor**.  
4. Si esa probabilidad es muy baja (por debajo de un umbral, típicamente 0.05), se **rechaza H₀**: la diferencia es estadísticamente significativa y no se explica solo por azar muestral.  
***Idea clave:*** * en el ejemplo de las semillas no alcanza con co* *mparar dos medias "a ojo". El TCL permite construir la distribución esperada de esas medias bajo el supuesto de que no hay diferencia real, y sobre esa distribución normal se aplica el test para decidir si la diferencia observada es lo bastante grande como* * para no ser producto del azar. Sin el TCL no habría base teórica para saber qué distribución usar ni cómo calcular esas probabilidades — es el fundamento estadístico detrás de la mayoría de los test de hipótesis paramétricos (test t, test z, ANOVA, etc.).*  
*Notas de la clase*  
- Materia de último cuatrimestre, con manejo flexible pero exigiendo marcar asistencia en cada clase.  
- 16 clases en total, sin feriados; 4 dedicadas a parciales/instancias evaluativas.  
- Primer parcial: teórico, probablemente presencial (se confirma más cerca de la fecha); si es virtual, con cámara prendida y compartiendo pantalla.  
- Segundo parcial: trabajo práctico final, similar a cuatrimestres anteriores, se entrega en la segunda mitad de la cursada.  
- El profesor no graba las clases; sube el contenido de las diapositivas al campus.  
**Clase 2 — 28/8 · Numpy**  
*Pendiente — se actualiza cuando se dicte la clase.*  
Clase 3 — 4/9 · Pandas  
*Pendiente.*  
Clase 4 — 11/9 · Data cleaning  
*Pendiente.*  
Clase 5 — 18/9 · Análisis exploratorio de datos y estadística descriptiva  
*Pendiente.*  
Clase 6 — 25/9 · Visualización de datos  
*Pendiente.*  
🟣 2/10 · Primer parcial teórico  
**Fecha evaluatoria.** Primer parcial: teórico y virtual.  
**Clase 7 — 9/10 · Análisis de datos con R**  
*Pendiente.*  
🟣 16/10 · Recuperatorio primer parcial  
**Fecha evaluatoria.**  
**Clase 8 — 23/10 · Integración de fuentes / SQL con pandas / Cassandra**  
*Pendiente.*  
**Clase 9 — 30/10 · Conceptos básicos del modelado de datos**  
*Pendiente.*  
**Clase 10 — 6/11 · Modelos de clasificación**  
*Pendiente.*  
**Clase 11 — 13/11 · Modelos de regresión**  
*Pendiente.*  
**Clase 12 — 20/11 · Modelos de clustering**  
*Pendiente.*  
🟣 27/11 · Defensa TP final  
**Fecha evaluatoria.** Segundo parcial: defensa del trabajo práctico final (informe con bases de la Encuesta Permanente de Hogares — INDEC).  
🟣 4/12 · Recuperatorio TP final  
**Fecha evaluatoria.**  
🟢 11/12 · Instancia de finales y última instancia de recuperatorio  
**Fecha evaluatoria.** Examen integrador para quienes no llegaron a regularizar (nota máxima 4), y última instancia de finales.  
     
   
Bibliografía  
**Obligatoria**  
- Chan, D., Badano, C., Rey, A. (2019). *Análisis inteligente de datos con lenguaje R* (pp. 1-73). edUTecNe. — se ven los dos primeros capítulos (introducción a la minería de datos e introducción al análisis de datos); es la referencia conceptual "de cabecera" de la materia, con ejemplos en R.  
- McKinney, W. (2023). *Python para análisis de datos*. Ediciones Anaya Multimedia. (Trabajo original 2022) — el autor es el creador de Pandas; se usa más como referencia práctica de Python que conceptual.  
**Optativa**  
- Mitchell, T. (1997). *Machine Learning*. McGraw Hill.  
- Szretter Noste, M. E. (2017). *Apunte de regresión lineal*. FCEyN UBA.  
- Zenaida Hernández, M. (2012). *Métodos de análisis de datos* (apuntes). Universidad de La Rioja.  
Herramientas  
Python · R · SQL · Cassandra · Pandas · Google Colab  
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANUlEQVR4nO3OMQ2AABAAsSNhwgJGkPcrHpnRgQU2QtIq6DIze3UGAMBf3Gu1VcfXEwAAXrseaJkELjbMzy0AAAAASUVORK5CYII=)  
🗂️ Estructura del repositorio  
Introducción al Análisis de Datos  
 ├── Material  
 │   ├── 0 - Funcionamiento.pdf  
 │   └── 1 - Clase 1.pdf  
 └── README.md  
   
Cada nueva clase se agrega a Material/ numerada en orden (2 - Clase 2.pdf, 3 - Clase 3.pdf, ...), y el desarrollo completo se pega dentro del botón desplegable correspondiente en el [🗓️ Cronograma de clases, reemplazando el *"Pendiente"*. Cuando eso pasa, sumá también sus subtemas al Índice de arriba, como está hecho con la Clase 1.](#anchor-4 "#anchor-4")  
