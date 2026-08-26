---
titulo: Clase 01
modulo: Clase 01
resumen: Fundamentos
---

# Sesión 01 · Trabajar con inteligencia artificial

**Marco teórico**

Construimos una petición, trabajamos la respuesta que vuelve y abrimos la caja donde ocurre el proceso.

*IA Generativa Aplicada · ZEGEL · Ing. César Uribe*

---

## Índice

| Movimiento | Tema | Principios |
|:--|:--|:--|
| I | La petición | 01 – 04 |
| II | El trabajo | 05 – 07 |
| III | La verificación | 08 – 11 |
| IV | La caja | 12 – 16 |
| V | El mapa | 17 |

**Tesis de la sesión:** cada concepto aparece en el momento exacto en que un problema real lo vuelve necesario.

---

# I · La petición

## Principio 01 — Toda tarea empieza en un problema concreto

Elegimos primero el problema y después la herramienta. Quien empieza por la herramienta termina aprendiendo cosas porque existen; quien empieza por el problema aprende cosas porque las necesita.

«Usarla en mi trabajo» describe una intención. Una tarea es algo que hoy nos cuesta resolver: entender un concepto, comparar dos informes, redactar un texto cuyo comienzo se nos resiste.

## Principio 02 — Resultado y contexto sostienen cualquier petición

| Orden | Componente | Pregunta que responde |
|:--|:--|:--|
| Primero | **Resultado** | ¿Qué queremos obtener? |
| Segundo | **Contexto** | ¿Qué necesita saber el sistema para ayudarnos a conseguirlo? |

Empezamos como empezaríamos con una persona: decimos qué necesitamos.

El contexto crece con el problema. Una operación aritmética trivial se resuelve con la operación; un concepto denso mejora cuando declaramos desde dónde preguntamos. La pregunta operativa es simple: **¿qué sabemos de nosotros que el sistema todavía ignora?**

### Construcción por capas

Una petición se construye por capas. La instrucción central permanece idéntica en las cuatro; cada capa retira ambigüedad.

| Capa | Aporte |
|:--|:--|
| 01 · Acción + objeto | La instrucción central |
| 02 · Contexto | Desde dónde preguntamos |
| 03 · Resultado | Para qué lo necesitamos |
| 04 · Forma | Cómo debe presentarse |

La extensión es una consecuencia; el criterio es la claridad. Una petición breve resuelve mucho, y una extensa puede naufragar.

## Tres formas de pedir prácticamente lo mismo

| Forma | En qué consiste | Cuándo conviene |
|:--|:--|:--|
| **01 · Sentido común** | Una acción, un objeto y el contexto imprescindible. | Se escribe en menos de un minuto y muchas veces basta. |
| **02 · Características apiladas** | El mismo problema con las condiciones separadas en lista: nivel de conocimiento, actores, ejemplo, orden de la explicación. | Cuando siete condiciones dentro de un párrafo denso cuestan más de leer. |
| **03 · Estructura formal** | Rol, objetivo, contexto, formato de salida y advertencias. | Cuando el problema amerita organizar las instrucciones como un pequeño documento de trabajo. |

Las tres compiten en igualdad. Elegimos según el resultado que necesitamos, el tiempo disponible y el costo de corregir una respuesta mala.

## Principio 03 — La estructura organiza; el criterio decide

Las tres formas son prompts por igual. La apariencia de prompt pertenece a la estética; el funcionamiento se comprueba al enviarlo.

**Sobre el rol:** orienta cuando la perspectiva importa, y su efecto termina ahí. Decir «actúa como el mejor administrador del mundo» produce un encuadre, y el resultado sigue dependiendo del problema. Cada elemento que añadimos merece una razón propia.

## Principio 04 — Cada capa retira ambigüedad

Es el mismo cambio que separa a quien construye una hoja de cálculo gigantesca de quien primero comprueba si la fórmula básica funciona. Cuando comprendemos qué necesitamos, tenemos algo con qué trabajar.

> Mientras el problema permanezca confuso, una plantilla perfecta nos ayudará a expresar esa confusión con gran precisión.

**Rendimientos decrecientes.** Siempre queda una condición más que añadir. Llega un punto en que refinar la petición cuesta más que probarla, y ahí conviene probar.

---

# II · El trabajo

## El esquema elemental

```
ENTRADA  →  PROCESO  →  SALIDA
lo que          ?         lo que
enviamos                obtenemos
```

Durante la primera mitad del recorrido trabajamos los extremos. El centro se abre en el Movimiento IV.

## Principio 05 — El trabajo empieza cuando llega la respuesta

Hasta el botón de enviar aprendemos a entrar. Lo que sigue —leer, detectar qué parte quedó oscura, pedir otra versión, transformar el resultado— concentra casi todo el valor.

Cada mensaje hereda lo dicho antes: basta señalar qué parte quedó pendiente, porque el contexto previo sigue disponible para el sistema.

## El ciclo de trabajo

**Pedir → Recibir → Reaccionar**

| Reaccionar significa | Forma que toma |
|:--|:--|
| Aclarar | Identificamos qué parte quedó oscura |
| Corregir | Ajustamos registro, tono o nivel técnico |
| Profundizar | Pedimos otro ejemplo, paso a paso |
| Transformar | Convertimos el resultado en otro formato |
| Comparar | Contrastamos con la fuente |

Una conversación de trabajo consiste en aproximarse. Empieza como pregunta y termina como transformación de la misma información hasta volverla útil.

## Principio 06 — Cada conversación funciona como un expediente

En mensajería personal conviven asuntos heterogéneos dentro de una misma relación. Aquí gobierna la disciplina inversa: **un problema, un espacio de conversación.**

La razón práctica llega a los tres días, cuando volvemos y encontramos un asunto reconocible. La razón técnica aparece al abrir la caja.

## Principio 07 — Cada entrada abre un abanico de salidas posibles

Las mismas peticiones ejecutadas en conversaciones separadas producen respuestas distintas, y las tres merecen lectura. Al cambiar la entrada, cambia el espacio de salidas.

De ahí que experimentar resulte inevitable: un correo, un Excel, un informe y una imagen piden formulaciones distintas entre sí.

---

# III · La verificación

## Principio 08 — La certeza proviene de la evidencia; el tono proviene de la generación

Cuando una persona afirma algo con seguridad, suponemos alguna razón detrás de esa seguridad. La intuición viaja mal hacia el sistema: **en una respuesta generada, el tono también se genera.**

Preguntar «¿estás seguro?» produce otra respuesta del mismo sistema, que puede corregirse o ratificarse. Para distinguir cuál de las dos ocurrió volvemos a la evidencia.

## El recorrido completo

**Pedir** (resultado + contexto) → **Trabajar** (iterar sobre la respuesta) → **Verificar** (según el riesgo)

La mayoría se detiene en el primer recuadro. La verificación es el paso que decide si el resultado puede sostener algo con consecuencias.

## Verificación proporcional al riesgo

La pregunta útil es **«¿qué pasa si esto está mal?»**.

| Nivel | Ejemplos de uso | Consecuencia del error |
|:--|:--|:--|
| **Riesgo bajo** | Recomendaciones, nombres para una actividad, ideas iniciales | Corregimos o elegimos otra cosa y seguimos con el día |
| **Riesgo intermedio** | Un correo importante, el resumen de un informe, un análisis que vamos a presentar | Nos deja mal parados o nos lleva a una decisión equivocada |
| **Riesgo alto** | Una obligación tributaria, una interpretación legal aplicada, un cálculo financiero | Exigimos origen comprobable antes de usarlo |

> A mayor costo del error → mayor exigencia de verificación.

## Principio 09 — Verificamos en proporción a las consecuencias

La regla rinde más que «verifícalo todo», porque verificarlo todo excede a cualquiera. Al cambiar el tono de un correo trabajamos ligeros; al interpretar una norma trabajamos con la fuente delante.

Las tres categorías funcionan como una forma de razonar. La pregunta operativa permanece constante: **¿qué ocurre mañana si usamos esto y está mal?**

## Principio 10 — Verificar significa abrir la fuente

Cuando el sistema menciona documentación institucional obtenemos una pista, y la comprobación empieza al abrir esa página. El sistema puede citar mal una página, atribuir una afirmación correcta a una fuente equivocada o enlazar un documento real cuyo contenido difiere de lo afirmado.

Diez citas equivalen a diez pistas. Una fuente oficial relevante pesa más que veinte páginas que se copian entre sí: **la evidencia se mide por calidad.**

## Afirmación, evidencia y grado de certeza

| En una persona que informa | En una respuesta generada |
|:--|:--|
| Afirma → Evidencia → **Certeza** | Afirma → Evidencia → **Tono** |
| El vínculo se puede interrogar | El tono se genera junto con el texto y mide estilo |

Un profesional distingue entre «lo comprobé», «lo recuerdo», «creo que es así» y «me falta información». Con un sistema generativo establecemos esa relación por fuera, mediante fuentes.

**Dos movimientos que cambian el trabajo de verificación:**

- **Anclar a la fuente** — entregamos la fuente primaria y pedimos trabajo exclusivo sobre ese documento: interpretarlo, resumirlo, compararlo, explicarlo. Estrecha el margen para inventar, y la comprobación sigue siendo nuestra.
- **Auditar lo ya dicho** — pedimos una revisión de la explicación anterior contra la documentación consultada, separada en tres grupos: lo respaldado directamente, lo que requiere mayor precisión y lo que excede a esa fuente.

Verificamos con ayuda de la propia herramienta mientras conservemos la distinción: «la IA revisó» y «la verdad quedó garantizada» describen hechos diferentes.

## Principio 11 — La herramienta reduce el esfuerzo; la responsabilidad permanece nuestra

Nos acerca a la fuente, la explica y la compara con otra. La decisión que exige precisión vuelve a la fuente, y las consecuencias vuelven a quien firma.

Cuando firmamos, presentamos, decidimos o actuamos sobre esa información, la verificación deja de ser una habilidad de IA y vuelve a ser una habilidad nuestra.

---

# IV · La caja

## Texto y tokens

El modelo procesa unidades llamadas **tokens**. Un token a veces coincide con una palabra completa; otras veces es parte de una palabra, un signo o una terminación.

```
TEXTO → TOKENS → MODELO → TOKENS → TEXTO
```

Nuestras nociones de «fácil» y «difícil» pertenecen a otro sistema de medida. Una tarea trivial para nosotros puede resultar extraña para el modelo, y al revés.

## Principio 12 — El modelo genera una continuación

Trabaja estimando continuaciones a partir del contexto disponible y de las enormes cantidades de relaciones y patrones que aprendió. La imagen del archivador con una ficha por tema pertenece a otra tecnología.

> Una respuesta probable habita el terreno de lo verosímil; la verdad se comprueba aparte. «Útil» y «verdadero» describen cosas distintas.

Ahí nace todo lo que trabajamos en el movimiento anterior.

## Observación 13 — El mecanismo se enuncia simple; sus efectos se despliegan

Decir que un avión produce sustentación por diferencias de presión describe el mecanismo. Cruzar un océano pertenece a otra escala.

**Cuidado con la simplificación inversa:** «escoge la palabra más probable» comprime demasiado, porque la generación admite distintas estrategias. Nos basta con esto: estima continuaciones según el contexto y lo aprendido.

## Modelo y sistema

Usamos un sistema completo. El modelo genera lenguaje, y la empresa construye alrededor búsqueda, ejecución de código, manejo de datos, archivos, imágenes y conectores.

Ante treinta mil filas que requieren una media, preferimos una operación matemática real: el cálculo pertenece a la calculadora.

## Principio 14 — Entrenamiento y contexto son dos procesos

El modelo llega con capacidades aprendidas durante su **entrenamiento**. Después trabaja con el **contexto** disponible en la interacción: nuestro documento, resultados de una búsqueda, datos de una herramienta.

Cuando entregamos un PDF, ese PDF ocupa contexto durante la conversación. La frase «la IA aprendió mi documento» funde dos procesos separados.

## La ventana de contexto

Una conversación dispone de un presupuesto finito medido en tokens. Dentro compiten:

- Instrucciones del sistema
- Historial de la conversación
- Documentos aportados
- Resultados de herramientas
- La respuesta que se está generando

Cuando un componente crece, otro se comprime. Ahí está la razón técnica del Principio 06: cada problema merece su propio espacio de conversación.

Un libro entero, veinte documentos y trescientas páginas de conversación conviven con fidelidad decreciente a lo largo de la interacción.

## Cuatro comportamientos que arrastra el proceso

| # | Comportamiento | Qué es |
|:--|:--|:--|
| 01 | **Sesgos** | Lo aprendido depende de los datos, de su selección y del proceso de entrenamiento. Una máquina hereda la forma de sus datos. |
| 02 | **Ajuste** | Tras el entrenamiento vienen procesos que hacen el sistema más útil, seguro y conversable. Su huella aparece en cada respuesta. |
| 03 | **Estilo** | Listas, títulos, fórmulas de cortesía. Surge del entrenamiento, los ajustes, las instrucciones del sistema y decisiones de producto. |
| 04 | **Sicofancia** | La tendencia a acomodarse a la posición del usuario y a reforzarla más de lo debido. |

El riesgo aparece cuando confundimos amabilidad conversacional con evaluación independiente. Una pregunta que ya contiene la conclusión invita a confirmarla; una pregunta que pide evaluación —beneficios, riesgos, supuestos débiles, escenarios de fracaso— abre espacio para el desacuerdo. **La forma de preguntar pertenece al control de calidad**, además del estilo.

## Principio 15 — Responsabilidad epistémica

Sabemos cuánto respaldo tiene aquello que vamos a usar. Esperamos que el grado de seguridad de una afirmación guarde relación con la evidencia de quien la emite; con un sistema generativo establecemos esa relación por fuera.

«Definitivamente» describe un estilo. «Me falta seguridad» ofrece una señal útil. La medición de la incertidumbre llega desde mecanismos externos, y ahí entran las fuentes.

## El esquema completo

```
ENTRADA → CONTEXTO → MODELO → GENERACIÓN → SALIDA
             ↑                      ↑
        HERRAMIENTAS          ENTRENAMIENTO
   búsqueda · código        sesgos · ajuste
   archivos · datos      sicofancia · incertidumbre

        TOKENS · LÍMITE DE CONTEXTO
```

Todo esto ocurre mientras alguien escribe una pregunta de cuatro palabras. La interfaz vuelve simple la superficie: ahí residen su gran virtud y su gran ocultamiento.

## Principio 16 — Elegimos el sistema que se adapta al trabajo

La pregunta útil apunta al ajuste entre sistema y tarea. Un modelo excelente dentro de un producto ajeno a nuestra necesidad se convierte en mala elección. Investigación, hojas de cálculo, documentos e imágenes piden capacidades distintas alrededor del modelo.

Modelos, productos, precios, límites y capacidades evolucionan muy rápido. Al elegir herramienta para algo serio investigamos el estado actual, con datos de este año.

---

# V · El mapa

## Inteligencia artificial abarca mucho más que un chatbot

| Nivel | Alcance |
|:--|:--|
| **Inteligencia artificial** | Visión, lenguaje, planificación, razonamiento, robótica, aprendizaje |
| **Machine learning** | Aprender patrones desde los datos, en lugar de escribir todas las reglas |
| **Redes neuronales · deep learning** | Las arquitecturas que sostienen ese aprendizaje |
| **IA generativa** | Texto, imágenes, audio, música, video, código |
| **LLM · modelos de lenguaje** | Modelos generativos de texto, con capacidades multimodales |

Es un mapa para orientarse. Algunos conceptos describen campos, otros técnicas, otros tipos de modelos y otros productos; muchas categorías se superponen.

## De un campo entero hasta una caja de texto

| # | Nivel | Contenido |
|:--|:--|:--|
| 1 | Campo | Inteligencia artificial |
| 2 | Tecnologías | Machine learning, deep learning |
| 3 | Modelos | LLM, multimodales |
| 4 | Sistemas | Modelo + herramientas |
| 5 | Productos | ChatGPT, Claude, Gemini |
| 6 | Interfaz | Una caja de texto |
| 7 | **Nosotros** | Quienes decidimos y firmamos |

Decir «la IA» comprime siete niveles en dos palabras. Funciona como abreviatura mientras conozcamos qué hay detrás.

## Principio 17 — El problema pone el límite de lo que aprendemos

Desarrollar, entrenar o personalizar modelos tiene su camino propio: programación, estadística, álgebra lineal, probabilidad, optimización. Para trabajar mejor dominamos primero la zona baja del mapa.

Usamos una hoja de cálculo con provecho mientras la ingeniería eléctrica sigue su curso, y comprender ciertos fundamentos mejora nuestras decisiones. Con ese límite claro, aprendemos aquello que la tarea reclama.

---

# Síntesis

| Movimiento | Fórmula | Idea que sostiene |
|:--|:--|:--|
| **La petición** | Resultado + contexto | Qué queremos obtener y qué necesita saber el sistema para ayudarnos a conseguirlo. |
| **El trabajo** | Pedir → trabajar → verificar | Casi todos nos detenemos en el primer verbo, y ahí se pierde la mayor parte del valor. |
| **La caja** | Entrada → proceso → salida | Un modelo, con tokens, con contexto finito y con herramientas alrededor. |
| **El mapa** | Campo → producto → interfaz | Y al final de la cadena, quien firma, presenta, decide y responde. |

La pregunta inicial era «¿qué tenemos que aprender para dominar la inteligencia artificial?».
Una mejor pregunta: **¿cómo aprendemos a trabajar con ella?**

> Aprender para comprender. Comprender para transformar.