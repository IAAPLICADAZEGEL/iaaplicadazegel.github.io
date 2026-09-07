---
titulo: Registro de finanzas personales con Python
modulo: Caso 050
area: Automatización
---

## Herramientas

> [Python](https://www.python.org/)
>
> [Thonny](https://thonny.org/)

## Premisa

Crear una aplicación de escritorio simple para registrar ingresos y egresos personales, almacenando la información en Excel e incorporando respaldo automático y registro de errores.

## Prompt

```text
Genera un sistema de escritorio simple, práctico y minimalista para registrar finanzas personales.

Debe estar desarrollado en Python y ejecutarse directamente desde Thonny. Sin hacer ningun cambio yo como usuario.

Entrega todo el sistema en un único archivo .py monolítico.

La aplicación debe permitir registrar:

- Tipo de movimiento: Ingreso / Egreso
- Descripción
- Monto
- Fecha

FUNCIONALIDAD:

- interfaz gráfica de escritorio con Tkinter;
- formulario sencillo y fácil de usar;
- botón para registrar movimientos;
- mostrar los movimientos registrados;
- calcular total de ingresos, egresos y saldo;
- validar campos obligatorios;
- validar que el monto sea numérico y positivo;
- guardar automáticamente los registros en un archivo Excel;
- crear el archivo Excel si todavía no existe;
- utilizar openpyxl para trabajar con Excel;
- generar copias de seguridad automáticas del archivo de datos;
- mantener un archivo de log para registrar errores y eventos importantes;
- mostrar mensajes comprensibles cuando ocurra un error;
- evitar pérdida de información ante errores comunes.

ARCHIVOS GENERADOS:

- finanzas.xlsx
- archivo de log de errores
- copias de seguridad del archivo Excel

El programa debe crear automáticamente los archivos o directorios necesarios.

DISEÑO:

- aplicación de escritorio limpia;
- distribución ordenada;
- botones claramente identificados;
- interfaz adecuada para un usuario sin conocimientos técnicos.

CÓDIGO:

- todo el código debe estar contenido en un solo archivo Python;
- utiliza funciones claras y organizadas;
- incluye comentarios únicamente donde sean útiles;
- utiliza principalmente librerías estándar de Python;
- limita las dependencias externas a las estrictamente necesarias;
- el código debe poder copiarse directamente en Thonny y ejecutarse.

Al finalizar tu respuesta incluye:

1. código Python completo;
2. librerías necesarias;
3. instrucciones para instalarlas desde Thonny;
4. pasos para ejecutar el sistema;
5. explicación breve de dónde se guardan el Excel, los backups y los logs.

No entregues fragmentos de código.
Devuelve una versión completa lista para ejecutar.
````

## Implementación

1. Descargar e instalar [Thonny](https://thonny.org/).
2. Abrir Thonny.
3. Ir a **Herramientas → Gestionar paquetes**.
4. Buscar e instalar:

```text
openpyxl
```

5. Crear un archivo nuevo.
6. Pegar el código generado.
7. Guardarlo como:

```text
finanzas.py
```

8. Presionar **Ejecutar**.
9. Registrar un ingreso y un egreso de prueba.
10. Verificar la creación del archivo Excel, el log y las copias de seguridad.

## En caso de error

Copiar el mensaje de error completo y enviarlo en el mismo chat:

```text
Analiza el siguiente error de mi aplicación Python ejecutada en Thonny:

[PEGAR ERROR]

Corrige el problema y genera nuevamente todo el archivo Python completo.

No entregues parches ni fragmentos.

Conserva:
- interfaz de escritorio;
- almacenamiento en Excel;
- sistema de backups;
- logs de errores;
- funcionamiento original.

Devuelve el código completo listo para reemplazar el anterior.
```
