---
titulo: IA local con LM Studio
modulo: Caso 052
area: IA Local
---

## Herramientas

> LM Studio  
> Artificial Analysis — comparación de modelos

## Premisa

Instalar y ejecutar un modelo de inteligencia artificial directamente en el equipo utilizando **LM Studio**, seleccionando un modelo adecuado según la RAM y VRAM disponibles.

## Paso 1 — Instalar LM Studio

1. Descargar LM Studio para Windows, macOS o Linux.
2. Instalar y abrir la aplicación.
3. Identificar los recursos disponibles del equipo:
   - RAM del sistema;
   - VRAM de la tarjeta gráfica, si dispone de GPU dedicada.

LM Studio permite descargar y ejecutar modelos locales desde su propia interfaz. :contentReference[oaicite:0]{index=0}

:contentReference[oaicite:1]{index=1}

---

## Paso 2 — Buscar modelos

1. Abrir **Discover**.
2. Buscar un modelo por nombre o familia.
3. Revisar:
   - tamaño;
   - cuantización;
   - compatibilidad con el equipo;
   - propósito del modelo.

LM Studio permite buscar modelos compatibles y ofrece distintas cuantizaciones; como punto de partida, una variante de **4 bits** suele ofrecer un buen equilibrio entre tamaño y calidad. :contentReference[oaicite:2]{index=2}

---

## Paso 3 — Seleccionar según el equipo

Como regla práctica:

| Recursos | Orientación |
|---|---|
| Equipo sin GPU dedicada | Preferir modelos pequeños cuantizados que entren cómodamente en RAM |
| 8 GB RAM | Modelos pequeños |
| 16 GB RAM | Modelos pequeños o medianos cuantizados |
| 8 GB VRAM | Modelos pequeños con aceleración GPU |
| 16 GB VRAM o más | Mayor margen para modelos y contexto |

> Evitar utilizar toda la RAM o VRAM disponible. El modelo necesita memoria adicional durante su ejecución.

El tamaño del archivo del modelo **no es el único consumo de memoria**: también influyen el contexto y la configuración de carga.

Para comparar capacidad y calidad de distintos modelos:

:contentReference[oaicite:3]{index=3}

---

## Paso 4 — Descargar

1. Seleccionar el modelo.
2. Elegir una cuantización compatible con el equipo.
3. Presionar **Download**.
4. Esperar a que finalice la descarga.

---

## Paso 5 — Ejecutar el modelo

1. Abrir **Chat**.
2. Seleccionar **Select Model**.
3. Elegir el modelo descargado.
4. Cargarlo en memoria.
5. Escribir una consulta de prueba.

```text
Explica qué es la inteligencia artificial generativa utilizando un ejemplo sencillo aplicado a una empresa.
````

## Prueba adicional

Comprobar que el modelo funciona de manera local desconectando temporalmente Internet después de haber descargado los archivos necesarios.

LM Studio permite utilizar modelos descargados y conversar con ellos localmente; también permite trabajar con documentos de forma local. ([LM Studio][1])


[1]: https://lmstudio.ai/docs/app?utm_source=chatgpt.com "Welcome to LM Studio Docs! | LM Studio"
