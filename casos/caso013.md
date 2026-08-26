---
titulo: Un contenido, cinco formatos
modulo: Caso 013
area: General
resumen: Por qué elegir el archivo de salida es una decisión distinta de decidir qué debe decir el contenido.
---

## A. Situación

Comercializamos suministros eléctricos. El área técnica recibe la ficha del
3M™ Scotch 9545N en inglés y pide una versión en español. La traducción sale
correcta y entonces empiezan los pedidos: archivo documental la quiere en Word, un
técnico en Markdown, un cliente en PDF, el jefe comercial en PowerPoint y compras
en Excel. La información es la misma cinco veces; el producto final, no.

## B. Objetivo

Distinguir entre el contenido que queremos conservar y la representación en que
necesitamos recibirlo, y reconocer cuándo el cambio de formato obliga a
reorganizar el contenido.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- La ficha técnica 3M™ Scotch 9545N Impregnated Cloth Tape, 2 páginas, en inglés: [pendiente: enlace al PDF oficial de 3M].
- Un equipo capaz de abrir .docx, .xlsx y .pptx, para revisar los archivos generados.

## D. Desarrollo

Recorremos el ciclo **fuente → contenido → estructura → formato → archivo**.

1. **Contenido base.** Adjuntamos la ficha original y pedimos la versión maestra:

       Traduce esta ficha técnica al español conservando terminología
       técnica, cifras, unidades y estructura del contenido.

2. **Salidas forzadas.** Sobre esa misma traducción pedimos, una por turno, cinco
   representaciones distintas:

       Conserva esta traducción como documento Markdown estructurado (.md).
       Genera una ficha técnica editable en Word (.docx).
       Genera una versión final preparada para distribución (.pdf).
       Convierte la información esencial en una presentación técnica breve (.pptx).
       Estructura las especificaciones en una hoja de cálculo con una
       característica por fila (.xlsx).

3. **Comparación.** Abrimos los cinco archivos y observamos qué le pasó a la misma
   información. El Markdown y el Word conservan casi toda la estructura original.
   El PDF la congela para distribuir. El PowerPoint obliga a seleccionar y
   jerarquizar: no cabe todo. El Excel obliga a descomponer el texto en campos y
   registros: lo que era un párrafo se vuelve fila y columna.
4. **Rutas.** Repetimos el ejercicio en ChatGPT, Gemini y Claude, y anotamos por
   dónde llegamos a cada archivo:

   | Salida | Ruta típica |
   | --- | --- |
   | .md | respuesta en el chat, lienzo editable o artefacto, y luego guardar |
   | .docx | creación directa del archivo, o lienzo → editor ofimático → exportar |
   | .pdf | creación directa, o exportación desde un documento ya generado |
   | .pptx | creación directa, o lienzo → herramienta de diapositivas → exportar |
   | .xlsx | creación directa, o generación en hoja de cálculo → descargar |

   La tabla vale como mapa de rutas y no como catálogo de compatibilidad: estas
   capacidades cambian rápido y dependen del plan y del entorno.
5. **Dos caminos.** Buscamos deliberadamente dos rutas distintas hacia el mismo
   `.pptx` o el mismo `.docx` y las comparamos: cuál conserva mejor el formato,
   cuál permite editar antes de exportar.

> El pedido «tradúcelo» y el pedido «dámelo en Excel» no piden lo mismo. El
> segundo no cambió la información: cambió qué podíamos hacer con ella después.

## E. Conceptos

- **Contenido:** información que queremos conservar.
- **Estructura:** organización lógica de esa información.
- **Formato:** representación empleada para expresar el contenido.
- **Archivo:** implementación concreta del resultado, como .docx, .pdf o .xlsx.
- **Salida forzada:** especificación explícita del archivo que esperamos recibir.
- **Conversión:** transformación de una representación en otra.

## F. Comprobación

Un compañero sostiene que pasar la ficha a PowerPoint o a Excel es solo cambiar
el formato, y que por eso los cinco archivos contienen exactamente lo mismo.
¿Dónde se rompe esa equivalencia?

- a) En la fidelidad visual, porque cada archivo aplica sus propias fuentes, márgenes y estilos, y la ficha termina viéndose distinta en cada uno de los cinco.
- b) En que seleccionar y descomponer son decisiones sobre el contenido.
- c) En la ruta de generación, dado que cada asistente llega al archivo por un camino diferente y el resultado depende del plan contratado y de la superficie utilizada.
- d) En el momento de la traducción, ya que al pedir cada formato el asistente vuelve sobre la ficha original y puede resolver los términos técnicos de otra manera.
