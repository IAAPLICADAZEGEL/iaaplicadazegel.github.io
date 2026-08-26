---
titulo: Comprar una laptop
modulo: Caso 007
area: General
resumen: Cómo un chat se convierte en espacio de trabajo cuando la decisión se afina a lo largo de la conversación.
---

## A. Situación

Necesitamos comprar una laptop para trabajo administrativo y uso personal, con un
tope de S/ 3,500. Tenemos claras las necesidades principales y sabemos armar un
buen pedido inicial. Lo que no anticipamos es que, apenas veamos la primera
comparación, aparecerán condiciones en las que no habíamos pensado.

## B. Objetivo

Comprender cómo una conversación sostenida en un mismo chat desarrolla una
decisión que el pedido inicial, por bien construido que esté, no alcanza a cerrar.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- Un chat nuevo, dedicado únicamente a esta decisión.

## D. Desarrollo

Recorremos el ciclo **prompt inicial → respuesta → aclarar → profundizar → corregir → ampliar → iterar → transformar**.

1. **Prompt inicial.** Abrimos un chat nuevo y escribimos:

       Recomiéndame una laptop adecuada para trabajo administrativo y uso
       personal.
       - Presupuesto máximo: S/ 3,500.
       - Principalmente usaré Office, navegación web, videollamadas y
         análisis básico de datos.
       - Quiero transportarla diariamente.
       - Prioriza buena autonomía y durabilidad.
       - Propón tres alternativas y compáralas.

2. **Aclarar.** Al leer la comparación recordamos un uso que omitimos:

       Me acabo de dar cuenta de que también utilizaré Power BI.
       ¿Cambia tu recomendación?

3. **Profundizar.** Pedimos las razones detrás de la preferencia:

       ¿Por qué priorizas ese modelo sobre los otros dos?

4. **Corregir.** Descartamos lo que no aplica a nuestro entorno:

       Prefiero Windows. Descarta cualquier alternativa con otro sistema
       operativo.

5. **Ampliar el contexto.** Sumamos una condición de uso doméstico:

       Además, quiero conectarla a dos monitores cuando trabaje desde casa.

6. **Iterar.** Cerramos con una evaluación que integre todo lo conversado:

       Con todo lo que hemos conversado, vuelve a evaluar las alternativas
       y dame tu recomendación final.

7. **Transformar.** Reutilizamos el resultado en otra forma:

       Convierte la comparación final en una tabla.

> Ninguno de los seis mensajes posteriores repitió el presupuesto ni los usos
> iniciales: el chat los seguía sosteniendo. El pedido abrió el trabajo y la
> conversación lo construyó.

## E. Conceptos

- **Iteración:** mejora progresiva de un resultado mediante nuevas interacciones.
- **Contexto conversacional:** información acumulada en el chat que da sentido a los mensajes siguientes.
- **Profundización:** exploración de las razones, detalles o implicaciones de una respuesta.
- **Transformación:** reutilización de un resultado previo para producir otra representación.
- **Chat como espacio de trabajo:** conversación dedicada al desarrollo progresivo de un problema.

## F. Comprobación

Un compañero sostiene que toda esta conversación era evitable: bastaba con
escribir desde el inicio un prompt que incluyera Power BI, Windows y los dos
monitores. ¿Dónde se rompe ese razonamiento?

- a) En que esos tres requisitos aparecieron al leer las respuestas.
- b) En que un prompt inicial con siete condiciones excede lo que un asistente procesa de una vez y termina ignorando las últimas de la lista.
- c) En que la profundización y la transformación son pasos que exigen un resultado previo, de modo que ningún pedido único puede contenerlos por más completo que sea.
- d) En que el asistente responde mejor a mensajes cortos y sucesivos que a uno extenso, porque cada turno le permite recalcular la comparación desde cero.
