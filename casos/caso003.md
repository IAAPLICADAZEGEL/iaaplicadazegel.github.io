---
titulo: Necesito entenderlo ahora
modulo: Caso 003
area: General
resumen: Qué devuelve un asistente cuando le pedimos un resumen sin decirle nada más.
---

## A. Situación

Un colega deja caer en el chat del equipo la *Nota de Estudios 27-2026* del Banco
Central de Reserva del Perú: cuarenta páginas sobre PBI, actividad sectorial y
empleo. La reunión empieza en diez minutos y el documento sigue cerrado.

## B. Objetivo

Comprender qué información selecciona un asistente de IA cuando recibe un pedido
breve y abierto sobre un documento extenso.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El [informe del BCRP en PDF](https://www.bcrp.gob.pe/docs/Publicaciones/Notas-Estudios/2026/nota-de-estudios-27-2026.pdf).
- Navegador web o aplicación móvil.

## D. Desarrollo

Recorremos el ciclo **documento → pedido directo → IA → resumen**.

1. **Documento.** Descargamos el PDF del BCRP y lo adjuntamos al asistente.
2. **Pedido.** Nombramos la necesidad tal como se la diríamos a un colega, sin
   añadir condiciones ni explicar para qué la queremos.
3. **Envío.** Escribimos exactamente:

       Resume este documento.

4. **Resumen.** Leemos lo que devuelve y anotamos qué puso primero: ¿el
   crecimiento del PBI de 3,7 %?, ¿el empleo?, ¿la estructura del informe?
5. **Contraste.** Nos preguntamos si con eso podríamos entrar a la reunión.

> El asistente decidió por nosotros qué era lo importante. No le dimos ningún
> criterio, así que aplicó el suyo: lo que el documento repite y destaca.

## E. Conceptos

- **Sentido común:** expresar directamente aquello que necesitamos, en lenguaje cotidiano.
- **Pedido directo:** instrucción sin condiciones, contexto ni formato especificado.
- **Resumen:** reducción de un contenido que conserva sus ideas relevantes.
- **Criterio de relevancia:** regla —explícita o no— que determina qué entra en el resumen.

## F. Comprobación

Alguien del equipo concluye que, como el resumen salió correcto, el pedido breve
sirve igual de bien para cualquier documento. ¿Qué le respondemos?

- a) Que los pedidos breves fallan siempre que el documento supera cierta extensión y conviene por eso fragmentarlo antes de adjuntarlo.
- b) Que el problema está en el formato PDF, porque el asistente lee mejor un texto pegado directamente en la conversación.
- c) Que salió correcto porque el asistente eligió el criterio, no nosotros.
- d) Que el resultado depende del asistente elegido, de modo que habría que repetir la prueba en las tres plataformas antes de concluir algo.
