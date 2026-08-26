---
titulo: De una imagen a datos utilizables
modulo: Caso 017
area: General
resumen: Cuándo basta el chatbot para recuperar el texto de una imagen y cuándo el volumen convierte esa tarea en un proceso documental.
---

## A. Situación

Trabajamos en un área administrativa donde todavía llegan documentos como
fotografías. Un compañero nos manda por WhatsApp la foto de un comprobante,
frontal y bien iluminada, y necesitamos el texto para seguir trabajando. Lo
resolvemos en segundos. Días después llegan 180 escaneos que deben digitalizarse,
revisarse y archivarse con un criterio uniforme, y la misma tarea deja de
parecerse a la anterior.

## B. Objetivo

Distinguir cuándo una extracción de texto se resuelve con la herramienta general
que ya usamos y cuándo el volumen y la exigencia de control piden una solución
especializada.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- La fotografía de un documento propio: un comprobante, una factura o una boleta.
- Para el escenario por lotes, una herramienta de OCR especializada como [ABBYY FineReader PDF](https://pdf.abbyy.com).

## D. Desarrollo

Recorremos el ciclo **imagen → reconocer → extraer → verificar → utilizar**.

1. **Extraer.** Adjuntamos la fotografía al asistente y escribimos:

       OCR esta imagen. Conserva cifras, fechas, nombres y estructura del
       contenido.

2. **Verificar.** Ponemos la imagen y el texto lado a lado y comprobamos lo que
   más se distorsiona: montos, fechas, números de documento, ceros y unos, letras
   con tilde.
3. **Encadenar.** Como ya es texto, seguimos con las operaciones de siempre:

       Organiza los datos extraídos en una tabla con fecha, descripción,
       número de documento y monto.

4. **Cambiar la escala.** Planteamos ahora los 180 documentos y anotamos qué
   aparece que antes no existía: procesamiento por lotes, reconocimiento
   consistente entre archivos, revisión sistemática, conservación de la estructura,
   exportación y control del flujo documental.
5. **Contrastar herramientas.** Procesamos un pequeño lote —cinco o seis
   escaneos— con la herramienta especializada y comparamos con el mismo lote
   pasado uno por uno por el chat: tiempo total, uniformidad del resultado y
   esfuerzo de revisión.

> Con un comprobante, verificar cuesta diez segundos. Con 180, verificar es el
> trabajo. La tarea no cambió de dificultad: cambió de naturaleza.

## E. Conceptos

- **OCR (optical character recognition):** conversión del texto contenido en una imagen en caracteres digitales.
- **IA multimodal:** modelo capaz de recibir imágenes además de texto y operar sobre ambas.
- **Procesamiento por lotes:** tratamiento de muchos documentos con un procedimiento uniforme.
- **Verificación:** comprobación del texto extraído contra el documento original.
- **Proceso documental:** conjunto de pasos repetibles que llevan un documento desde su ingreso hasta su conservación.

## F. Comprobación

Un compañero sostiene que, como el chatbot extrajo el comprobante sin un solo
error, conviene procesar así los 180 escaneos y ahorrarse la herramienta
especializada. ¿Dónde se rompe ese razonamiento?

- a) En la capacidad del asistente, porque los planes tienen límites de adjuntos y de mensajes que impedirían completar un lote de ese tamaño en una sola sesión de trabajo.
- b) En que el cuello de botella pasa a ser la verificación.
- c) En la consistencia del reconocimiento, dado que cada conversación resuelve la imagen por separado y el mismo campo puede quedar rotulado de maneras distintas entre documentos.
- d) En la exportación del resultado, ya que el texto obtenido en el chat debe trasladarse a mano hacia el sistema documental en lugar de generarse directamente en el formato requerido.
