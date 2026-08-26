---
titulo: Del Excel a un dashboard autónomo
modulo: Caso 021
area: General
resumen: Cómo convertir una hoja de cálculo en una página que se abre en el navegador y trae los datos dentro.
---

## A. Situación

Tenemos un Excel con cincuenta gastos personales y ya sabemos analizarlo
conversando. El problema es que cada consulta nueva exige volver al chat, adjuntar
otra vez el archivo y reconstruir el contexto. Queremos algo que se abra, se mire y
responda las preguntas de siempre sin intermediarios.

## B. Objetivo

Comprender qué agrega una representación visual interactiva sobre los mismos datos
y qué implica que esos datos viajen dentro del archivo que los muestra.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El archivo `002-B-gastos_personales.xlsx`, con 50 registros.
- Un navegador web para abrir el resultado.

## D. Desarrollo

Recorremos el ciclo **Excel → IA → datos + HTML + CSS + JavaScript → dashboard**.

1. **Pedir.** Adjuntamos el Excel y solicitamos la pieza completa:

       Convierte estos datos en un dashboard HTML interactivo. Incluye todos
       los registros directamente dentro del archivo para que funcione sin
       depender del Excel original.

2. **Especificar.** Detallamos qué debe contener, porque un dashboard sin destino
   se llena de gráficos decorativos:

       Incluye gasto total, promedio, cantidad de registros, evolución
       temporal, gastos por categoría, métodos de pago, principales gastos,
       filtros y la tabla completa.

3. **Guardar.** Conservamos el resultado como `dashboard_gastos.html`.
4. **Probar la autonomía.** Movemos el Excel original a otra carpeta, o lo
   renombramos, y abrimos el HTML en el navegador. Si todo sigue funcionando, los
   datos viajaban dentro.
5. **Explorar.** Usamos los filtros para responder tres preguntas que antes exigían
   una consulta al chat, y anotamos cuáles no puede responder.
6. **Cambiar el formato de origen.** Repetimos la generación entregando los mismos
   datos como CSV y como PDF, y observamos qué pasa con la estructura y con el
   esfuerzo de procesamiento en cada caso.

> El dashboard responde al instante las preguntas que previmos al pedirlo. Para
> cualquier otra, seguimos necesitando los datos y una conversación.

## E. Conceptos

- **Dashboard:** interfaz que reúne indicadores y visualizaciones para explorar información.
- **HTML:** lenguaje que estructura una página web.
- **CSS:** reglas que controlan su presentación.
- **JavaScript:** lenguaje que aporta comportamiento e interacción.
- **Datos incrustados:** información almacenada dentro del propio archivo que la muestra.
- **HTML monolítico:** documento que concentra estructura, estilos, lógica y datos.

## F. Comprobación

Un compañero abre el dashboard, lo encuentra más cómodo que la hoja de cálculo y
propone dejar de usar el Excel para estos gastos. ¿Qué se pierde en el camino?

- a) La posibilidad de corregir un registro mal cargado, porque el dashboard presenta la información pero no ofrece ningún mecanismo para editarla ni para volver a guardarla.
- b) La libertad de preguntar lo que no estaba previsto al construirlo.
- c) La compatibilidad con el resto del equipo, dado que una hoja de cálculo se abre y se comparte con herramientas que todos ya tienen instaladas en sus equipos.
- d) La vigencia de los indicadores, ya que los datos quedaron incrustados en el archivo y cualquier gasto posterior exigirá generar el dashboard nuevamente desde cero.
