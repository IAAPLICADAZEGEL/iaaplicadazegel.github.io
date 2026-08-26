---
titulo: ¿Qué IA analiza mejor mis datos?
modulo: Caso 020
area: General
resumen: Cómo comparar herramientas de IA ejecutando el mismo trabajo en todas, en lugar de contrastar sus funciones declaradas.
---

## A. Situación

La empresa tiene acceso a varios servicios de IA y hay que decidir con cuál
trabajaremos habitualmente los archivos de datos. Las páginas de cada producto
prometen lo mismo con palabras distintas. Tenemos un Excel de gastos ejecutivos y
una tarde: es más barato probar que leer comparativas.

## B. Objetivo

Comprender cómo se compara una herramienta con otra ejecutando el mismo trabajo, y
qué aporta poder inspeccionar cómo llegó a su resultado.

## C. Requerimientos

- Cuenta activa en los tres asistentes, para comparar entre ellos:
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El archivo `002-A-gastos_ejecutivos.xlsx`.
- Una hoja aparte para registrar las observaciones de cada servicio.

## D. Desarrollo

Recorremos el ciclo **mismo archivo + mismas preguntas → distintas IA → comparar**.

1. **Fijar la prueba.** Escribimos una sola vez el pedido que usaremos idéntico en
   los tres servicios:

       1. Calcula el gasto total y promedio.
       2. Identifica las tres principales categorías.
       3. Compara los departamentos.
       4. Genera un gráfico temporal.
       5. Identifica valores relevantes.
       6. Explica cómo obtuviste los resultados.

2. **Ejecutar.** Cargamos el mismo archivo en cada servicio y pegamos el mismo
   pedido, sin ayudarle a ninguno con aclaraciones extra.
3. **Registrar.** Anotamos para cada uno: si aceptó el Excel, si entendió las
   columnas, si los cálculos salieron, qué gráficos produjo, si explicó el
   procedimiento, si mostró código, con qué límites nos topamos, qué pudimos
   exportar y qué tan cómodo resultó el trabajo.
4. **Contrastar los números.** Ponemos el total, el promedio y la mediana de los
   tres lado a lado. Si alguno difiere, buscamos dónde: filas vacías, montos con
   texto, fechas mal interpretadas.
5. **Comparar planes.** Repetimos las operaciones que podamos en versión gratuita
   y de pago, y anotamos qué cambia realmente: velocidad, tamaño de archivo,
   gráficos, exportación.
6. **Decidir.** Elegimos no la mejor en abstracto, sino la que sostiene mejor este
   flujo de trabajo, considerando calidad, capacidades, límites, velocidad y costo.

> Dos servicios devolvieron el mismo total. Solo uno mostró cómo lo calculó, y ahí
> apareció que uno de los dos había descartado seis filas.

## E. Conceptos

- **Capacidad:** operaciones que una herramienta puede realizar.
- **Límite de uso:** restricción asociada al servicio o al plan.
- **Transparencia:** posibilidad de inspeccionar cómo se obtuvo un resultado.
- **Validación cruzada:** comparación de resultados obtenidos por métodos o herramientas distintas.
- **Flujo de trabajo:** secuencia de tareas reales que la herramienta debe sostener.

## F. Comprobación

Un compañero comprueba que dos servicios devuelven exactamente el mismo gasto
total y propone quedarse con el más rápido, porque el resultado ya está
confirmado. ¿Dónde se rompe ese razonamiento?

- a) En la velocidad como criterio, porque el tiempo de respuesta importa menos que los límites de tamaño de archivo cuando el dataset crezca en los próximos meses.
- b) En la exportación de resultados, dado que dos herramientas igualmente exactas pueden diferir en si permiten llevarse los gráficos y las tablas al informe final.
- c) En la comparación misma, ya que un solo indicador coincidente no dice nada sobre cómo se comportarán ambas herramientas frente a las demás operaciones del análisis.
- d) En que coincidir en el número no garantiza el mismo cálculo.
