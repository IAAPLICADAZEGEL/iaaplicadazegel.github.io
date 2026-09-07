---
titulo: Prompt reutilizable en Markdown
modulo: Caso 011
area: General
---

## Herramientas

> [ChatGPT](https://chatgpt.com/)
>
> [Claude](https://claude.ai/)
>
> [Gemini](https://gemini.google.com/)

## Acción

1. Tomar un prompt que ya haya funcionado en un chat.
2. Convertirlo en un archivo Markdown estructurado.

```markdown
# Informe de sesión

## Rol

Actúa como asistente académico.

## Objetivo

Convierte la transcripción proporcionada en un informe de la sesión.

## Salida

Incluye:

- temas trabajados;
- conceptos principales;
- actividades realizadas;
- ejemplos desarrollados;
- herramientas mencionadas;
- conclusiones.

## Advertencias

- Utiliza únicamente información presente en la transcripción.
- Distingue contenido académico de indicaciones administrativas.
- Conserva nombres y términos técnicos relevantes.

## Contexto

La transcripción corresponde a una sesión del curso Inteligencia Artificial Aplicada.
El informe servirá como registro académico.
````

3. Guardar el archivo como:

```text
informe_sesion.md
```

4. En una conversación nueva, adjuntar el archivo junto con otra transcripción.
5. Enviar:

```text
Aplica las instrucciones de informe_sesion.md a la transcripción adjunta.
```

6. Cuando necesites cambiar el comportamiento, editar únicamente el archivo `.md` y volver a utilizarlo.
