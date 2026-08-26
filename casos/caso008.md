---
titulo: Volvamos a la laptop
modulo: Caso 008
area: General
resumen: Qué sobrevive y qué se diluye cuando un mismo chat acumula varios asuntos y luego hay que retomar el primero.
---

## A. Situación

En el chat de la laptop dejamos definidos presupuesto, sistema operativo,
programas, autonomía, movilidad y conexión a monitores. Días después volvemos a
esa misma conversación —está a mano— para preparar una exposición, redactar un
par de mensajes y resolver otras consultas sueltas. Hoy retomamos la compra, y no
recordamos con exactitud en qué habíamos quedado.

## B. Objetivo

Reconocer hasta dónde una conversación conserva el contexto de un problema
cuando entre medio se han tratado otros asuntos.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El chat del Caso 007, con la recomendación final ya obtenida.
- Anotado aparte, lo que quedó decidido allí: presupuesto, requisitos y modelo recomendado.

## D. Desarrollo

Recorremos el ciclo **problema A → contexto A → problema B → contexto acumulado → regreso al problema A → recuperación**.

1. **Cambiar de asunto.** Sin abrir un chat nuevo, escribimos en el mismo hilo:

       Mañana tengo una exposición sobre liderazgo. Ayúdame a organizarla
       para 10 minutos.

2. **Continuar el nuevo asunto.** Lo desarrollamos durante varios mensajes, uno
   por turno:

       Dame tres formas de comenzar.
       Desarrolla la segunda.
       Propón cinco preguntas para el público.
       Convierte la estructura en un pequeño guion.

3. **Recuperar el problema anterior.** Volvemos sobre la compra:

       Volvamos a la laptop. ¿Cuál era mi presupuesto, qué requisitos
       establecimos y cuál fue la recomendación final?

4. **Observar.** Comparamos la respuesta con lo que anotamos aparte: qué requisitos
   devuelve completos, cuáles resume, cuáles omite y si el modelo recomendado
   coincide.
5. **Repetir.** Hacemos la misma prueba en un chat que arrastre una conversación
   bastante más larga, y comparamos cuánto se recupera esta vez.

> El asistente no guarda un expediente: relee la conversación entera cada vez.
> Cuanto más la llenamos de asuntos ajenos, más lejos queda lo que veníamos a
> buscar.

## E. Conceptos

- **Contexto conversacional:** información acumulada que permite interpretar y continuar una conversación.
- **Continuidad:** retomar un problema apoyándose en la información construida antes.
- **Ventana de contexto:** cantidad de información que el modelo considera en una interacción.
- **Encapsulamiento:** mantener dentro de un mismo espacio de conversación lo que pertenece a un solo problema.
- **Chat como expediente:** conversación dedicada a conservar el desarrollo, las decisiones y los resultados de un asunto.

## F. Comprobación

Un compañero sostiene que da lo mismo mezclar asuntos en un chat, porque el
asistente conserva todo lo escrito y siempre puede recuperarlo si se lo pedimos.
¿Dónde se rompe esa confianza?

- a) En el orden de los mensajes, ya que el asistente pondera más los primeros turnos de la conversación y los requisitos recientes pierden peso frente a los iniciales.
- b) En el cambio de tema, porque al pasar a la exposición el asistente descarta el contexto anterior y arranca un razonamiento independiente del previo.
- c) En la sesión, dado que el contexto solo se conserva mientras la pestaña permanece abierta y se pierde al cerrar la aplicación y volver días después.
- d) En que la ventana de contexto tiene un límite.
