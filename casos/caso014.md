---
titulo: El contexto puede vivir fuera del prompt
modulo: Caso 014
area: General
resumen: Cómo separar lo que cambia en cada tarea de lo que se repite siempre, y convertir esto último en archivos que se combinan según el trabajo.
---

## A. Situación

Llevamos la comunicación digital de un pequeño emprendimiento: posts, guiones de
video, textos para flyers, descripciones de servicios. Cada pedido a la IA empieza
igual, reescribiendo quiénes somos, qué ofrecemos, a quién le hablamos, con qué
tono y con qué colores. La tarea cambia cada vez; ese preámbulo, casi nunca. Hoy
hay que producir tres piezas y ya estamos copiando el mismo párrafo por tercera
vez.

## B. Objetivo

Reconocer que la información estable de un trabajo puede alojarse fuera del
prompt, en archivos que se seleccionan según la tarea.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- Un editor de texto plano y una carpeta llamada `contexto/`.
- La información real del emprendimiento: datos, servicios, ejemplos de piezas ya aprobadas.

## D. Desarrollo

Recorremos el ciclo **contexto reutilizable + instrucción específica → resultado**.

1. **Extraer.** Separamos lo estable en cinco archivos pequeños, uno por función:

       contexto/
       ├── DATOS_empresa.md      quiénes somos, público, ubicación, contacto
       ├── SERVICIOS_empresa.md  servicios, características, beneficios, condiciones
       ├── ESTILO_escritura.md   tono, vocabulario, estructura, criterios de redacción
       ├── GUIA_visual.md        colores, tipografías, composición, uso de imágenes
       └── CASOS_material.md     piezas anteriores aprobadas y situaciones frecuentes

2. **Prompt con todo dentro.** Como referencia, armamos primero el pedido
   tradicional: un solo mensaje con empresa, servicios, público, estilo, criterios
   y tarea, todo junto.
3. **Prompt con el contexto fuera.** En un chat nuevo adjuntamos
   `DATOS_empresa.md`, `SERVICIOS_empresa.md` y `ESTILO_escritura.md`, y
   escribimos únicamente:

       Utiliza los archivos proporcionados como contexto. Crea un post para
       Instagram sobre el servicio de evaluación inicial.

4. **Componer según la tarea.** Repetimos cambiando la combinación de archivos:

       SERVICIOS + ESTILO + CASOS → Escribe un guion de 30 segundos
       explicando este servicio.

       DATOS + SERVICIOS + GUIA_visual → Diseña una pieza promocional 1:1
       para este servicio.

5. **Comparar.** Ponemos los dos caminos lado a lado: largo de la instrucción,
   qué cuesta modificar el tono en cada uno, si las tres piezas suenan a la misma
   empresa, y qué queda disponible para la próxima semana.
6. **Mantener.** Cambiamos una sola cosa —el tono en `ESTILO_escritura.md`— y
   volvemos a generar las tres piezas.

> Ese cambio de tono se escribió una vez y alcanzó a las tres piezas. En el prompt
> gigante habría habido que encontrarlo y corregirlo tres veces, con tres
> resultados posibles.

## E. Conceptos

- **Contexto estable:** información que cambia lentamente y sirve a muchas tareas.
- **Instrucción variable:** lo que necesitamos producir ahora.
- **Contexto seleccionado:** conjunto de archivos elegidos para una tarea concreta.
- **Contexto componible:** módulos que se combinan de distinta manera según el trabajo.
- **Consistencia:** que piezas distintas mantengan la misma voz y los mismos criterios.

## F. Comprobación

Un compañero propone juntar los cinco archivos en un único `EMPRESA.md` y
adjuntarlo siempre, para no tener que decidir nada antes de cada pedido. ¿Qué se
pierde en el camino?

- a) La claridad del mantenimiento, porque al corregir el tono habría que localizarlo dentro de un archivo extenso donde conviven datos, servicios y criterios gráficos.
- b) La economía de la ventana de contexto, dado que adjuntar siempre el archivo completo consume espacio con información que esa tarea concreta no llegará a utilizar.
- c) La posibilidad de elegir qué contexto pesa en cada tarea.
- d) La trazabilidad del material aprobado, ya que los ejemplos de piezas anteriores quedarían mezclados con las condiciones comerciales de los servicios.
