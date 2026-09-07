---
titulo: Análisis reproducible con Python
modulo: Caso 025
area: General
---

## Herramientas

> [ChatGPT](https://chatgpt.com/)
>
> [Claude](https://claude.ai/)
>
> [Gemini](https://gemini.google.com/)
>
> [Google Colab](https://colab.research.google.com/)

## Recurso

> Utilizar uno de estos archivos:
>
> `002-A-gastos_ejecutivos.xlsx`  
> `002-B-gastos_personales.xlsx`  
> `002-C-ventas_ultimos_3m.xlsx`

## Acción

1. Adjuntar el archivo de datos.
2. Solicitar el procedimiento en código:

```text
Genera el código Python necesario para reproducir este análisis.

El código debe:

- cargar el archivo Excel;
- identificar y limpiar los datos necesarios;
- calcular las principales métricas descriptivas;
- generar gráficos relevantes;
- mostrar los resultados de forma clara.

Utiliza pandas y matplotlib.

Entrega código completo, organizado y listo para ejecutar en Google Colab.
````

3. Abrir [Google Colab](https://colab.research.google.com/).
4. Subir el archivo y ejecutar el código generado.
5. Si aparece un error, copiarlo al asistente:

```text
Analiza este error y corrige el código completo:

[PEGAR ERROR]
```

6. Modificar posteriormente el análisis, por ejemplo:

```text
Ahora adapta el código para comparar los resultados por mes.
```

7. Sustituir el dataset por uno nuevo con la misma estructura y volver a ejecutar el mismo código para comprobar que el análisis es reproducible.
