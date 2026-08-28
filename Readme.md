# <font color="#1F6FEB">Metodología de Sistemas I</font>

Apuntes de cursada, material de clase y seguimiento del Trabajo Práctico grupal de la materia **Metodología de Sistemas I**. El objetivo del repositorio es centralizar lo que se va viendo en cada clase, dejar registro de las decisiones tomadas para el TP y servir de referencia rápida para repasar antes de las entregas.

---

## <font color="#8250DF">🧭 Índice</font>

<details>
<summary><font color="#8250DF"><strong>📅 Clase 1 — 24/08 · Presentación de la materia, el TP y primeros conceptos</strong></font></summary>

- [<font color="#1A7F37">De qué se trata la materia</font>](#clase-1-de-que-se-trata-la-materia)
- [<font color="#1A7F37">El Trabajo Práctico (TP)</font>](#clase-1-el-trabajo-practico-tp)
- [<font color="#9A6700">Ideas de proyecto (brainstorming)</font>](#clase-1-ideas-de-proyecto-brainstorming)
- [<font color="#9A6700">Candidatas propias (Grupo 5)</font>](#clase-1-candidatas-propias-grupo-5)
- [<font color="#1A7F37">Diferencia de expectativas</font>](#clase-1-diferencia-de-expectativas)
- [<font color="#1A7F37">Locación de servicio vs. Locación de obra</font>](#clase-1-locacion-de-servicio-vs-locacion-de-obra)
- [<font color="#1A7F37">Alcance (límite) de un sistema</font>](#clase-1-alcance-limite-de-un-sistema)
- [<font color="#1A7F37">Objetivos de corto, mediano y largo plazo</font>](#clase-1-objetivos-de-corto-mediano-y-largo-plazo)

</details>

<details>
<summary><font color="#8250DF"><strong>🗓️ Fechas de entrega / revisión del TP</strong></font></summary>

<details>
<summary><font color="#1A7F37">Prototipo inicial</font></summary>

**Se entrega:** conjunto de pantallas (HTML/JS) con datos estáticos que reflejen la información a procesar, resultado de aplicar Design Thinking sobre el proceso elegido.
**Fecha confirmada: 31/08.**

</details>

<details>
<summary><font color="#1A7F37">Análisis</font></summary>

**Se entrega:** listado de requerimientos funcionales y no funcionales, vinculado a las interfaces de usuario diseñadas en el prototipo.
*(Fecha de la plantilla de cátedra: 4/5 — a confirmar para esta cursada.)*

</details>

<details>
<summary><font color="#1A7F37">Diseño</font></summary>

**Se entrega:** detalle de casos de uso, modelo de clases y modelo de datos.
*(Fecha de la plantilla de cátedra: 18/5 — a confirmar para esta cursada.)*

</details>

<details>
<summary><font color="#1A7F37">Desarrollo</font></summary>

**Se entrega:** detalle de las formas de trabajo grupal y su documentación (buenas prácticas de desarrollo).
*(Fecha de la plantilla de cátedra: 1/6 — a confirmar para esta cursada.)*

</details>

<details>
<summary><font color="#1A7F37">Pruebas</font></summary>

**Se entrega:** diseño de pruebas unitarias, funcionales, de regresión y de performance.
*(Fecha de la plantilla de cátedra: 1/6 — a confirmar para esta cursada.)*

</details>

<details>
<summary><font color="#1A7F37">Implementación</font></summary>

**Se entrega:** configuración de ambientes (usuarios, recursos, seguridad y variables).
*(Fecha de la plantilla de cátedra: 22/6 — a confirmar para esta cursada.)*

</details>

**Corrección:** las entregas se revisan en el tablero de GitHub Projects. Una tarea pasa de *In Progress* a *Resol* cuando el grupo la da por terminada; si el profesor la considera bien resuelta pasa a *Done*, y si no, vuelve a *In Progress* con comentarios para corregir.

</details>

---

## <a id="clase-1"></a><font color="#8250DF">📅 Clase 1 — 24/08 · Presentación de la materia, el TP y primeros conceptos</font>

### <a id="clase-1-de-que-se-trata-la-materia"></a><font color="#1A7F37">De qué se trata la materia</font>

- La materia no es de programación: el objetivo es **diseñar** un sistema, no construirlo. Esa parte queda para las materias de programación del resto de la carrera.
- Se busca que cada estudiante pueda sumar una experiencia real al currículum: haber relevado, analizado y diseñado un sistema para un cliente concreto, aunque sea de alcance chico.
- Se trabaja con dos herramientas colaborativas:
  - **Figma** (pizarrón virtual compartido) para dinámicas de grupo, brainstorming y diagramas en clase.
  - **GitHub Projects** para la planificación y el seguimiento de tareas del TP.
- Cada clase se toma asistencia y se dedican un par de minutos a una dinámica de feedback (una especie de “retro”): qué gustó, qué no, y propuestas de mejora, para poder charlarlo durante la cursada y no recién al final del cuatrimestre.

### <a id="clase-1-el-trabajo-practico-tp"></a><font color="#1A7F37">El Trabajo Práctico (TP)</font>

**Consigna general:** diseñar un sistema informático para optimizar un proceso real de una empresa o persona, siguiendo la metodología vista en clase (no se llega a programar, sí a dejar un diseño que facilite la programación posterior).

Puntos clave para tener en cuenta a la hora de armarlo:

- **Grupos de 3 personas.** Se recomienda número impar para poder destrabar decisiones por mayoría si el grupo no se pone de acuerdo.
- **El cliente tiene que ser real**, no un caso ficticio. Debe ser alguien accesible (familiar, conocido, empleador, etc.) que pueda dedicarle tiempo real al equipo — si dedica “media hora por mes” no alcanza. La interacción con ese cliente es en sí misma valiosa: ayuda a que el propio cliente termine de entender qué necesita.
- **Documentación**: se centraliza en un Google Docs de solo lectura, donde se va agregando todo lo producido durante la cursada.
- **Gestión de tareas con GitHub Projects** (tablero tipo Kanban):
  - Columnas: *To Do* → *In Progress* → *Resol* (a revisión) → *Done*. Si una tarea entregada no está a la altura, vuelve a *In Progress* con comentarios.
  - Cada tarea (issue) debe llevar un **label con el número de grupo** — imprescindible para que después funcionen los filtros por grupo.
  - Cada tarea necesita **un único responsable asignado** (ni todos, ni nadie).
  - Se arman **vistas filtradas por grupo** para que cada equipo gestione solo lo suyo.
- **Idea de proyecto**: tiene que ser algo chico y acotado. Se insistió varias veces en no abarcar demasiado (ej.: “gestión de gimnasio” es demasiado amplio si se le suman turnos, facturación, abonos, etc. — conviene quedarse con una sola funcionalidad concreta) para poder concentrarse en aplicar bien las técnicas de la materia y no perderse en el tamaño del problema.

#### <a id="clase-1-ideas-de-proyecto-brainstorming"></a><font color="#9A6700">💡 Ideas de proyecto (brainstorming — a desarrollar)</font>

Lluvia de ideas propuesta en clase como punto de partida para elegir el proyecto de cada grupo. Son ideas abiertas, no compromisos definitivos:

- Gestión de gimnasio (rutinas personalizadas, seguimiento por alumno)
- Sistema de seguimiento de encomiendas
- Sistema de inventario / stock para una papelera
- Gestión de ventas digitales (fotografía de eventos deportivos)
- Sistema de pedidos de cafetería
- Sistema de notas para una institución secundaria
- Sistema de turnos (peluquería, consultorio médico, actividades deportivas)
- Mantenimiento de senderos de un parque nacional
- BackOffice / gestión de stock
- Venta de entradas
- E-commerce de accesorios para mascotas

#### <a id="clase-1-candidatas-propias-grupo-5"></a><font color="#9A6700">🎯 Candidatas propias (Grupo 5)</font>

De esa lluvia de ideas, las que quedaron como candidatas concretas para el proyecto del equipo:

1. **BackOffice — Gestión de stock**
2. **Sistema de venta de entradas** (estilo passline)
3. **Gestión de turnos** en peluquería / consultorio médico particular
4. **Sistema de gestión para e-commerce de accesorios de mascotas**

Info útil de la clase para arrancar el desarrollo, aplicable a estas cuatro:

- **La idea de “turnos” fue avalada explícitamente en clase**: se marcó como un clásico pero todavía muy necesario, porque “mucha gente no tiene sistema de turnos” — y se dio de ejemplo justamente una peluquería. Es un buen indicio de que el problema es real y acotado.
- **Punto de partida metodológico para cualquiera de las cuatro** (mismo camino que se usó en clase con el sistema de ventas de ejemplo):
  1. Identificar la **entrada / activador** del sistema: qué evento dispara todo (un pedido de stock que ingresa, una compra de entrada, un turno solicitado, una venta en el e-commerce).
  2. Definir la **salida esperada**: qué se considera “resuelto” (stock actualizado, entrada emitida, turno confirmado, pedido despachado).
  3. Recién ahí desglosar los **elementos internos** (los pasos/subsistemas que conectan la entrada con la salida) y armar el **happy path**.
  4. Cerrar con el **alcance/límite**: dejar explícito qué queda afuera (cobros, logística, reposición de stock, etc., según corresponda a cada idea) para evitar diferencias de expectativas con el cliente.
- **Antes de elegir una definitiva**, confirmar que haya un **cliente real y accesible** que pueda dedicarle tiempo al equipo (el requisito no negociable del TP) — vale tanto para la peluquería/consultorio como para el negocio de stock, entradas o e-commerce de mascotas.
- **Mantenerla acotada**: mismo criterio que se remarcó con “gestión de gimnasio” — elegir una sola de estas cuatro y no ir sumándole funcionalidades de las otras tres a medida que avanza el diseño.

### <a id="clase-1-diferencia-de-expectativas"></a><font color="#1A7F37">Diferencia de expectativas</font>

Uno de los ejes centrales de la clase: cuando alguien da una orden o pide algo, tiene en la cabeza un resultado esperado que **no siempre coincide** con lo que la otra persona entiende o entrega. Esa brecha es la fuente más común de conflictos entre cliente y proveedor.

- Se ilustró con ejemplos cotidianos (una tarea doméstica mal especificada, un pedido en un local de comida rápida que no coincide con la publicidad, reclamos de clientes por el resultado de un trabajo) y con una escena de película donde un jefe corrige a un empleado sin explicitar nunca el estándar que esperaba, generando desgaste innecesario.
- **Conclusión útil para el TP:** no asumir que el cliente “sabe” explicar lo que necesita ni que uno entiende automáticamente lo que pide. Hay que preguntar, confirmar y dejar explícito el alcance para minimizar diferencias de expectativas.

### <a id="clase-1-locacion-de-servicio-vs-locacion-de-obra"></a><font color="#1A7F37">Tipos de contratación: Locación de servicio vs. Locación de obra</font>

Dos formas de encuadrar la relación con un cliente, con implicancias distintas para el diseño del TP:

| | Locación de **servicio** | Locación de **obra** |
|---|---|---|
| Qué se vende | Horas / tiempo de trabajo | Un producto o resultado terminado |
| Ejemplo | Una consultora que “alquila” desarrolladores por hora | Comprometerse a entregar un sistema funcionando |
| Riesgo típico | El cliente paga aunque el alcance crezca | El proveedor absorbe el costo si el alcance crece sin renegociar (*scope creep*) |

Se representó con un ejemplo dialogado (roleplay) donde un “cliente” va agregando pedidos sobre la marcha (“una rutina personalizada”, “falta esto”, “falta el botoncito”, “ahora quiero un reporte estadístico”) y el “proveedor” termina entregando mucho más de lo pactado originalmente sin cobrar de más — ejemplo directo de scope creep en locación de obra.

- **Conclusión útil para el TP:** en locación de obra, el proveedor es quien más necesita preguntar y dejar todo por escrito antes de arrancar, porque cualquier cosa no explicitada corre por su cuenta. En locación de servicio el riesgo de sobrecosto lo asume más el cliente, así que es este quien debería preguntar más para no pagar de más.

### <a id="clase-1-alcance-limite-de-un-sistema"></a><font color="#1A7F37">Alcance (límite) de un sistema</font>

Se trabajó en vivo el diseño de un sistema de ventas de ejemplo, partiendo de un diagrama con los elementos: *recibir pedido → seleccionar forma de pago → cobrar (tarjeta) → preparar pedido → enviar mercadería*, con la pregunta “¿hay stock?” como bifurcación.

- **Elementos**: cada bloque o subsistema que compone el sistema (recibir pedido, cobrar, preparar pedido, etc.).
- **Relaciones**: las flechas/interacciones entre esos elementos.
- **Objetivo**: en el ejemplo, entregar la mercadería pedida por el cliente.
- **Happy path**: el camino donde todo sale bien y se cumple el objetivo sin interrupciones. El “camino no feliz” (no hay stock, falla el cobro, etc.) también hay que contemplarlo, pero se distingue del camino ideal.
- **Límite / alcance**: definir explícitamente qué **no** hace el sistema. En el ejemplo se discutió si estaban dentro o fuera del alcance: la logística de envío, la reposición de stock, la gestión del circuito de devoluciones (mercadería defectuosa) y el pago de sueldos del personal — se concluyó que, salvo la logística en sí, varias de esas dudas dependen del criterio de cada equipo y conviene dejarlas explícitas para evitar ambigüedad.

> **Idea clave repetida en clase:** si el límite de lo que uno se compromete a hacer no queda claro, se generan diferencias de expectativas → conflictos → pérdida de tiempo, dinero o clientes. Definir el alcance es, según se remarcó, una de las partes más importantes de la primera etapa del TP.

### <a id="clase-1-objetivos-de-corto-mediano-y-largo-plazo"></a><font color="#1A7F37">Objetivos de corto, mediano y largo plazo</font>

Se planteó un ejercicio (ejemplo cotidiano: “sacar la basura”) para mostrar cómo toda tarea puntual está enmarcada dentro de objetivos de distinto horizonte temporal, y que conviene pensarlos **de atrás para adelante** (ingeniería inversa): primero se define el objetivo de largo plazo, después el de mediano que lo sostiene, y recién ahí se entiende por qué la acción de corto plazo (la tarea concreta) importa.

- Ejemplo armado en clase: sacar la basura a horario (**corto**) → evitar multas / optimizar gastos superfluos (**mediano**) → ahorrar para un objetivo mayor, como comprar un auto (**largo**).
- **Conclusión útil para el TP:** las mismas preguntas hay que hacérselas al cliente. Si dice “quiero vender más”, conviene preguntar en qué plazo y con qué objetivo mayor se relaciona esa necesidad — eso ayuda a que las personas que ejecutan tareas puntuales entiendan el contexto y tomen mejores decisiones sobre cómo hacerlas (ej.: entender que sacar la basura fuera de horario tiene un impacto económico, no solo de higiene, cambia cómo se prioriza la tarea).

---

## <font color="#8250DF">📎 Material de referencia</font>

Presentaciones usadas como apoyo teórico durante la cursada. Se complementan con lo desarrollado en clase (ver secciones de arriba).

### <font color="#1A7F37">Teoría General de los Sistemas</font>

Resumen de los conceptos centrales del PDF, base teórica que se usó en clase para analizar el ejemplo del sistema de ventas:

- **Origen:** desarrollada por Ludwig von Bertalanffy, propone una visión holística — el sistema como un todo, no solo la suma de sus partes.
- **Concepto de sistema:** conjunto de elementos interrelacionados que trabajan para alcanzar un objetivo común; un cambio en una parte impacta en el resto.
- **Atributos:** elementos, relaciones, objetivo (teleología) y límite (frontera con el entorno).
- **Clasificaciones:** abiertos / cerrados / aislados según el intercambio con el entorno; naturales / artificiales; concretos / abstractos; estáticos / dinámicos; simples / complejos.
- **Cualidades clave:** entropía, homeostasis, sinergia, retroalimentación (positiva/negativa), equifinalidad, permeabilidad, adaptabilidad y emergencia.
- **Dato vs. información:** el dato es una representación simbólica sin significado propio hasta que se contextualiza; la información es el conjunto de datos organizados que reduce la incertidumbre y apoya decisiones.
- **Sistema de información:** conjunto de recursos (humanos, tecnológicos, materiales, financieros y metodológicos) que capturan, procesan, almacenan y distribuyen información. Sus etapas son captura → procesamiento → almacenamiento → distribución.
- **Requisitos de la información eficiente:** exactitud, relevancia, oportunidad, integridad, claridad, consistencia, accesibilidad y confiabilidad.

[![Ver PDF](https://img.shields.io/badge/📄_Ver_PDF-Teor%C3%ADa_General_de_los_Sistemas-0A66C2?style=for-the-badge)](./Material/2-TeoríaGeneraldelosSistemas.pdf)

### <font color="#1A7F37">Proyectos, Procesos, Productos, Personas (las 4 P del desarrollo de software)</font>

No se llegó a desarrollar en profundidad durante esta clase; queda como material de referencia para las próximas. Resumen del PDF:

- **Proyectos:** conjunto de actividades planificadas para lograr un objetivo en un tiempo definido. Componentes: objetivo (debe ser **SMART**: específico, medible, alcanzable, relevante y con tiempo definido), alcance, restricciones y recursos. Ciclo de vida: iniciación → planificación → ejecución → monitoreo y control → cierre.
- **Procesos:** secuencia de pasos para lograr un resultado específico. Se distingue entre procesos de gestión de proyectos (Scrum, PMBOK) y procesos técnicos (Agile, Waterfall). Su importancia radica en dar organización, gestionar riesgos y permitir adaptación al cambio.
- **Productos:** resultado tangible del trabajo (software, sistema, app). Características clave: funcionalidad, calidad y mantenibilidad. Ciclo de vida: concepción → desarrollo → implementación → mantenimiento → retirada.
- **Personas:** recurso clave del proyecto. Roles típicos: desarrolladores, analistas, testers y gestores de proyecto. Factores clave: competencia, colaboración y cultura organizacional.

[![Ver PDF](https://img.shields.io/badge/📄_Ver_PDF-Proyectos%2C_Procesos%2C_Productos%2C_Personas-0A66C2?style=for-the-badge)](./Material/1-ProyectosProcesosProductosPersonas.pdf)

### <font color="#1A7F37">Guía del Trabajo Práctico grupal (etapas y entregables)</font>

Detalle completo de cada etapa disponible en el índice, sección [🗓️ Fechas de entrega / revisión del TP](#-fechas-de-entrega--revisión-del-tp).

---

## <font color="#8250DF">🗂️ Estructura del repositorio</font>

```
Metodología de Sistemas I
├── Material
│   ├── 1-ProyectosProcesosProductosPersonas.pdf
│   └── 2-TeoríaGeneraldelosSistemas.pdf
└── Readme.md
```
