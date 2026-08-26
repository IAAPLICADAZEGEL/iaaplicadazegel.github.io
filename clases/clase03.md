---
titulo: De los datos al procedimiento
modulo: Clase 03
resumen: Sobre el trabajo con datos.
---
# Sesión 03 · De los datos al procedimiento

**Marco teórico**

Trabajar con datos exige convertir información registrada en evidencia útil para responder preguntas. Para hacerlo, definimos qué queremos conocer, comprendemos la estructura de los datos, elegimos métricas apropiadas, interpretamos los resultados y conservamos un procedimiento capaz de repetirse.

La inteligencia artificial reduce la fricción técnica de muchas de estas operaciones. Nuestro criterio sigue guiando el proceso: formulamos la pregunta, delimitamos la evidencia, revisamos los cálculos y decidimos qué significa el resultado.

Nuestro recorrido puede resumirse así:

```text
PREGUNTA → DATOS → PREPARACIÓN → ANÁLISIS → INTERPRETACIÓN → COMUNICACIÓN → PROCEDIMIENTO
```

---

# I · Construimos el análisis

## Principio 01 — Comenzamos por una pregunta analítica

Un conjunto de datos admite muchas lecturas. Nosotros establecemos cuál resulta relevante al convertir una necesidad en una pregunta que pueda resolverse mediante evidencia.

Una buena pregunta define cuatro elementos:

| Elemento               | Qué establecemos                                             |
| ---------------------- | ------------------------------------------------------------ |
| **Objeto**             | Qué fenómeno queremos comprender                             |
| **Unidad de análisis** | Qué representa cada observación                              |
| **Comparación**        | Entre qué grupos, categorías o periodos buscamos diferencias |
| **Resultado**          | Qué medida permitirá responder la pregunta                   |

A partir de esta definición seleccionamos datos y métricas.

También delimitamos el alcance de nuestras conclusiones:

| Alcance          | Pregunta                                                             |
| ---------------- | -------------------------------------------------------------------- |
| **Descriptivo**  | ¿Qué ocurrió?                                                        |
| **Diagnóstico**  | ¿Qué factores ayudan a explicar lo ocurrido?                         |
| **Predictivo**   | ¿Qué comportamiento podemos estimar hacia adelante?                  |
| **Prescriptivo** | ¿Qué acción ofrece mejores resultados bajo determinadas condiciones? |

Cada nivel exige evidencia y métodos adicionales. Esta distinción nos permite expresar conclusiones con precisión.

---

## Principio 02 — Comprendemos la estructura antes de resumir

Antes de calcular, inspeccionamos qué representa cada fila, qué significa cada columna y qué nivel de detalle conserva el conjunto.

La **granularidad** resulta especialmente importante. Una fila puede representar una transacción, una persona, un producto, un día o un agregado mensual. Cambiar esa unidad cambia también el significado de nuestras métricas.

Revisamos seis dimensiones básicas:

| Dimensión        | Qué revisamos                                            |
| ---------------- | -------------------------------------------------------- |
| **Cobertura**    | Cantidad de registros y periodo representado             |
| **Granularidad** | Unidad representada por cada fila                        |
| **Tipo**         | Variables numéricas, categóricas, temporales y textuales |
| **Consistencia** | Categorías, unidades y formatos uniformes                |
| **Completitud**  | Presencia de valores necesarios para el análisis         |
| **Unicidad**     | Correspondencia entre cada registro y su unidad real     |

Con esta inspección establecemos qué preguntas pueden responder los datos disponibles.

---

## Principio 03 — Elegimos métricas según la pregunta

Cada métrica ilumina una propiedad diferente del conjunto.

| Operación            | Qué observamos                                           |
| -------------------- | -------------------------------------------------------- |
| **Conteo**           | Magnitud                                                 |
| **Total**            | Acumulación                                              |
| **Promedio**         | Valor medio                                              |
| **Mediana**          | Valor central resistente a extremos                      |
| **Proporción**       | Participación respecto de un total                       |
| **Tasa**             | Frecuencia relativa a una población, tiempo o exposición |
| **Distribución**     | Forma en que se reparten los valores                     |
| **Evolución**        | Cambio a través del tiempo                               |
| **Dispersión**       | Variabilidad entre observaciones                         |
| **Valores extremos** | Registros alejados del comportamiento habitual           |

Para interpretar una métrica definimos siempre su **unidad, periodo y denominador**.

Por ejemplo, una cantidad absoluta muestra volumen. Una proporción incorpora el tamaño del conjunto. Una tasa incorpora además una base de exposición.

Esta diferencia resulta esencial cuando comparamos grupos de tamaños distintos.

También examinamos las métricas en conjunto. La distancia entre promedio y mediana, la dispersión y la forma de la distribución pueden revelar información que una cifra aislada deja fuera de nuestra vista.

---

## Principio 04 — Separamos evidencia, interpretación y explicación

Durante el análisis distinguimos tres capas:

| Capa               | Qué expresamos                                             |
| ------------------ | ---------------------------------------------------------- |
| **Observación**    | Lo que podemos calcular directamente con los datos         |
| **Interpretación** | El patrón que identificamos a partir de esas observaciones |
| **Explicación**    | Los factores que proponemos para comprender el patrón      |

Un aumento registrado pertenece a la observación.

Una tendencia creciente pertenece a la interpretación.

Las razones que originaron esa tendencia pertenecen a la explicación y requieren variables, contexto o evidencia complementaria.

Esta separación fortalece nuestras conclusiones y facilita que otras personas comprendan hasta dónde llega la evidencia disponible.

---

# II · Trabajamos con inteligencia artificial

## Principio 05 — Utilizamos la IA como interfaz y conservamos la verificación

La IA nos permite expresar operaciones mediante lenguaje natural y trasladar parte del trabajo técnico hacia una interfaz conversacional.

Podemos pedirle que:

* inspeccione estructuras;
* proponga preguntas;
* calcule métricas;
* transforme datos;
* genere código;
* construya gráficos;
* explique resultados;
* documente procedimientos.

El cambio principal ocurre en nuestra forma de interactuar con los datos.

Pasamos de concentrarnos únicamente en **cómo ejecutar una operación** a concentrarnos también en **qué necesitamos conocer y cómo comprobaremos el resultado**.

Para resultados cuantitativos buscamos trazabilidad:

| Nivel             | Evidencia disponible                                    |
| ----------------- | ------------------------------------------------------- |
| **Resultado**     | Cifra, tabla o gráfico final                            |
| **Procedimiento** | Operaciones utilizadas para obtenerlo                   |
| **Ejecución**     | Código, fórmulas o transformaciones realmente aplicadas |
| **Validación**    | Comprobación mediante controles, recálculo o contraste  |

Cuanto mayor sea el impacto del resultado, mayor valor tendrá esta trazabilidad.

---

## Principio 06 — Evaluamos herramientas mediante el flujo completo

Comparamos herramientas haciendo que resuelvan una tarea equivalente con los mismos datos y criterios.

Evaluamos principalmente:

| Criterio              | Qué observamos                                             |
| --------------------- | ---------------------------------------------------------- |
| **Exactitud**         | Correspondencia entre cálculo y datos                      |
| **Comprensión**       | Lectura adecuada de tipos, fechas, categorías y estructura |
| **Trazabilidad**      | Visibilidad del procedimiento utilizado                    |
| **Capacidad técnica** | Archivos, código, gráficos y transformaciones disponibles  |
| **Integración**       | Facilidad para conectar, exportar y reutilizar resultados  |
| **Eficiencia**        | Pasos y esfuerzo requeridos                                |
| **Límites**           | Tamaño, contexto, mensajes, ejecución y almacenamiento     |
| **Costo**             | Valor obtenido respecto del gasto                          |

De esta manera sustituimos la comparación genérica de herramientas por una evaluación vinculada al trabajo real.

Para nosotros, una herramienta adquiere valor cuando mejora el flujo completo.

---

# III · Convertimos el análisis en un producto

## Principio 07 — Separamos datos, procedimiento y representación cuando el trabajo crece

Un análisis pequeño puede reunir todos sus componentes en un único archivo. A medida que aumentan el volumen, la frecuencia de actualización o el número de usuarios, nos conviene separar responsabilidades.

Podemos reconocer tres configuraciones:

| Configuración  | Estructura                    | Uso apropiado                                 |
| -------------- | ----------------------------- | --------------------------------------------- |
| **Incrustada** | Datos + representación        | Conjuntos pequeños y estables                 |
| **Separada**   | Archivo de datos ↔ aplicación | Datos reemplazados periódicamente             |
| **Conectada**  | Fuente → aplicación           | Datos actualizados desde un origen compartido |

En las configuraciones separadas y conectadas utilizamos el **esquema** como contrato.

Definimos:

* nombres de columnas;
* tipos de datos;
* unidades;
* formatos de fecha;
* identificadores;
* categorías;
* reglas de actualización.

Mientras conservemos ese contrato, podemos sustituir o ampliar los registros manteniendo estable el procedimiento.

Esta separación aporta tres ventajas principales:

**Escala.** Trabajamos con estructuras capaces de recibir conjuntos mayores.

**Vigencia.** Actualizamos la información desde su fuente.

**Mantenimiento.** Modificamos datos, lógica y presentación como componentes diferenciados.

---

## Principio 08 — Comunicamos resultados para una audiencia concreta

Un análisis adquiere valor cuando otra persona puede comprenderlo y utilizarlo.

Por ello organizamos la comunicación alrededor de la pregunta original.

En informes, dashboards y aplicaciones procuramos presentar:

* indicador;
* significado;
* unidad;
* periodo;
* comparación relevante;
* fuente;
* fecha de actualización;
* alcance;
* responsable del procedimiento.

Seleccionamos la representación según la relación que queremos mostrar:

| Relación                           | Representación habitual        |
| ---------------------------------- | ------------------------------ |
| Comparación entre categorías       | Barras                         |
| Evolución temporal                 | Líneas                         |
| Distribución                       | Histograma o diagrama de caja  |
| Relación entre variables numéricas | Dispersión                     |
| Valor exacto                       | Tabla o indicador              |
| Composición sencilla               | Barras apiladas o proporciones |

El gráfico cumple una función analítica: dirige nuestra atención hacia una relación específica.

Cuando publicamos el resultado ampliamos también su ciclo de vida. Además de construirlo, asumimos actualización, acceso, mantenimiento y documentación.

---

# IV · Convertimos el trabajo en un procedimiento

## Principio 09 — Conservamos el procedimiento cuando el análisis debe repetirse

Una conversación puede producir un resultado útil. El código permite además conservar las operaciones que construyeron ese resultado.

Cuando guardamos un procedimiento podemos:

* ejecutarlo con nuevos datos;
* inspeccionar cada transformación;
* modificar una operación específica;
* versionar sus cambios;
* revisar errores;
* compartir el método;
* automatizar tareas recurrentes.

Para lograr reproducibilidad conservamos juntos los elementos esenciales:

```text
DATOS + CÓDIGO + PARÁMETROS + ENTORNO → RESULTADO REPRODUCIBLE
```

Los notebooks de Jupyter y Google Colab resultan especialmente útiles porque reúnen código, resultados, gráficos y documentación dentro de un mismo artefacto.

La IA puede participar en este nivel generando código, explicándolo, corrigiéndolo y adaptándolo. Nosotros mantenemos la ejecución como mecanismo de comprobación.

---

# V · Elegimos el nivel adecuado de solución

Cada problema merece un nivel de formalización acorde con su frecuencia, audiencia, escala y riesgo.

| Situación                            | Producto apropiado                            |
| ------------------------------------ | --------------------------------------------- |
| **Exploración rápida**               | Conversación + resultados                     |
| **Análisis puntual**                 | Informe o notebook                            |
| **Análisis recurrente**              | Notebook o script reutilizable                |
| **Información compartida**           | Dashboard o aplicación                        |
| **Datos actualizados continuamente** | Aplicación conectada a una fuente             |
| **Proceso crítico**                  | Código versionado + controles + documentación |

Nuestro objetivo consiste en construir la solución suficiente para el trabajo que queremos realizar.

La sofisticación aporta valor cuando responde a una necesidad concreta.

---

# Síntesis

A lo largo de este recorrido desarrollamos una forma de trabajar con datos basada en nueve decisiones:

1. **Formulamos una pregunta analítica.**
2. **Comprendemos la unidad y estructura de los datos.**
3. **Elegimos métricas coherentes con la pregunta.**
4. **Distinguimos observación, interpretación y explicación.**
5. **Usamos la IA conservando mecanismos de verificación.**
6. **Evaluamos herramientas mediante trabajo comparable.**
7. **Diseñamos una arquitectura acorde con escala y actualización.**
8. **Comunicamos resultados para una audiencia concreta.**
9. **Conservamos procedimientos cuando buscamos repetibilidad.**

Estas decisiones forman una progresión profesional:

```text
PREGUNTAR → COMPRENDER → MEDIR → INTERPRETAR → VERIFICAR → COMUNICAR → REPRODUCIR
```

---

# Continuidad formativa

La IA nos permite recorrer este proceso con mayor velocidad. Para ampliar nuestra autonomía y criterio, complementamos su uso con formación específica en análisis de datos.

Una ruta sólida combina:

**hojas de cálculo → estadística → SQL → visualización → Python → proyectos reales**

De esta manera avanzamos desde el análisis asistido hacia la capacidad de comprender, construir, revisar y mantener nuestros propios procedimientos.

## Recursos recomendados

| Prioridad | Recurso                                                   | Tipo                    | Enfoque                                                               | Nivel              | Acceso                                                                                                                                    |
| --------- | --------------------------------------------------------- | ----------------------- | --------------------------------------------------------------------- | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------- |
| 01        | **Google Data Analytics Professional Certificate**        | Curso · Coursera        | Fundamentos, hojas de cálculo, SQL, visualización y proceso analítico | Inicial            | [Coursera](https://www.coursera.org/professional-certificates/analisis-de-datos-de-google/?utm_source=chatgpt.com)                        |
| 02        | **Tidy Data — Hadley Wickham**                            | Artículo                | Estructura y organización de datos                                    | Fundamental        | [Journal of Statistical Software](https://www.jstatsoft.org/v59/i10/?utm_source=chatgpt.com)                                              |
| 03        | **Practical Statistics for Data Scientists, 2nd Edition** | Libro                   | Estadística aplicada al análisis de datos                             | Inicial–intermedio | [O'Reilly](https://www.oreilly.com/library/view/practical-statistics-for/9781492072935/?utm_source=chatgpt.com)                           |
| 04        | **IBM Data Analyst Professional Certificate**             | Curso · Coursera        | Excel, SQL, Python, pandas, NumPy y proyectos                         | Inicial–intermedio | [Coursera](https://www.coursera.org/professional-certificates/ibm-data-analyst?utm_source=chatgpt.com)                                    |
| 05        | **Python for Data Analysis, 3E — Wes McKinney**           | Libro · edición abierta | Python, pandas, limpieza, transformación y análisis                   | Intermedio         | [Edición abierta](https://wesmckinney.com/book/?utm_source=chatgpt.com)                                                                   |
| 06        | **Storytelling with Data — 10th Anniversary Edition**     | Libro · 2026            | Visualización y comunicación de resultados                            | Inicial–intermedio | [Wiley](https://www.wiley-vch.de/en?isbn=9781394388097&option=com_eshop&title=Storytelling+with+Data&view=product&utm_source=chatgpt.com) |
| 07        | **Kaggle Learn**                                          | Plataforma práctica     | Python, pandas, SQL, visualización y ejercicios                       | Inicial–intermedio | [Kaggle Learn](https://www.kaggle.com/learn?utm_source=chatgpt.com)                                                                       |
| 08        | **R for Data Science, 2e**                                | Libro · edición abierta | Flujo completo de análisis y datos ordenados                          | Complementario     | [R for Data Science](https://r4ds.hadley.nz/?utm_source=chatgpt.com)                                                                      |

---

## Idea central

> Cuando la inteligencia artificial reduce la dificultad técnica, nuestro valor se desplaza hacia el criterio: saber qué preguntar, comprender qué representan los datos, elegir cómo medirlos, verificar lo obtenido y convertir el análisis en un procedimiento confiable.

Aprendemos a trabajar **con IA y con datos** como competencias complementarias. La primera acelera nuestra ejecución; la segunda fortalece nuestra capacidad para decidir qué merece ser ejecutado y cómo evaluar el resultado.
