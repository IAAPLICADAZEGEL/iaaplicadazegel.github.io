---
titulo: Sistema contextual para generar infografías de ZELIMAR
modulo: Caso 046
area: Automatización
---

## Herramientas

> [ChatGPT](https://chatgpt.com/)
>
> [Claude](https://claude.ai/)

## Recursos

> [ZELIMAR — Ficha base](https://drive.google.com/file/d/1Ej-imT4Bmxi7jOpQAC47OR25wiq5joA9/view?usp=sharing)
>
> [ZELIMAR — Logotipo](https://drive.google.com/file/d/1SfQDuf_ApxdPW1ScJUMW3v1PxJGgznaT/view?usp=sharing)

## Premisa

ZELIMAR necesita un **sistema contextual** en ChatGPT Projects o Claude Projects para generar **únicamente imágenes del tipo infografía** para redes sociales, usando como base la ficha de información de la empresa y su logotipo.

Todos los archivos del sistema estarán en la **raíz del proyecto**, sin carpetas adicionales.

---

## Prompt — Planificador del sistema contextual

```text
Necesito crear un sistema contextual para usarlo dentro de ChatGPT Projects o Claude Projects en versión web.

El objetivo del sistema es generar únicamente imágenes del tipo infografía para redes sociales de la empresa ZELIMAR.

Fuentes base del sistema:
- una ficha de información de la empresa llamada "ZELIMAR ficha base";
- el logotipo oficial de ZELIMAR.

Quiero que el sistema funcione con la menor complejidad posible.

Condiciones del sistema:
- todos los archivos estarán en la raíz;
- no se usarán carpetas;
- los archivos deben ser independientes;
- deben poder cargarse directamente como sources del proyecto;
- el sistema debe mantenerse coherente con la empresa en cada generación;
- el sistema debe generar solo imágenes, no documentos largos ni piezas fuera del ámbito visual.

Flujo esperado:
1. El usuario escribe "Inicia".
2. El sistema responde preguntando qué desea generar hoy y puede sugerir recomendaciones de temporada o campaña para la empresa.
3. Si el usuario pide ideas, el sistema propone 10 ideas de infografías.
4. El usuario selecciona una idea.
5. El sistema pregunta para qué plataforma será la publicación.
6. El sistema pregunta o confirma el formato visual adecuado, por ejemplo 1:1, 4:5 o 9:16 según la plataforma.
7. El sistema genera la propuesta final como imagen infográfica profesional.

La imagen debe:
- usar la identidad visual de ZELIMAR;
- respetar el logotipo;
- aprovechar la información de la ficha base;
- tener estructura de infografía;
- verse profesional y lista para redes sociales.

Necesito que planifiques la cantidad mínima de archivos necesaria para este sistema.

Para cada archivo indica:
- nombre;
- función;
- contenido;
- si puede generarse completo o si requiere revisión posterior.

Prioriza simplicidad, uso inmediato y coherencia visual.
````

---

## Continuación — Generación de los archivos del sistema

```text
Genera ahora todos los documentos del sistema contextual.

Entrégalos completos en formato TXT, listos para copiar y usar de inmediato dentro de un proyecto de ChatGPT o Claude.

Todos los archivos deben estar pensados para permanecer en la raíz del proyecto.

No dejes secciones incompletas.

Si algún contenido requiere revisión posterior, simúlalo de forma coherente y marca claramente qué parte conviene verificar.

Genera primero el archivo principal de instrucciones del sistema y luego los demás archivos en el orden recomendado.
```

---

## Flujo de uso del sistema

1. Crear un nuevo proyecto en **ChatGPT Projects** o **Claude Projects**.
2. Colocar las instrucciones principales si la plataforma lo permite.
3. Cargar todos los archivos del sistema contextual en la raíz del proyecto.
4. Iniciar una nueva tarea escribiendo:

```text
Inicia
```

5. El sistema preguntará qué se desea generar hoy.
6. Si hace falta, propondrá ideas de infografías.
7. El usuario seleccionará una idea.
8. El sistema pedirá la plataforma y el formato.
9. El sistema generará la imagen infográfica final.
