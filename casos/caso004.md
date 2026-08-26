---
titulo: Necesito un resumen para mi situación
modulo: Caso 004
area: General
resumen: Cómo cambia una respuesta cuando el pedido dice qué queremos y para qué lo usaremos.
---

## A. Situación

Trabajamos en un área administrativa. La jefatura compartió la *Nota de Estudios
27-2026* del BCRP porque mañana, en la reunión de equipo, se comentará la
situación económica. No se espera que expongamos el informe: se espera que
podamos hablar de él.

## B. Objetivo

Reconocer cómo la respuesta de un asistente se ajusta cuando el pedido incorpora
el resultado esperado y el uso que le daremos.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El [informe del BCRP en PDF](https://www.bcrp.gob.pe/docs/Publicaciones/Notas-Estudios/2026/nota-de-estudios-27-2026.pdf).
- El resumen obtenido en el Caso 0.3, para comparar.

## D. Desarrollo

Recorremos el ciclo **resultado + contexto → IA → respuesta adaptada**.

1. **Resultado.** Precisamos qué queremos obtener: los principales resultados del
   informe, no el informe entero.
2. **Contexto.** Precisamos para qué lo usaremos: explicarlos brevemente en una
   reunión de trabajo.
3. **Pedido.** Juntamos ambos elementos en una sola frase y escribimos:

       Resume los principales resultados de este informe para poder
       explicarlos brevemente durante una reunión de trabajo.

4. **Comparación.** Ponemos esta respuesta al lado de la del Caso 0.3 y marcamos
   las diferencias: qué desapareció, qué apareció, qué cambió de orden.

> Añadimos dos datos y no una instrucción más. El asistente no obedeció mejor:
> supo para quién estaba escribiendo.

## E. Conceptos

- **Resultado:** aquello que esperamos obtener del asistente.
- **Contexto:** información sobre nuestra situación que permite adaptar la respuesta.
- **Prompt adaptativo:** pedido construido como resultado + contexto.
- **Destinatario:** persona o escenario al que sirve la respuesta.

## F. Comprobación

Un compañero sostiene que agregar el contexto solo hace la respuesta más larga,
porque el asistente ya tenía el documento completo. ¿Dónde se rompe ese
razonamiento?

- a) En que el contexto no agrega información: descarta la que sobra.
- b) En que el asistente nunca lee el documento entero, de modo que el contexto funciona en realidad como una instrucción de búsqueda dentro del archivo adjunto.
- c) En que la longitud depende del límite de palabras del plan gratuito y no de lo que escribamos en el pedido junto con el documento.
- d) En que el contexto solo influye cuando se indica además el formato de salida, porque sin formato el asistente vuelve a su estructura por defecto.
