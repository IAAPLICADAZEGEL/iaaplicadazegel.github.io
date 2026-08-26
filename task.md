# IA Aplicada · Zegel

## Tareas pendientes

Tareas manuales que solo realizará el usuario:

* Grabar el video de bienvenida.
* Mejorar todas las áreas de enlaces.

---

# Automatizaciones

## A. Actualizar `content/actual.md`

### Entrada del usuario

El usuario proporcionará una lista con los enlaces de los nuevos videos.

Cada video deberá incluir, cuando corresponda:

* Título.
* Fecha de publicación.
* Enlace de YouTube.

### Proceso

1. Identificar los **3 videos nuevos** proporcionados por el usuario.

2. Estos reemplazarán a los 3 videos actualmente mostrados como recientes en `content/actual.md`.

3. Para cada video nuevo:

   * Usar su nombre correcto.
   * Usar su fecha correspondiente.
   * Mantener el enlace de YouTube **directo y suelto**, sin redirección ni enlace Markdown.

4. Los videos que dejan de formar parte de los 3 más recientes deberán trasladarse a una sección llamada:

   `## Anteriores`

5. Dentro de `Anteriores`, los videos deberán mostrarse en una tabla.

6. En esta tabla, los enlaces sí deberán escribirse como enlaces Markdown.

### Regla importante

Los 3 videos actuales deben mantener el enlace de YouTube directamente en el documento:

```text
https://www.youtube.com/watch?v=...
```

No usar:

```markdown
[Ver video](https://www.youtube.com/watch?v=...)
```

---

## B. Agregar un nuevo grupo de capacitación

### Entrada del usuario

El usuario proporcionará:

* Nombre del grupo, identificado por mes o meses y año.
* Enlace de Google Drive de las anotaciones.
* Enlace de la playlist de YouTube donde estarán las grabaciones.

Ejemplo de nombre:

```text
Agosto–Septiembre 2026
```

### Cambios requeridos

#### `content/anotaciones.md`

Agregar el nuevo grupo al listado de grupos.

El orden deberá ser:

**más reciente → más antiguo**

Cada grupo deberá conservar su enlace correspondiente de Google Drive.

#### `content/grabaciones.md`

Agregar el nuevo grupo con:

* Nombre del grupo.
* Estado: `En curso`.
* Enlace de la playlist de YouTube.

El orden deberá ser:

**más reciente → más antiguo**

---

## C. Cerrar un grupo de capacitación

### Entrada del usuario

El usuario proporcionará el nombre del grupo que desea cerrar.

### Proceso

Buscar el grupo correspondiente en:

```text
content/grabaciones.md
```

Cambiar únicamente su estado:

```text
En curso
```

por:

```text
Cerrado
```

Mantener sin cambios:

* Nombre del grupo.
* Enlace de las grabaciones.
* Posición del grupo dentro del documento.
* Cualquier otro dato asociado.

---

## D. Actualizar el manifiesto de casos

### Objetivo

Sincronizar automáticamente los casos existentes en la carpeta:

```text
casos/
```

con el archivo:

```text
content/manifest.json
```

### Proceso

1. Revisar todos los archivos Markdown de la carpeta `casos/`.
2. Leer el encabezado YAML de cada archivo.
3. Obtener de cada caso:

   * Número del caso.
   * Título.
   * Nombre del archivo.
4. Actualizar `content/manifest.json`.
5. Agregar los casos que todavía no estén registrados.
6. Mantener los casos ordenados por número ascendente.
7. Evitar registros duplicados.

### Formato esperado

```json
{ "archivo": "caso003.md", "n": "003", "titulo": "Diseño de rúbrica de evaluación" }
```

### Reglas

* `archivo` debe coincidir exactamente con el nombre real del archivo.
* `n` debe conservar tres dígitos.
* `titulo` debe obtenerse del YAML del caso.
* No inventar títulos ni números.
* No eliminar casos existentes salvo que el archivo correspondiente ya no exista en `casos/`.
* El resultado final de `content/manifest.json` debe ser JSON válido.
