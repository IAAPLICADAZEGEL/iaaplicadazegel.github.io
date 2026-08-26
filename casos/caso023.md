---
titulo: Del archivo al dato vivo
modulo: Caso 023
area: General
resumen: Qué se gana y de qué se empieza a depender cuando la visualización consulta una fuente remota en lugar de un archivo local.
---

## A. Situación

El dashboard de ventas funciona, pero cada vez que el equipo comercial actualiza
sus registros hay que sustituir el archivo a mano. El equipo, además, ya no trabaja
con un Excel en un escritorio: mantiene una hoja compartida que cambia varias veces
al día. La visualización va siempre un paso atrás de los datos.

## B. Objetivo

Reconocer qué cambia cuando una aplicación deja de contener sus datos y pasa a
consultarlos desde una fuente remota.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- Una cuenta de Google y una hoja de cálculo destinada al ejercicio.
- Los datos de práctica con la estructura de `002-C-ventas_ultimos_3m.xlsx`.
- Un dashboard HTML ya construido sobre esa estructura, y un navegador.

## D. Desarrollo

Recorremos el ciclo **hoja compartida → fuente accesible → fetch → datos → dashboard**.

1. **Preparar.** Trasladamos los datos de práctica a una hoja de Google Sheets, con
   los mismos nombres de columna que espera el dashboard.
2. **Exponer.** Configuramos la hoja para que sus datos puedan recuperarse desde
   fuera, en un formato de intercambio como CSV o JSON, y guardamos la dirección
   resultante.
3. **Conectar.** Pedimos la modificación del proyecto:

       Adapta este dashboard para que recupere los registros desde la
       siguiente fuente remota en lugar de leer un archivo local. Mantén los
       mismos indicadores, gráficos y filtros.

4. **Probar el circuito.** Agregamos una venta nueva en la hoja, recargamos el
   dashboard y comprobamos si aparece.
5. **Probar la dependencia.** Desconectamos la red, o revocamos el acceso a la
   hoja, y volvemos a abrir el dashboard. Anotamos qué muestra ahora.
6. **Comparar arquitecturas.** Ponemos las tres versiones en una línea: datos
   dentro del HTML, datos en un archivo aparte, datos alojados fuera de la
   aplicación. La visualización es la misma; lo que cambió es dónde viven los
   datos y de qué depende cada una.

> El dashboard dejó de estar desactualizado y empezó a poder estar caído. No
> eliminamos un problema: cambiamos de problema.

## E. Conceptos

- **Fuente remota:** origen de datos situado fuera de la aplicación.
- **`fetch`:** mecanismo web para solicitar recursos alojados en otra ubicación.
- **CSV/JSON:** representaciones habituales para intercambiar datos estructurados.
- **CORS:** política del navegador que regula las solicitudes entre orígenes distintos.
- **Dependencia externa:** componente ajeno del que pasa a depender el funcionamiento.

## F. Comprobación

Un compañero ve que la venta agregada aparece al recargar y concluye que conectar
el dashboard a la hoja compartida lo mejora en todo sentido. ¿Dónde se rompe esa
conclusión?

- a) En que ahora depende de algo que no controlamos.
- b) En la estructura de la hoja, porque cualquiera con acceso puede renombrar una columna o insertar una fila de totales y dejar la visualización sin poder interpretar los datos.
- c) En las restricciones del navegador, dado que las solicitudes entre orígenes distintos están reguladas y no toda fuente remota resulta accesible desde una página local.
- d) En la exposición de la información, ya que publicar la hoja para que el dashboard la consulte amplía quién puede alcanzar esos registros de venta.
