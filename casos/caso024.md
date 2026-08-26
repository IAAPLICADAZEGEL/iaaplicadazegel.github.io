---
titulo: Del dashboard local al dashboard publicado
modulo: Caso 024
area: General
resumen: Qué cambia cuando un archivo que funciona en nuestra máquina se convierte en una dirección que otros consultan.
---

## A. Situación

El dashboard funciona bien en nuestra computadora: doble clic y ahí están los
indicadores. Gerencia pide consultarlo desde otros equipos, con un enlace. El
problema ya no es de análisis ni de visualización: es que el resultado tiene que
salir de nuestro escritorio.

## B. Objetivo

Distinguir construir de publicar, y reconocer qué responsabilidades aparecen
cuando un recurso propio pasa a ser consultado por otras personas.

## C. Requerimientos

- Cuenta activa en uno de estos asistentes (la versión gratuita basta):
  - [ChatGPT](https://chatgpt.com)
  - [Claude](https://claude.ai)
  - [Gemini](https://gemini.google.com)
- El dashboard HTML ya construido, en un solo archivo o como carpeta de proyecto.
- Una cuenta de Google, para la ruta de publicación integrada.
- Una cuenta en un servicio de alojamiento web como [Netlify](https://www.netlify.com).
- Un segundo dispositivo para comprobar el acceso.

## D. Desarrollo

Recorremos el ciclo **proyecto local → publicar → URL → usuarios**.

1. **Ruta A: publicar dentro del entorno de trabajo.** Insertamos o integramos el
   dashboard en un sitio sencillo hecho con Google Sites y anotamos qué tan directo
   resultó, qué se integró bien con las cuentas del equipo, qué restricciones
   aparecieron y qué costaría mantenerlo.
2. **Ruta B: alojar el proyecto como sitio web.** Publicamos los mismos archivos en
   un servicio de alojamiento y obtenemos una dirección propia. Anotamos el control
   sobre los archivos, cómo se actualiza una versión nueva, qué tan simple fue el
   despliegue y hasta dónde podría crecer.
3. **Probar de verdad.** Abrimos ambas direcciones desde otro dispositivo y fuera
   de la red de la oficina. Un dashboard que solo carga en nuestra máquina no está
   publicado.
4. **Actualizar.** Cambiamos algo en el dashboard y lo publicamos otra vez por
   ambas rutas, midiendo cuántos pasos toma cada una.
5. **Comparar.** Ponemos las dos rutas frente a los mismos criterios: facilidad,
   control, actualización, requisitos técnicos y para qué situación conviene cada
   una.
6. **Cerrar el encargo.** Definimos por escrito quién puede ver el enlace, quién lo
   actualiza y qué pasa si deja de funcionar un lunes por la mañana.

> Mientras era un archivo, un error lo notábamos nosotros. Desde que es un enlace,
> lo nota Gerencia.

## E. Conceptos

- **Local:** recurso que se ejecuta desde nuestro propio dispositivo.
- **Hosting:** infraestructura que almacena y sirve contenido web.
- **Despliegue:** proceso por el que una aplicación se prepara y se publica.
- **URL:** dirección mediante la cual otras personas acceden al recurso.
- **Mantenimiento:** trabajo continuo de conservar disponible y actualizado lo publicado.

## F. Comprobación

Un compañero sostiene que publicar el dashboard es solo subir el archivo, y que
una vez obtenido el enlace la tarea queda cerrada. ¿Qué se pierde en el camino?

- a) La verificación del acceso, porque un enlace que abre desde nuestra sesión puede exigir permisos que las demás personas de la organización no tienen concedidos.
- b) El control de versiones, dado que cada actualización sustituye lo publicado y conviene saber qué versión están viendo quienes consultan el tablero en ese momento.
- c) Que a partir del enlace respondemos por lo que muestra.
- d) La elección de la ruta de publicación, ya que integrar el tablero en el entorno de trabajo y alojarlo como sitio propio ofrecen niveles de control muy distintos.
