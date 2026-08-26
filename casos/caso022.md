---
titulo: Separar los datos de la visualización
modulo: Caso 022
area: General
resumen: Cómo construir una aplicación a partir de la estructura de los datos, sin entregar todos los registros.
---

## A. Situación

Una empresa registra sus ventas de forma continua: ya van 120 operaciones y el
archivo sigue creciendo cada semana. Necesitamos una visualización, pero incrustar
los datos dentro de ella significaría rehacerla cada lunes. Además, el archivo
completo contiene información que preferiríamos no adjuntar a un chat.

## B. Objetivo

Comprender que una aplicación puede construirse a partir de la estructura de los
datos, y qué se gana al mantener los registros fuera de ella.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El archivo `002-C-ventas_ultimos_3m.xlsx`, con fecha, producto, cantidad, precio unitario, total, canal de venta, método de pago y región.
- Un navegador web.

## D. Desarrollo

Recorremos el ciclo **muestra → estructura → aplicación**, y después **archivo real → aplicación → visualización**.

1. **Entregar la estructura.** En lugar del archivo completo, damos una fila de
   ejemplo que muestre cada campo y su tipo:

       Fecha: 2025-05-11
       Producto: Cámara DSLR
       Cantidad: 9
       Precio Unitario: 978.75
       Total: 8808.75
       Canal: Venta telefónica
       Pago: PayPal
       Región: Centro

2. **Pedir la aplicación.** Sobre esa estructura solicitamos la pieza:

       Construye un dashboard HTML compatible con esta estructura. Los datos
       reales serán cargados posteriormente desde un archivo externo. Incluye
       indicadores, gráficos, filtros, tabla y un mecanismo de carga del
       archivo.

3. **Incorporar los datos.** Recién ahora cargamos `002-C-ventas_ultimos_3m.xlsx`
   en el dashboard ya construido.
4. **Probar.** Comprobamos que interpreta bien cada campo: que las fechas ordenen,
   que los montos sumen, que las regiones agrupen.
5. **Forzar el cambio.** Agregamos veinte operaciones al archivo y lo volvemos a
   cargar, sin tocar el HTML. Si la visualización se actualiza, la separación
   funciona.
6. **Probar el límite.** Cambiamos el nombre de una columna en el archivo y
   observamos qué ocurre: ahí aparece de qué depende realmente la aplicación.

> Nunca le entregamos las 120 operaciones y aun así el dashboard las interpreta.
> Lo que necesitaba conocer era la forma de los datos, no su contenido.

## E. Conceptos

- **Esquema:** definición de la estructura que siguen los datos.
- **Muestra:** subconjunto empleado para representar un conjunto mayor.
- **Datos externos:** información almacenada de forma independiente de la aplicación.
- **Separación de responsabilidades:** mantener con vida propia componentes de función distinta.
- **Compatibilidad:** correspondencia entre el archivo y lo que la aplicación espera recibir.

## F. Comprobación

Un compañero objeta que construir el dashboard con una sola fila de ejemplo es
trabajar a ciegas, y que sin las 120 operaciones el resultado será poco confiable.
¿Dónde se rompe esa objeción?

- a) En el volumen como criterio, porque adjuntar 120 registros tampoco garantiza que la herramienta los recorra completos antes de proponer los indicadores del tablero.
- b) En la sensibilidad de la información, dado que entregar operaciones reales a un servicio externo introduce un riesgo que la fila de ejemplo evita por completo.
- c) En que la aplicación se construye sobre la estructura, no sobre los registros.
- d) En la utilidad de la muestra, ya que una fila bien elegida contiene cada campo con su tipo y su formato, que es exactamente lo que el código necesita anticipar.
