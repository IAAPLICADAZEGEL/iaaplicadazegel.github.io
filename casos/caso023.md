---
titulo: Dashboard conectado a datos remotos
modulo: Caso 023
area: General
---

## Herramientas

> [ChatGPT](https://chatgpt.com/)
>
> [Claude](https://claude.ai/)
>
> [Gemini](https://gemini.google.com/)
>
> [Google Sheets](https://sheets.google.com/)

## Acción

1. Subir los datos de práctica a Google Sheets, conservando los mismos nombres de columna.

2. Obtener una fuente accesible en formato CSV o JSON.

3. Enviar al asistente:

```text
Adapta este dashboard para que recupere los registros desde la siguiente fuente remota en lugar de leer un archivo local.

Fuente:
[PEGAR URL CSV O JSON]

Mantén:
- los mismos indicadores;
- gráficos;
- filtros;
- tabla;
- estructura visual.

Utiliza fetch para cargar los datos.
````

4. Guardar el HTML actualizado y abrirlo en el navegador.

5. Agregar un nuevo registro en Google Sheets y recargar el dashboard para comprobar que se actualiza.

6. Probar qué ocurre si:

* no hay conexión a Internet;
* cambia la estructura de la hoja;
* la fuente deja de ser accesible.

7. Comparar las tres variantes:

```text
Datos incrustados en HTML
Datos en archivo externo
Datos desde fuente remota
```
