---
titulo: El resumen debe cumplir condiciones
modulo: Caso 005
area: General
resumen: Cómo una lista de características convierte la respuesta en algo que podemos verificar punto por punto.
---

## A. Situación

Ya revisamos el informe del BCRP y ahora debemos preparar una síntesis para
circularla internamente. Sabemos de antemano cómo tiene que ser: corta, con las
cifras intactas y con conclusiones al final. Lo que no sabemos es cómo lograr que
salga así a la primera.

## B. Objetivo

Distinguir cómo una lista de características previamente definidas convierte la
respuesta de un asistente en un resultado verificable.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El [informe del BCRP en PDF](https://www.bcrp.gob.pe/docs/Publicaciones/Notas-Estudios/2026/nota-de-estudios-27-2026.pdf).
- Una hoja o documento aparte para marcar el cumplimiento de cada característica.

## D. Desarrollo

Recorremos el ciclo **resultado → características → IA → resultado controlado**.

1. **Resultado.** Definimos el producto: una síntesis interna del informe.
2. **Características.** Enumeramos las condiciones que debe cumplir, una por
   línea, sin mezclar dos en la misma.
3. **Pedido.** Apilamos el resultado y su lista y escribimos:

       Resume este informe con las siguientes características:
       - Máximo 300 palabras.
       - Identifica los principales resultados.
       - Conserva las cifras y porcentajes relevantes.
       - Separa actividad económica y empleo.
       - Utiliza lenguaje ejecutivo y claro.
       - Finaliza con tres conclusiones.

4. **Comprobación.** Leemos la respuesta como quien revisa una lista: contamos
   las palabras, buscamos las cifras, verificamos la separación de bloques y las
   tres conclusiones.
5. **Ajuste.** Si alguna característica no se cumplió, la señalamos y volvemos a
   pedir solo esa.

> La lista sirve dos veces: primero para pedir y después para revisar. Sin ella,
> «quedó bien» es lo único que podríamos decir del resultado.

## E. Conceptos

- **Característica:** condición concreta que debe cumplir el resultado.
- **Apilado de características:** construcción del pedido mediante una lista acumulativa de requisitos.
- **Control del resultado:** evaluación de la salida contra condiciones definidas antes de pedirla.
- **Lenguaje ejecutivo:** redacción breve y directa, orientada a la decisión.

## F. Comprobación

Alguien del equipo propone reemplazar las seis características por la frase «hazlo
bien y profesional» para ahorrar tiempo al escribir. ¿Qué se pierde en el camino?

- a) La precisión del vocabulario, porque «profesional» significa cosas distintas según el sector y el asistente elige entonces un registro promedio.
- b) El control de la extensión, que es la única característica que un asistente no puede inferir por sí solo a partir del documento adjunto.
- c) La posibilidad de reutilizar el pedido en otros informes, ya que una frase general obliga a reescribirlo por completo cada vez.
- d) La lista contra la cual revisar la respuesta.
