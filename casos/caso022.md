---
titulo: Dashboard con datos externos
modulo: Caso 022
area: General
---

## Herramientas

> [ChatGPT](https://chatgpt.com/)
>
> [Claude](https://claude.ai/)
>
> [Gemini](https://gemini.google.com/)

## Recurso

> Archivo: `002-C-ventas_ultimos_3m.xlsx`

## Acción

1. Proporcionar al asistente solo una muestra de la estructura de los datos:

```text
Fecha: 2025-05-11
Producto: Cámara DSLR
Cantidad: 9
Precio Unitario: 978.75
Total: 8808.75
Canal: Venta telefónica
Pago: PayPal
Región: Centro
````

2. Enviar:

```text
Construye un dashboard HTML compatible con esta estructura.

Los datos reales serán cargados posteriormente desde un archivo externo.

Incluye:
- indicadores principales;
- gráficos;
- filtros;
- tabla;
- mecanismo para cargar el archivo de datos.

Genera todo en un único archivo HTML con CSS y JavaScript integrados.
```

3. Guardar el resultado como:

```text
dashboard_ventas.html
```

4. Abrir el dashboard y cargar `002-C-ventas_ultimos_3m.xlsx`.

5. Verificar que interprete correctamente fechas, montos, productos, canales, métodos de pago y regiones.

6. Agregar nuevos registros al Excel y volver a cargarlo sin modificar el HTML.

7. Probar qué ocurre si cambia el nombre o la estructura de alguna columna.
