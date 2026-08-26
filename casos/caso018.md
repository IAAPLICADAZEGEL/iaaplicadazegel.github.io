---
titulo: Aprender a preguntar a los datos
modulo: Caso 018
area: General
resumen: Qué tipos de pregunta admite un conjunto de datos, y cómo cada una lo muestra desde un ángulo distinto.
---

## A. Situación

Llevamos meses registrando los gastos personales en una hoja de cálculo: fecha,
categoría, monto, descripción y método de pago. Los datos están completos y
ordenados. Aun así, mirar las cincuenta filas una por una no nos dice qué está
pasando con nuestras finanzas, y no sabemos bien qué habría que preguntarle al
archivo.

## B. Objetivo

Reconocer los tipos de pregunta que un conjunto de datos puede responder y qué
muestra cada uno.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El archivo `002-B-gastos_personales.xlsx`, con 50 registros: fecha, categoría, monto, descripción y método de pago.

## D. Desarrollo

Recorremos el ciclo **datos → pregunta → métrica → comparación → interpretación**.

1. **Pregunta abierta.** Adjuntamos el archivo y empezamos como en cualquier
   conversación:

       ¿Qué puedes decirme sobre mis gastos?

   Anotamos qué eligió mostrarnos sin que se lo pidiéramos.
2. **Magnitud.** Preguntamos por el acumulado:

       ¿Cuánto gasté en total?

3. **Tendencia central.** Pedimos dos medidas juntas, para poder compararlas:

       ¿Cuál es el gasto promedio y cuál es la mediana?

   Si difieren mucho, algo en la distribución está tirando del promedio.
4. **Distribución.** Agrupamos y comparamos participaciones:

       ¿Cómo se distribuyen los gastos entre las diferentes categorías?

5. **Evolución.** Incorporamos el tiempo:

       Genera un gráfico que muestre cómo evolucionaron mis gastos a lo
       largo del tiempo.

6. **Valores relevantes.** Buscamos lo que se sale del patrón:

       ¿Qué registros se alejan considerablemente del comportamiento
       habitual?

7. **Revisión.** Volvemos sobre las seis respuestas y anotamos qué pregunta
   respondió cada una: contar, resumir, distribuir, comparar, evolucionar,
   detectar.

> Los datos fueron siempre los mismos cincuenta registros. Lo que cambió en cada
> paso fue qué le pedimos que mirara.

## E. Conceptos

- **Variable:** característica registrada para cada observación.
- **Registro:** observación individual del conjunto de datos.
- **Métrica:** medida calculada a partir de los datos.
- **Tendencia central:** valor que representa el centro de una distribución.
- **Distribución:** forma en que los valores se reparten.
- **Valor atípico:** observación considerablemente distinta de las demás.

## F. Comprobación

Un compañero calcula el gasto promedio del mes, lo compara con el del mes
anterior y concluye que ya sabe cómo gastó. ¿Qué le respondemos?

- a) Que el promedio de un mes con pocos registros resulta poco estable y bastaría un solo movimiento tardío para desplazarlo por encima o por debajo del mes anterior.
- b) Que faltaría incorporar la dimensión temporal dentro del mes, porque dos meses con idéntico promedio pueden concentrar el gasto en semanas muy distintas.
- c) Que el promedio no muestra cómo se reparten los gastos.
- d) Que las categorías no participan por igual en el total, de modo que la comparación entre meses exige revisar antes si la composición del gasto se mantuvo.
