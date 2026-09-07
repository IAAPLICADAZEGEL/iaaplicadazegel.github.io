---
titulo: Registro de finanzas personales con Streamlit
modulo: Caso 051
area: Automatización
---

## Herramientas

> [Python](https://www.python.org/)
>
> [Streamlit](https://streamlit.io/)
>
> [Thonny](https://thonny.org/)

## Premisa

Crear una aplicación web local para registrar ingresos y egresos personales mediante Python y Streamlit, con almacenamiento local y exportación de datos a Excel.

## Prompt

```text
Genera una aplicación web local simple, práctica y minimalista para registrar finanzas personales.

Debe estar desarrollada en Python con Streamlit y ejecutarse localmente desde Thonny o una terminal.

Entrega todo el sistema en un único archivo Python .py.

La aplicación debe permitir registrar:

- Tipo de movimiento: Ingreso / Egreso
- Descripción
- Monto
- Fecha

FUNCIONALIDAD:

- interfaz web con Streamlit;
- formulario para registrar movimientos;
- tabla con los movimientos almacenados;
- cálculo automático de:
  - total de ingresos;
  - total de egresos;
  - saldo disponible;
- validación de campos obligatorios;
- validación de montos positivos;
- almacenamiento persistente local;
- guardar los registros en un archivo Excel;
- crear automáticamente el archivo si no existe;
- permitir descargar o exportar los datos en formato Excel;
- mostrar los movimientos registrados en pantalla;
- permitir filtrar por tipo de movimiento o fecha;
- generar copias de seguridad automáticas;
- mantener un archivo de log para errores y eventos importantes;
- mostrar mensajes claros cuando ocurra algún problema.

ARCHIVOS:

- finanzas.xlsx
- archivo de logs
- carpeta o archivos de backup

El sistema debe crear automáticamente los recursos necesarios.

DISEÑO:

- interfaz limpia y minimalista;
- formulario fácil de utilizar;
- indicadores visibles para ingresos, egresos y saldo;
- tabla ordenada;
- botón para descargar el archivo Excel.

CÓDIGO:

- todo el sistema debe estar contenido en un único archivo Python;
- utiliza Streamlit para la interfaz;
- utiliza pandas y openpyxl para trabajar con los datos y Excel;
- utiliza funciones claras y organizadas;
- evita dependencias innecesarias;
- el código debe estar listo para copiar y ejecutar.

Al finalizar incluye:

1. código Python completo;
2. librerías necesarias;
3. comandos de instalación;
4. pasos para ejecutarlo;
5. explicación breve de dónde se guardan los datos, backups y logs.

No entregues fragmentos de código.
Devuelve una versión completa lista para ejecutar.
````

## Implementación

1. Instalar [Python](https://www.python.org/) y [Thonny](https://thonny.org/).
2. Abrir Thonny.
3. Instalar las librerías necesarias:

```text
streamlit
pandas
openpyxl
```

También pueden instalarse desde terminal:

```bash
pip install streamlit pandas openpyxl
```

4. Crear un archivo:

```text
finanzas_streamlit.py
```

5. Pegar el código generado.
6. Guardar el archivo.
7. Abrir una terminal en la ubicación del archivo.
8. Ejecutar:

```bash
streamlit run finanzas_streamlit.py
```

9. Abrir la dirección local que aparece en pantalla, normalmente:

```text
http://localhost:8501
```

10. Registrar movimientos y probar la exportación a Excel.

## En caso de error

```text
Analiza el siguiente error de mi aplicación Streamlit:

[PEGAR ERROR]

Corrige el problema y genera nuevamente todo el archivo Python completo.

No entregues parches ni fragmentos.

Conserva:
- interfaz web con Streamlit;
- almacenamiento local;
- exportación a Excel;
- backups;
- logs;
- cálculos de ingresos, egresos y saldo.

Devuelve todo el código completo listo para reemplazar el anterior.
```

