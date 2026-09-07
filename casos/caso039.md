---
titulo: Generación de video de logotipo
modulo: Caso 039
area: Video
---

## Prompt

> Archivo usados:
>
> [Logo / recurso principal](https://drive.google.com/file/d/1SfQDuf_ApxdPW1ScJUMW3v1PxJGgznaT/view?usp=sharing)
>
> Herramienta sugerida:
>
> [Google Flow](https://flow.google.com/)

```text
Analiza el logotipo adjunto y crea un prompt breve para animarlo de forma profesional.

La animación debe construirse a partir de los elementos visuales del propio logo: formas, líneas, símbolos, colores, texturas o conceptos que pueda representar la marca.

Describe únicamente lo que ocurre en escena, en orden cronológico, desde el inicio hasta la aparición final del logotipo.

La animación debe sentirse corporativa, elegante y coherente con la identidad visual del logo.

El resultado debe:
- explicar cómo entra o aparece el logo;
- indicar qué elementos se mueven, transforman o se integran;
- aprovechar los colores y formas del diseño original;
- terminar con el logotipo completo, limpio y claramente visible;
- mantener intactos el nombre, símbolo, proporciones y diseño del logo.

No describas duración ni segundos.
No expliques el proceso creativo.
No incluyas parámetros técnicos.
No agregues eslóganes ni textos que no existan en el logo.
No describas la empresa salvo que sea necesario para entender la animación.

Devuelve únicamente el prompt de animación, en texto plano.
````

---

## Flujo de trabajo elaborado

### 1. Generación de secuencias

Adjuntar el logotipo y solicitar propuestas de animación.

**Prompt:**

```text
Analiza el logotipo adjunto y proporciona 5 ideas de secuencia visual si mi objetivo es realizar una animación profesional de presentación del logotipo.

Cada propuesta debe describir únicamente lo que ocurre en escena, desde el inicio hasta la aparición final del logo.

Las ideas deben aprovechar las formas, colores y elementos visuales presentes en el propio logotipo.

No describas duración, segundos ni parámetros técnicos.

Devuelve las 5 propuestas numeradas.
```

---

### 2. Desarrollo de la secuencia seleccionada

Elegir una de las propuestas y dividirla en tres momentos visuales: inicio, intermedio y final.

**Prompt:**

```text
Desarrolla la secuencia N.º [X] en 3 prompts independientes para generar imágenes:

1. Imagen inicial
2. Imagen intermedia
3. Imagen final

Las tres imágenes deben representar momentos consecutivos de una misma animación y mantener total continuidad visual entre ellas.

Conserva el diseño, colores, proporciones y elementos originales del logotipo.

Describe únicamente lo que debe verse en cada imagen.

Formato: [vertical 9:16 / panorámico 16:9].
```

---

### 3. Desarrollo de las imágenes

Generar las imágenes una por una utilizando los prompts anteriores.

#### Imagen inicial

```text
Genera la imagen inicial utilizando el prompt definido anteriormente.

Formato: [9:16 / 16:9].
```

#### Imagen intermedia

```text
Genera ahora la imagen intermedia de la misma secuencia.

Formato: [9:16 / 16:9].
```

#### Imagen final

```text
Genera ahora la imagen final de la secuencia.

Formato: [9:16 / 16:9].
```

---

### 4. Generación del prompt orquestador

Una vez obtenidas las tres imágenes, solicitar el prompt que describirá toda la animación.

**Prompt:**

```text
Analiza las tres imágenes de referencia: inicio, intermedio y final.

Crea un único prompt de animación que conecte las tres imágenes en orden cronológico.

Describe únicamente lo que ocurre en escena y cómo los elementos se mueven, aparecen, se transforman o se integran desde la imagen inicial hasta la imagen final.

La transición debe ser continua, natural, elegante y profesional.

Respeta exactamente la identidad visual del logotipo.

No describas segundos ni duración.
No agregues escenas nuevas.
No agregues textos que no aparezcan en las imágenes.
No expliques el proceso.
No incluyas parámetros técnicos.

Devuelve únicamente el prompt final de animación en texto plano.
```

---

### 5. Generación del video en Google Flow

1. Ir a **Google Flow**.
2. Crear un proyecto nuevo.
3. Seleccionar generación de video.
4. Agregar las imágenes **inicial, intermedia y final** como ingredientes o referencias visuales.
5. Insertar el **prompt orquestador**.
6. Revisar que el orden de las referencias corresponda a la secuencia.
7. Enviar y generar el video.

