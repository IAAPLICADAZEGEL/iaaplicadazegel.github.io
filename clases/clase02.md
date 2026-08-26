---
titulo: Clase 02
modulo: Clase 02
resumen: Casos aplicados
---

# Sesión 02 · Del documento al dato

**Marco teórico**

La sesión anterior trabajó la conversación. Esta trabaja el material: documentos que llegan hechos, archivos que guardan registros y las primeras representaciones construidas sobre ellos.

*IA Generativa Aplicada · ZEGEL · Ing. César Uribe*

---

## Índice

| Movimiento | Tema | Principios |
|:--|:--|:--|
| I | El documento como materia prima | 18 – 22 |
| II | Del documento al dato | 23 – 26 |
| III | De la lectura a la representación | 27 – 28 |
| IV | Alcances hacia la Sesión 03 | Cuatro anticipos |

**Tesis de la sesión:** el trabajo cambia de naturaleza según lo que tengamos delante. Un texto pide fidelidad, un conjunto de registros pide preguntas y una representación pide decisiones de arquitectura.

**Continuidad con la Sesión 01.** Los diecisiete principios anteriores siguen vigentes y esta sesión los pone a prueba sobre material real: la petición se construye igual, el trabajo empieza igual cuando llega la respuesta y la verificación crece igual con el riesgo. La numeración continúa desde ahí.

---

# I · El documento como materia prima

## Principio 18 — Transformar información existente es la operación central de este bloque

Los cuatro primeros casos comparten una misma forma: entregamos un documento que ya existe y solicitamos otra versión de ese mismo contenido. Cambia el idioma, cambia el formato, cambia el registro, cambia el orden. El contenido permanece.

Esto separa dos familias de tareas:

| Familia | Origen del contenido | Riesgo dominante |
|:--|:--|:--|
| **Transformación** | El documento entregado | Que aparezca contenido ajeno al original |
| **Generación** | El modelo y el contexto | Que el resultado carezca de respaldo comprobable |

En la transformación, el documento manda. Cada afirmación del resultado debería poder rastrearse hasta el origen.

## Principio 19 — La fidelidad se declara de manera explícita

Una traducción gramaticalmente perfecta puede resultar inservible para un área técnica cuando altera una cifra, adapta una unidad o suaviza una advertencia. Por eso la petición declara qué elementos permanecen idénticos:

- Cifras y valores numéricos
- Unidades de medida y temperaturas
- Terminología técnica del dominio
- Normas y referencias citadas
- Advertencias de seguridad
- Estructura y orden del contenido

**Sobre el campo «Advertencia».** La estructura formal que la Sesión 01 presentó recibe aquí un nombre operativo, **ROSAC**: Rol, Objetivo, Salida, Advertencia y Contexto. La Advertencia es el campo donde declaramos aquello que permanece intacto, y su valor crece exactamente con el costo de que algo cambie.

## Principio 20 — Estructurar consiste en decidir qué constituye una fila y qué constituye una columna

Convertir una ficha técnica en tabla parece una tarea de formato, y en realidad es una tarea de criterio. Antes de la conversión definimos la unidad de análisis:

```
DOCUMENTO → UNIDAD DE ANÁLISIS → COLUMNAS → TABLA
```

Una característica por fila. Columnas que respondan a la comparación que vendrá después: característica, especificación, valor, unidad, norma de referencia. La tabla resulta útil en la medida en que anticipa el uso —comparar cotizaciones, contrastar proveedores, auditar cumplimiento.

**Ante la ambigüedad.** Un documento real llega con datos incompletos o expresados de varias maneras. La conducta que conviene declarar es la señalización: marcar la celda como pendiente de confirmación y conservar el texto original de origen. Así el vacío permanece visible y la revisión humana sabe dónde mirar.

## Principio 21 — Depurar exige un criterio de pertinencia declarado de antemano

Una transcripción de cuatro horas contiene explicación académica, ejemplos, intervenciones, indicaciones administrativas, saludos, repeticiones y conversación espontánea. Convertirla en informe consiste en **elegir**, y la elección obedece al destino del documento.

| Destino del informe | Criterio de pertinencia |
|:--|:--|
| Registro académico | Temas, conceptos, actividades, ejemplos, herramientas, conclusiones |
| Acta administrativa | Acuerdos, responsables, fechas, compromisos |
| Material de estudio | Explicaciones, definiciones, ejercicios resueltos |

El mismo material produce documentos distintos según el criterio. Declarar el destino en el contexto de la petición resuelve la mayor parte de las decisiones que vendrán después.

## Principio 22 — Mejorar la redacción conserva los hechos

El caso del currículum ilumina la frontera con precisión. Reformular «hacía reportes» como «elaboración de reportes periódicos para el área administrativa» mejora la presentación de un hecho existente. Añadir «reduje en 30 % el tiempo de cierre» inventa un hecho.

| Operación legítima | Operación que fabrica |
|:--|:--|
| Verbos de acción sobre funciones reales | Métricas inventadas al momento |
| Vocabulario profesional actual | Certificaciones ausentes del origen |
| Orden, jerarquía y síntesis | Responsabilidades ampliadas |
| Perfil que sintetiza lo declarado | Logros atribuidos |

La prueba es directa: cada afirmación del documento final debe poder señalarse en el borrador original. Esa correspondencia funciona como criterio de veracidad para cualquier documento personal, comercial o académico.

---

# II · Del documento al dato

## Principio 23 — Un documento se lee; un conjunto de datos se interroga

Aquí cambia la naturaleza del material. Un Excel con cincuenta registros contiene la respuesta a decenas de preguntas distintas, y todas conviven en la misma tabla hasta que alguien formula una.

| Término | Definición |
|:--|:--|
| **Registro** | Observación individual del conjunto |
| **Variable** | Característica registrada para cada observación |
| **Métrica** | Medida calculada a partir de los datos |
| **Tendencia central** | Valor que representa el centro de una distribución |
| **Distribución** | Forma en que los valores se reparten |
| **Evolución temporal** | Comportamiento de una variable a través del tiempo |
| **Valor atípico** | Observación considerablemente diferente de las demás |
| **Agregación** | Combinación de registros mediante suma, promedio o conteo |

Este vocabulario mínimo permite pedir con precisión. Quien dispone de las palabras «mediana», «distribución» y «atípico» formula preguntas que la hoja de cálculo puede responder.

## Principio 24 — Cada pregunta observa los mismos datos desde una perspectiva distinta

El flujo del análisis descriptivo mantiene siempre la misma forma:

```
DATOS → PREGUNTA → MÉTRICA → COMPARACIÓN → INTERPRETACIÓN
```

Y el recorrido completo se despliega en seis operaciones:

| # | Operación | Pregunta que responde | Métrica típica |
|:--|:--|:--|:--|
| 01 | **Contar** | ¿Cuántos registros tenemos? | Conteo, cobertura temporal |
| 02 | **Resumir** | ¿Cuál es la magnitud acumulada y su centro? | Total, promedio, mediana |
| 03 | **Distribuir** | ¿Cómo se reparte entre categorías? | Participación porcentual |
| 04 | **Comparar** | ¿Qué diferencias existen entre grupos? | Contraste entre departamentos, regiones, canales |
| 05 | **Evolucionar** | ¿Cómo se comporta a través del tiempo? | Serie temporal, variación mensual |
| 06 | **Detectar** | ¿Qué registros merecen revisión particular? | Valores atípicos, extremos |

**Promedio y mediana juntos.** Ambos describen el centro y responden a preguntas distintas. Cuando la distancia entre ellos crece, esa distancia informa sobre la presencia de valores extremos, y la operación 06 encuentra ahí su punto de partida.

## Principio 25 — El análisis descriptivo responde «¿qué ocurrió?»

Ese es su alcance completo y ahí reside su valor. Caracteriza el pasado registrado: magnitudes, repartos, evoluciones y singularidades.

Las preguntas sobre causas, predicciones y decisiones pertenecen a otros tipos de análisis, con otros métodos y otras exigencias de evidencia. La Sesión 01 lo formuló para las respuestas generadas; aquí vale para los números: **la descripción se comprueba en los datos, y la explicación reclama evidencia adicional.**

## Principio 26 — Describir, interpretar y explicar son tres operaciones sucesivas

```
DATO OBSERVADO → INTERPRETACIÓN → EXPLICACIÓN CAUSAL
```

| Nivel | Ejemplo | Respaldo que exige |
|:--|:--|:--|
| **Dato observado** | Operaciones registra el mayor gasto acumulado | El propio conjunto de datos |
| **Interpretación** | El gasto se concentra en pocas categorías | Los datos, más un criterio de lectura |
| **Explicación causal** | Operaciones administra peor sus recursos | Contexto externo: tamaño del equipo, presupuesto asignado, naturaleza de las funciones, política de gastos |

Un informe generado por IA suele entregar los tres niveles con la misma fluidez y en el mismo párrafo. Separarlos es trabajo nuestro, y coincide exactamente con el Principio 08: el tono viste por igual al dato comprobable y a la conjetura.

**Regla operativa para cualquier informe descriptivo.** Revisamos cada conclusión y le asignamos su nivel. Las del primer nivel se sostienen solas; las del tercero llegan acompañadas de la evidencia que las respalda o permanecen enunciadas como hipótesis.

---

# III · De la lectura a la representación

## Principio 27 — Un dashboard suma representación e interacción a los mismos datos

| Artefacto | Contiene |
|:--|:--|
| **Excel** | Datos |
| **Informe** | Datos + lectura fija |
| **Dashboard** | Datos + representación + interacción |

La conversación resuelve preguntas de una en una. La representación visual permite explorar: filtrar, ordenar, acercarse a un periodo, aislar una categoría. Cada gráfico responde a una familia de preguntas, y elegirlo consiste en decidir qué queremos observar.

| Pregunta | Representación apropiada |
|:--|:--|
| ¿Cómo evoluciona? | Serie temporal |
| ¿Cómo se reparte? | Distribución por categorías |
| ¿Cuánto en total? | Indicador único |
| ¿Qué destaca? | Ranking de principales registros |
| ¿Qué compone el conjunto? | Detalle en tabla con filtros |

**El archivo monolítico.** Un documento HTML puede concentrar estructura, estilos, comportamiento y datos, y funcionar como pieza autónoma en cualquier navegador. Para conjuntos pequeños y estables, esa autonomía es su gran virtud: un archivo, un doble clic, un resultado.

```
DATOS + APLICACIÓN = UN ARCHIVO
```

## Principio 28 — La estructura basta para construir la herramienta

El octavo caso introduce el desplazamiento conceptual más importante de la sesión. Para construir una aplicación sobre datos, conocer su **esquema** —nombres de columnas, tipos, un ejemplo de fila— resulta suficiente. El contenido completo llega después.

```
MUESTRA → ESTRUCTURA → APLICACIÓN
ARCHIVO REAL → APLICACIÓN → VISUALIZACIÓN
```

Esta separación abre tres ventajas concretas:

| Ventaja | Situación donde importa |
|:--|:--|
| **Privacidad** | Datos sensibles permanecen en nuestro entorno mientras la herramienta se construye fuera |
| **Escala** | Archivos grandes exceden el contexto disponible; el esquema ocupa unas líneas |
| **Vigencia** | Datos que cambian a diario mantienen la misma aplicación |

Aquí reaparece la ventana de contexto del Principio 14: el esquema pesa unos pocos tokens y el conjunto completo puede pesar más de lo que la conversación admite. Trabajar con la estructura es también una decisión de economía.

**Dos arquitecturas, una misma visualización:**

| Arquitectura | Forma | Cuándo conviene |
|:--|:--|:--|
| Datos incrustados | `DATOS + VISUALIZACIÓN = HTML` | Conjunto pequeño, estable, portátil |
| Datos separados | `DATOS ↔ VISUALIZACIÓN` | Conjunto grande, sensible o cambiante |

---

# IV · Alcances hacia la Sesión 03

Los cuatro temas siguientes quedan enunciados aquí y se desarrollan con detalle en la próxima sesión. Conviene reconocerlos desde ahora, porque cada uno resuelve una limitación que ya apareció durante estos casos.

## Alcance 01 — Analizar al analista

Los servicios de IA disponibles procesan un mismo archivo con capacidades distintas: comprensión de columnas, calidad de los cálculos, gráficos, explicación del procedimiento, uso de código, límites de tamaño, opciones de exportación.

La comparación útil ejecuta el mismo trabajo en cada herramienta con el mismo archivo y las mismas preguntas. Ahí aparece la **validación cruzada**: cuando dos plataformas coinciden en los cálculos principales, ganamos confianza; cuando difieren, ganamos una pregunta que investigar.

Y aparece la **transparencia** como criterio propio: dos herramientas pueden entregar el mismo número, y aquella que permite inspeccionar el procedimiento entrega además la posibilidad de auditarlo.

> **Pregunta que abre:** ¿qué valor adicional aporta poder revisar cómo se obtuvo un resultado correcto?

## Alcance 02 — El dato vivo

El dashboard construido con datos incrustados exige reconstrucción cada vez que el origen cambia. La siguiente arquitectura sitúa los datos en una fuente accesible —una hoja compartida, un archivo publicado— y la aplicación los consulta al abrirse.

```
Caso incrustado   →  datos dentro del HTML
Caso separado     →  archivo junto al HTML
Fuente remota     →  datos alojados fuera de la aplicación
```

La visualización permanece; la ubicación de los datos cambia. Con esa autonomía llegan también dependencias nuevas: disponibilidad de la fuente, permisos de acceso, políticas del navegador, formatos de intercambio.

> **Pregunta que abre:** ¿qué ventajas y qué dependencias aparecen cuando la aplicación consulta un origen externo?

## Alcance 03 — Construir y publicar son problemas distintos

Un dashboard que funciona en nuestra computadora resuelve un problema personal. Convertirlo en una dirección que otras personas consulten pertenece a otro terreno: alojamiento, despliegue, actualización, permanencia.

```
CONSTRUIR ≠ PUBLICAR
```

Cuando el resultado pasa a manos de terceros aparecen responsabilidades nuevas: mantener los datos vigentes, documentar qué representa cada indicador, señalar la fecha de actualización y responder por lo que otros decidan a partir de esa pantalla.

> **Pregunta que abre:** ¿qué obligaciones asumimos cuando una visualización deja de ser un archivo personal?

## Alcance 04 — Del resultado al procedimiento

La conversación entrega resultados. El código entrega el procedimiento que produce esos resultados.

| Camino | Forma | Lo que conserva |
|:--|:--|:--|
| Conversacional | `DATOS → IA → RESULTADO` | El resultado |
| Con código | `DATOS → CÓDIGO → RESULTADO` | El procedimiento |
| Con IA que construye código | `DATOS + OBJETIVO → IA → CÓDIGO → RESULTADO` | Ambos |

Un procedimiento guardado puede inspeccionarse, corregirse, versionarse y ejecutarse otra vez con datos compatibles. Ahí nace la **reproducibilidad**: la capacidad de repetir un análisis y obtener resultados consistentes a partir de las mismas condiciones. Para todo análisis que se repita cada mes, esa propiedad decide entre rehacer la conversación completa o ejecutar una celda.

> **Pregunta que abre:** ¿qué ganamos al conservar el procedimiento además de sus resultados?

---

# Síntesis

| Movimiento | Fórmula | Idea que sostiene |
|:--|:--|:--|
| **El documento** | Origen → transformación → destino | El documento manda: cada afirmación del resultado se rastrea hasta él. |
| **El dato** | Datos → pregunta → métrica → interpretación | La descripción se comprueba en los datos; la explicación reclama evidencia adicional. |
| **La representación** | Datos + representación + interacción | Elegir un gráfico consiste en decidir qué queremos observar. |
| **La arquitectura** | Estructura antes que contenido | El esquema basta para construir la herramienta. |

## El recorrido completo del bloque de datos

```
PREGUNTAR → ANALIZAR → COMPARAR → VISUALIZAR → SEPARAR → CONECTAR → PUBLICAR → REPRODUCIR
   ↑___________ Sesión 02 ___________↑        ↑________ Sesión 03 ________↑
```

Esta sesión llega hasta la separación entre datos y aplicación. La siguiente recorre la comparación de herramientas, las fuentes actualizables, la publicación y el código reproducible.

## Idea central

> La IA reduce la dificultad técnica de trabajar con documentos y datos. Comprender qué preguntamos, qué representan los resultados y cómo se construyó el análisis permanece como la parte esencial del trabajo.