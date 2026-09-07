---
titulo: Sistema contextual para generación de proformas
modulo: Caso 045
area: Automatización
---

## Herramientas

> [ChatGPT](https://chatgpt.com/)
>
> [Claude](https://claude.ai/)

## Premisa

La empresa **DemoPeru SAC** necesita automatizar la generación de proformas desde el área administrativa con la menor intervención posible.

La solución será un **sistema contextual** implementado mediante un proyecto de ChatGPT o Claude, compuesto por instrucciones y archivos de referencia permanentes.

---

## Prompt — Planificación del sistema contextual

```text
Necesito crear un sistema contextual para utilizarlo dentro de ChatGPT Projects o Claude Projects en su versión web.

El sistema estará orientado a generar automáticamente proformas para DemoPeru SAC.

Quiero que diseñes la estructura mínima de archivos necesaria para que el proyecto pueda funcionar de manera consistente.

Todos los archivos deben:

- ser independientes;
- estar ubicados en la carpeta raíz;
- no depender de carpetas anidadas;
- poder cargarse directamente como fuentes del proyecto;
- tener una función clara dentro del sistema;
- evitar información duplicada.

El sistema debe activarse cuando el usuario escriba:

"Inicia"

A partir de ese momento debe actuar contextualmente sin requerir que el usuario conozca prompts o instrucciones adicionales.

Debe solicitar únicamente la información necesaria y evitar realizar demasiadas preguntas. Siempre que sea posible, agrupa las preguntas en una sola interacción.

Flujo esperado:

1. Usuario escribe "Inicia".
2. Solicitar:
   - nombre o razón social del receptor;
   - DNI o RUC;
   - teléfono;
   - dirección;
   - servicios;
   - monto;
   - descuento, si corresponde.
3. Validar la información.
4. Calcular subtotal, descuento, IGV 18 % y total.
5. Generar una proforma final.

Salida requerida:

Documento HTML/CSS autocontenido, profesional, imprimible en A4 y preparado para exportarse a PDF.

Contexto de la empresa:

Empresa: DemoPeru SAC
RUC: 123456789
Dirección: Av. Ejemplo 123
IGV: 18 %

El sistema debe contar con una plantilla de salida que permita mantener siempre la misma estructura visual de la proforma.

Planifica la cantidad mínima de archivos necesaria.

Para cada archivo indica:

- nombre;
- función;
- contenido que debe almacenar;
- relación con los demás archivos.

Diferencia entre:

1. archivos que pueden generarse completamente;
2. archivos que contienen información que posteriormente debería revisar o editar manualmente.

Prioriza simplicidad, mantenimiento fácil y uso inmediato dentro de ChatGPT Projects o Claude Projects.
````

---

## Continuación — Generación de los archivos

Después de aprobar la estructura propuesta, utilizar:

```text
Genera ahora todos los documentos propuestos.

Entrega cada archivo completo en formato TXT para poder copiarlo directamente al proyecto.

Los documentos deben estar preparados para uso inmediato por un agente de IA.

Cuando algún dato requiera mi revisión, utiliza información provisional coherente y marca claramente qué dato debo verificar posteriormente.

No dejes secciones incompletas.

Genera primero el archivo principal de instrucciones del sistema y posteriormente los demás archivos en el orden recomendado.
```

---

## Implementación

1. Crear un nuevo proyecto en **ChatGPT Projects** o **Claude Projects**.
2. Si la plataforma dispone de un campo de instrucciones, colocar allí las instrucciones principales.
3. Cargar los demás documentos del sistema como fuentes del proyecto.
4. Mantener todos los archivos independientes y sin carpetas anidadas.
5. Abrir una nueva conversación dentro del proyecto.
6. Escribir:

```text
Inicia
```

7. Proporcionar los datos solicitados.
8. Verificar que el sistema genere la proforma HTML final siguiendo la plantilla definida.
