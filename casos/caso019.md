---
titulo: La IA como analista de datos
modulo: Caso 019
area: General
resumen: Cómo conducir un análisis descriptivo conversando con el archivo, y dónde separar el dato de la interpretación.
---

## A. Situación

En el área administrativa registramos los gastos ejecutivos de los colaboradores:
fecha, empleado, departamento, categoría, monto, descripción y medio de pago.
Gerencia quiere entender cómo se están distribuyendo. Abrir el Excel y revisarlo
a mano tomaría la tarde; el archivo, en cambio, puede adjuntarse.

## B. Objetivo

Comprender cómo se conduce un análisis descriptivo conversando con un archivo, y
distinguir el dato observado de la interpretación y de la explicación causal.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El archivo `002-A-gastos_ejecutivos.xlsx`, con las variables fecha, empleado, departamento, categoría, monto, descripción y medio de pago.
- Capacidad del asistente para trabajar con archivos adjuntos.

## D. Desarrollo

Recorremos el ciclo **archivo → inspeccionar → calcular → visualizar → interpretar**.

1. **Inspeccionar.** Antes de pedir cálculos, verificamos qué hay:

       Identifica las columnas, tipos de información y cantidad de registros
       disponibles.

2. **Calcular.** Pedimos las medidas básicas en un solo turno:

       Calcula el gasto total, el promedio y la mediana. Identifica las
       principales categorías y el gasto por departamento.

3. **Visualizar.** Elegimos representaciones según lo que queremos ver:

       Genera un gráfico de la evolución temporal de los gastos, uno de
       participación por categoría y uno de comparación entre departamentos.

4. **Interpretar.** Pedimos lectura, no solo números:

       ¿Cuáles son los principales patrones que observas?

5. **Delimitar.** Tomamos cada conclusión del informe y la clasificamos en tres
   columnas: qué es dato observado, qué es interpretación nuestra o del asistente,
   y qué sería una explicación causal que el archivo no puede sostener.
6. **Revisar valores.** Cerramos con lo que merece atención humana:

       ¿Qué registros merecen una revisión particular y por qué?

> El paso 5 no calcula nada y es el que más cambia el informe. Sin él, una
> observación bien redactada pasa por una explicación.

## E. Conceptos

- **Dataset:** conjunto organizado de datos.
- **Análisis descriptivo:** caracterización de lo que muestran los datos.
- **Agregación:** combinación de registros mediante suma, promedio o conteo.
- **Visualización:** representación gráfica de la información.
- **Interpretación:** significado que atribuimos a los patrones observados.
- **Explicación causal:** afirmación sobre las causas, que exige evidencia externa al dataset.

## F. Comprobación

Al ver que Operaciones registra el mayor gasto de todos los departamentos, un
compañero concluye que administra peor sus recursos. ¿Dónde se rompe esa
conclusión?

- a) En que el dato dice cuánto se gastó, no por qué.
- b) En la comparación entre departamentos, porque no se normalizó el gasto por número de colaboradores ni por volumen de operación de cada área durante el periodo.
- c) En la composición del gasto, dado que un departamento puede concentrar categorías inevitablemente más costosas sin que eso indique nada sobre su gestión.
- d) En el periodo analizado, ya que tres meses de registros pueden recoger un desembolso extraordinario que no representa el comportamiento habitual del área.
