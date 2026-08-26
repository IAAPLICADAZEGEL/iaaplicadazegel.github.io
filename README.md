# IA Aplicada · Zegel

Aplicación de una sola página que consume documentos Markdown con front matter YAML.

## Publicar en GitHub Pages

1. Sube el contenido de esta carpeta a la raíz del repositorio.
2. Settings → Pages → Source: `main` / carpeta raíz.
3. **No borres `.nojekyll`**: sin ese archivo, Jekyll convierte los `.md` en `.html` y la aplicación deja de encontrarlos.
4. Ajusta `CFG.base` en `index.html` a la URL real del sitio. Disqus la usa como identidad de cada hilo.

## Probar en local

`fetch()` no funciona con `file://`. Levanta un servidor:

```
python -m http.server 8000
```

Y abre `http://localhost:8000`.

## Agregar una clase o un caso

1. Crea el archivo en `clases/` o `casos/`.
2. Añade su entrada en `content/manifest.json`.

No hay descubrimiento automático de archivos: el manifiesto es la única fuente de verdad.

## Front matter admitido

```yaml
---
titulo: Anatomía de una instrucción
modulo: Clase 03
fecha: 18 de agosto de 2026
lectura: 12 min de lectura
estado: Semana 04
resumen: Una línea que aparece bajo el título.
---
```

## Atajos de teclado

| Tecla | Acción |
|---|---|
| `/` o `Ctrl/Cmd+K` | Buscar |
| `o` | Comentarios |
| `t` | Cambiar tema |
| `Esc` | Cerrar lo que esté abierto |

## Markdown soportado

Encabezados, párrafos, negrita, cursiva, código en línea, bloques de código, listas ordenadas y sin ordenar, citas, tablas, reglas, enlaces e imágenes. Una URL de YouTube sola en su línea se convierte en video incrustado.

Las rutas de imagen se resuelven desde la raíz del sitio: `![](images/diagrama.png)`.
