---
titulo: Sistema WEB Proforma 
modulo: Caso 030
area: General
---

## Prompt

> Archivo usados:
> 
> [INFO EMPRESA](https://drive.google.com/file/d/1Ej-imT4Bmxi7jOpQAC47OR25wiq5joA9/view?usp=sharing)
> 
> [Logo](https://drive.google.com/file/d/1SfQDuf_ApxdPW1ScJUMW3v1PxJGgznaT/view?usp=sharing)
> 
> [Referencia](https://drive.google.com/file/d/14DeC0pQsIobdKwCzDqg-CFDrH05cKpfe/view?usp=sharing)


> Subir la imagen, y obtener el enlace
> Servicio 1: [IMGBB](https://imgbb.com/)
> Servicio 2: [Thumbsnab](https://thumbsnap.com/)
> Servicio 3: [IMGUR](https://imgur.com/)

 
```markdown
# Generador de proformas ZELIMAR

## Fuente de datos
Adjunto la **ficha base institucional de ZELIMAR S.A.C.** Es la única fuente para:
- Datos del emisor (razón social, RUC, dirección, contactos, cuentas bancarias)
- Portafolio de servicios con códigos y unidades
- Condiciones comerciales estándar
- Identidad visual: paleta, tipografía, logotipo y tono

## Objetivo
Construye una aplicación monolítica en **un solo archivo index.html autocontenido**,  un generador de proformas exportables a **PDF A4** 
## Flujo
- Formulario a la izquierda: emisor precargado desde la ficha y editable, cliente, ítems, condiciones.
- Vista previa del documento a la derecha, actualizada en tiempo real.
- En móvil, la vista previa se ubica debajo del formulario.

## Tabla de ítems
Columnas: `código` · `descripción` · `unidad` · `cantidad` · `precio unitario` · `descuento %` · `subtotal`.

- Botones para añadir y eliminar filas, conservando siempre al menos una.
- El campo código ofrece los servicios de la ficha y autocompleta descripción y unidad.

## Reglas de cálculo (Perú)
- Subtotal por fila = `cantidad × precio × (1 − descuento/100)`
- Secuencia: valor de venta → **IGV 18 %** → total
- Interruptor **"los precios incluyen IGV"**: activo, desagrega; inactivo, suma
- Detracción según el porcentaje y las condiciones de la ficha, mostrada junto al neto a pagar cuando corresponda
- Importe en letras, formato `es-PE`, dos decimales, moneda `S/` o `US$`

## Documento generado
Hoja A4 vertical que incluye:
1. Encabezado institucional con logotipo
2. Número de proforma `COT-AAAA-0001` editable y fecha automática `DD/MM/AAAA`
3. Bloque de datos del cliente
4. Tabla de ítems
5. Totales destacados e importe en letras
6. Condiciones comerciales, datos bancarios y nota de detracción
7. Espacio de firma y pie con el lema

## Validaciones
- Obligatorios: razón social del cliente y al menos un ítem completo
- Cantidad y precio: números positivos
- Descuento: rango 0–100
- RUC: 11 dígitos cuando se completa

## Acciones
`Generar PDF A4` · `Copiar al portapapeles` · `Limpiar formulario`
```
