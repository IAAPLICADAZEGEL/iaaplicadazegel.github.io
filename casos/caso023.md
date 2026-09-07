---
titulo: Dashboard con datos en tiempo real desde Google Sheets
modulo: Caso 023
area: General
---

## Herramientas

> [Google Sheets](https://sheets.google.com/)
>
> [ChatGPT](https://chatgpt.com/)
>
> [Claude](https://claude.ai/)
>
> [Gemini](https://gemini.google.com/)

## Recurso

> [Archivo de ventas de referencia](https://docs.google.com/spreadsheets/d/1Y46UmZxP-1W2NKbJONhmLI2W-ni7Zex0/edit?usp=sharing&ouid=114704156722391767374&rtpof=true&sd=true)

## Acción

1. Subir el archivo Excel a Google Drive.
2. Abrirlo con Google Sheets.
3. Revisar los datos:
   - encabezados sin espacios innecesarios;
   - valores numéricos correctamente formateados;
   - sin columnas vacías.

4. En Google Sheets ir a:

```text
Archivo → Compartir → Publicar en la web
````

5. Seleccionar la hoja correspondiente y publicarla como **CSV**.

6. Copiar la URL CSV generada.

7. Enviar al asistente:

```text
Genera un dashboard descriptivo e interactivo en un único archivo HTML.

Fuente de datos:
[PEGAR URL CSV DE GOOGLE SHEETS]

Requisitos:

- carga los datos automáticamente con fetch();
- utiliza un proxy CORS cuando sea necesario;
- valida la estructura básica del CSV;
- incluye un conjunto de datos de respaldo si la carga falla;
- utiliza Chart.js para los gráficos;
- incluye indicadores y gráficos relevantes para analizar las ventas;
- diseño profesional y responsivo;
- muestra un mensaje si los datos no pueden cargarse.

Todo debe funcionar desde un único archivo HTML, sin backend.
```

8. Guardar el resultado como:

```text
dashboard_ventas.html
```

9. Abrirlo en el navegador.

10. Modificar un registro en Google Sheets, recargar el dashboard y comprobar que la información se actualiza.
