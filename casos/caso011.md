---
titulo: Del prompt escrito al prompt reutilizable
modulo: Caso 011
area: General
resumen: Cómo una instrucción que funciona deja de vivir dentro del chat y pasa a ser un archivo que se guarda, se modifica y se transporta.
---

## A. Situación

Documentamos las sesiones de un curso de capacitación. Después de cada clase nos
llega la transcripción automática en Word —cuatro horas de explicaciones,
intervenciones, ejemplos e indicaciones administrativas, decenas de páginas— y la
convertimos en informe con ayuda de la IA. El prompt que armamos en el chat
funcionó. El problema aparece ahora: la sesión dos es la semana próxima, y la
tres, y la cuatro.

## B. Objetivo

Comprender en qué momento una instrucción deja de ser un mensaje de conversación
y empieza a comportarse como un recurso de trabajo que se conserva y se mantiene.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- Un editor de texto plano: Bloc de notas, TextEdit o similar.
- La transcripción de una sesión en Word, y la de una sesión posterior para reutilizar el archivo.

## D. Desarrollo

Recorremos el ciclo **prompt en chat → estructurar → Markdown → guardar → reutilizar**.

1. **Recuperar.** Volvemos al chat y copiamos el prompt que produjo el informe:
   el que empezaba «Actúa como asistente académico. Convierte la transcripción en
   un informe de la sesión…».
2. **Estructurar.** Lo desarmamos en sus componentes —rol, objetivo, salida,
   advertencias, contexto— y notamos que ya estaban ahí, mezclados en un párrafo.
3. **Convertir.** Los separamos con seis marcas de Markdown y nada más:
   `#` para el título, `##` para cada sección, `-` para las listas, `**` para
   resaltar, `>` para una nota al margen y la sangría de cuatro espacios para lo
   que deba copiarse literal. En el editor escribimos:

       # Informe de sesión

       ## Rol

       Actúa como asistente académico.

       ## Objetivo

       Convierte la transcripción proporcionada en un informe de la sesión.

       ## Salida

       El informe incluye:

       - temas trabajados;
       - conceptos principales;
       - actividades realizadas;
       - ejemplos desarrollados;
       - herramientas mencionadas;
       - conclusiones.

       ## Advertencias

       - Utiliza únicamente información presente en la transcripción.
       - Distingue el contenido académico de las indicaciones administrativas.
       - Conserva nombres y términos técnicos cuando sean relevantes.

       ## Contexto

       La transcripción corresponde a una sesión del curso Inteligencia
       Artificial Aplicada. El informe servirá como registro académico.

4. **Guardar.** Lo guardamos como `informe_sesion.md`, fuera del chat.
5. **Reutilizar.** En una conversación nueva adjuntamos el archivo junto con la
   transcripción de otra sesión y escribimos:

       Aplica las instrucciones de informe_sesion.md a la transcripción
       adjunta.

6. **Mantener.** Abrimos el archivo y le hacemos tres cambios: agregamos la
   sección `## Participaciones relevantes`, pedimos en la salida un informe de
   máximo dos páginas, y sumamos una advertencia para diferenciar las afirmaciones
   del docente de las intervenciones de los estudiantes. Guardamos y volvemos a
   adjuntarlo.
7. **Contraste.** Comparamos este recorrido con la alternativa: abrir el Word,
   releer el párrafo largo, editar la parte correcta sin romper el resto y pegarlo
   de nuevo en cada sesión.

> Los tres cambios tomaron tres líneas y ninguna relectura. La estructura no
> adornó la instrucción: la volvió modificable.

## E. Conceptos

- **Markdown:** formato de texto ligero que representa la estructura con caracteres simples.
- **Archivo .md:** extensión habitual de un documento escrito en Markdown.
- **Texto plano con estructura:** contenido legible a la vez por una persona y por una máquina.
- **Prompt reutilizable:** instrucción conservada como archivo, independiente de la conversación donde nació.
- **Mantenimiento:** modificación de una instrucción en un solo lugar, sin rehacerla.

## F. Comprobación

Un compañero sostiene que guardar la instrucción en Markdown en lugar de Word es
una preferencia estética, porque el texto que lee la IA termina siendo el mismo.
¿Dónde se rompe esa equivalencia?

- a) En que las marcas hacen visible la estructura al adjuntar el archivo.
- b) En el peso del archivo, ya que un .md ocupa una fracción de un .docx y se transporta entre herramientas sin pérdidas de formato ni conversiones intermedias.
- c) En la compatibilidad, porque no todos los asistentes admiten documentos de Word como adjunto y algunos exigen pegar el contenido dentro de la conversación.
- d) En el orden de las secciones, dado que Word tiende a reacomodar los títulos al copiar y la instrucción llega al asistente con los componentes desordenados.
