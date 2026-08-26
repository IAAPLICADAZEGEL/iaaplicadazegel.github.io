---
titulo: Cuando el análisis se convierte en código
modulo: Caso 025
area: General
resumen: Por qué conservar el procedimiento, y no solo el resultado, cambia lo que podemos hacer con un análisis que se repite.
---

## A. Situación

Venimos calculando métricas, generando gráficos y armando tableros con ayuda de la
IA. Ahora el mismo análisis hay que repetirlo cada mes, con datos nuevos. Podríamos
rehacer la conversación entera, y saldrían resultados; lo que no quedaría es la
certeza de haber hecho exactamente lo mismo que el mes anterior.

## B. Objetivo

Comprender qué se gana al conservar el procedimiento de un análisis como código
ejecutable, además de sus resultados.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- Uno de los datasets del bloque: `002-A-gastos_ejecutivos.xlsx`, `002-B-gastos_personales.xlsx` o `002-C-ventas_ultimos_3m.xlsx`.
- Una cuenta de Google para trabajar en [Google Colab](https://colab.research.google.com).
- Opcionalmente, un entorno Jupyter instalado en el equipo.

## D. Desarrollo

Recorremos el ciclo **datos + objetivo → IA → código → ejecutar → resultado → reejecutar**.

1. **Pedir el procedimiento.** Cambiamos lo que solicitamos: no el análisis, sino
   el modo de producirlo:

       Genera el código Python necesario para reproducir este análisis: carga
       el Excel, calcula las métricas descriptivas principales y genera los
       gráficos correspondientes. Utiliza bibliotecas habituales de análisis
       de datos.

2. **Ejecutar en el navegador.** Abrimos Google Colab, subimos el dataset, pegamos
   el código y ejecutamos las celdas. Corregimos lo que falle: rutas, nombres de
   columna, tipos de dato.
3. **Trabajar con la IA dentro del entorno.** Usamos la asistencia disponible en el
   propio Colab para explicar o modificar partes del código, y comparamos ese
   recorrido con el anterior: pedir fuera, copiar y pegar, ejecutar.
4. **Ejecutar en nuestro equipo.** Repetimos el mismo análisis en un entorno
   Jupyter local y verificamos si las métricas principales coinciden con las de
   Colab.
5. **Modificar la pregunta.** Cambiamos el eje del análisis:

       En lugar de analizar por categoría, compara los resultados por mes.

   Ajustamos el código con ayuda de la IA y volvemos a ejecutar.
6. **Reejecutar con datos nuevos.** Sustituimos el archivo por otro de estructura
   compatible y corremos el notebook sin tocar una línea. Guardamos el par
   `analisis.ipynb` + dataset como la unidad que conservamos.

> El notebook produjo los mismos números dos veces, en dos entornos distintos. Eso
> no lo puede afirmar una conversación, por buena que haya sido.

## E. Conceptos

- **Python:** lenguaje ampliamente utilizado para análisis de datos.
- **Notebook:** documento ejecutable organizado en celdas.
- **Biblioteca:** conjunto reutilizable de funcionalidades disponible para un lenguaje.
- **Reproducibilidad:** capacidad de repetir un procedimiento y obtener resultados consistentes en las mismas condiciones.
- **Procedimiento ejecutable:** análisis conservado en una forma que puede inspeccionarse, corregirse y volver a correr.

## F. Comprobación

Un compañero sostiene que pedir código es un rodeo innecesario, porque el chat ya
entrega las métricas y los gráficos correctos en la mitad del tiempo. ¿Dónde se
rompe ese razonamiento?

- a) En la inspección de los cálculos, porque el código deja a la vista qué filas se descartaron y cómo se agruparon, mientras que la conversación solo muestra el número final.
- b) En que la conversación entrega el resultado y no el procedimiento.
- c) En la comparación entre periodos, dado que dos conversaciones distintas pueden resolver el mismo pedido con criterios diferentes y volver no comparables los meses analizados.
- d) En el tiempo total, ya que la ventaja inicial del chat se pierde apenas el análisis debe repetirse mes a mes sobre datos nuevos con la misma estructura.
