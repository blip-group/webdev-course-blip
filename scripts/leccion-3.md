# Guion de la Lección 3 · Enlaces, imágenes seguras y listas interactivas

**Curso:** Fundamentos de Desarrollo Web · **Lección 3 de 6** · **Editor:** JSFiddle
**Duración:** unos 8 minutos · **Público:** estudiantes de 12 a 17 años, sin experiencia previa.

Este es el texto de la narración y lo que se ve en pantalla en cada escena. Entre corchetes van las indicaciones; no se leen en voz alta. El código terminado está en [`completed-examples/leccion-3/catalogo`](../completed-examples/leccion-3/catalogo) y el de partida, en [`starter-files/leccion-3/catalogo`](../starter-files/leccion-3/catalogo).

---

## Resumen de escenas

| # | Escena | Minuto | Duración aprox. |
|---|---|---|---|
| 1 | Introducción | 0:00 | 0:24 |
| 2 | El código base | 0:24 | 0:16 |
| 3 | Lista con viñetas | 0:40 | 1:20 |
| 4 | Lista numerada | 2:00 | 1:14 |
| 5 | Imágenes | 3:14 | 1:52 |
| 6 | Enlaces | 5:06 | 1:59 |
| 7 | Repaso y cierre | 7:05 | 1:18 |

---

## Escena 1 — Introducción (0:00–0:24)

**En pantalla:** el título de la lección; una página que se arma poco a poco (párrafo → lista → imagen → enlace).
**Texto en pantalla:** «Listas · Imágenes · Enlaces»

> En la lección anterior aprendimos a crear la estructura básica de una página, con títulos y párrafos. Ahora le daremos más contenido usando listas, imágenes y enlaces.
>
> Piensa en una página donde recomiendas tus juegos favoritos. No todo tiene que estar en un solo párrafo: también podrías organizarlos con nombres en una lista, añadir imágenes y dejar un enlace para que conozcan más.

---

## Escena 2 — El código base (0:24–0:40)

**En pantalla:** JSFiddle con el código base (`h1` y `p`) y el resultado a la derecha.
**Texto en pantalla:** «Código base: título y párrafo»

> Ahora vamos a construir un pequeño catálogo en JSFiddle. Copiamos este código: una etiqueta `h1` para el título y una `p` para el párrafo. Lo ejecutamos con el botón Run y este es el resultado.

---

## Escena 3 — Lista con viñetas (0:40–2:00)

**En pantalla:** una lámina con una lista con viñetas; después, el código con un subtítulo `h2`, una lista `ul` y tres elementos `li`.
**Texto en pantalla:** «ul = lista con viñetas» · «li = cada elemento»

> El título y el párrafo ya están preparados. Ahora vamos con los nombres de los juegos. Para agrupar elementos sin indicar una clasificación, podemos usar una lista con viñetas; por ejemplo, una selección de tres juegos.
>
> Lo haremos así. Primero escribimos un subtítulo con `h2`, que dirá «Mi selección», lo cerramos y presionamos Run.
>
> Para hacer la lista, primero necesitamos la etiqueta `ul`. La cerramos y, dentro de ella, pondremos los elementos de la lista, cada uno con una etiqueta `li`. Se me ocurre como primer juego Minecraft. Cerramos la etiqueta y presionamos Run.
>
> Ese es el primer juego. Si queremos agregar más, simplemente reutilizamos el código y lo repetimos adentro. Podemos poner, por ejemplo, God of War y Fortnite. Presionamos Run de nuevo y ahí están los tres juegos.

---

## Escena 4 — Lista numerada (2:00–3:14)

**En pantalla:** una lámina que compara `ul` y `ol` («¿y si importa el orden?»); después, el código con la lista `ol` «Mi orden de preferencia».
**Texto en pantalla:** «ol = lista numerada» · «El orden importa»

> Una lista permite que el navegador entienda que estos tres nombres pertenecen a un mismo grupo; así se organizan las páginas web.
>
> Ahora imaginemos que queremos mostrar un orden de preferencia. En este caso podemos usar una lista numerada. Vamos a conservar la primera lista, la que no tiene números, y vamos a agregar otra para poder compararlas. La agregamos dejando un espacio.
>
> Es lo mismo que antes, pero en vez de «Mi selección» será «Mi orden de preferencia», y en vez de `ul` usaremos `ol`. La cerramos y metemos los mismos elementos.
>
> Si la ejecutamos, veremos primero Minecraft, luego God of War y luego Fortnite. Lo que cambia es el orden: si ponemos God of War al inicio, se mostrará como el número uno.

---

## Escena 5 — Imágenes (3:14–5:06)

**En pantalla:** una lámina que dice que la imagen se muestra con una dirección de internet, sin descargar archivos ni usar carpetas; después, el código con `h2`, `img`, `src`, `alt` y `width`, y la imagen abierta en su pestaña; una lámina sobre `alt`; y el resultado sin `width`.
**Texto en pantalla:** «img: inserta una imagen» · «src = de dónde viene» · «alt = descripción corta» · «width = ancho»

> Nuestro catálogo ya tiene listas. Ahora vamos a agregar una imagen con los videojuegos. Solo vamos a usar una dirección de internet para mostrarla: no tenemos que descargar archivos ni trabajar con ninguna carpeta.
>
> Primero hacemos un poco de espacio para organizarnos mejor y escribimos un subtítulo `h2`, que cerramos. Dentro pondremos el texto «Una imagen para el catálogo».
>
> Debajo ponemos la etiqueta de imagen, `img`, que sirve para insertarla. Con `src` indicamos la fuente, es decir, de dónde se va a obtener la imagen. En este caso es una imagen de dos personas jugando. Pegamos aquí la dirección.
>
> Luego, debajo, agregamos una descripción de la imagen, que veremos en un momento: `alt`, igual a una descripción corta. Por ejemplo, «Dos personas jugando FIFA». Y después `width`, para configurar el ancho.
>
> Lo ejecutamos y este es el resultado. Fíjate en que la descripción no aparece como texto en la página: solo se muestra en lugar de la imagen cuando esta no se puede cargar, y sirve para describirla.
>
> ¿Qué pasa si borramos el ancho? Mira: la imagen sale enorme. Configurar el ancho sirve para que no se desborde y para que se muestre bien.

---

## Escena 6 — Enlaces (5:06–7:05)

**En pantalla:** una lámina sobre el enlace o hipervínculo; después, el código con `h2`, `p`, `a`, `href`, `target="_blank"` y `rel="noopener noreferrer"`; y una lámina que dice que el enlace se abre en otra pestaña.
**Texto en pantalla:** «a = enlace» · «href = la dirección» · «target="_blank" = en otra pestaña» · «rel="noopener noreferrer" = buena práctica»

> Ahora nos falta una forma de visitar otra página desde nuestro catálogo. Para eso vamos a crear un enlace, también llamado hipervínculo. Vamos a añadir el sitio oficial de Fortnite, por ejemplo, porque está en nuestra lista.
>
> Primero dejamos unos espacios y escribimos un subtítulo, que cerramos. Dentro ponemos el texto «Conoce uno de estos juegos». Después escribimos una `p`, para que sea un párrafo, la cerramos y, dentro, ponemos todo lo demás.
>
> Para el enlace usamos la etiqueta `a`, un espacio, y con `href` indicamos la dirección. Vamos al sitio de Fortnite, copiamos la dirección y la pegamos aquí.
>
> Ahora configuramos el enlace. Primero `target`: si elegimos `_blank`, el enlace se abre en otra pestaña y no en la misma en la que estamos.
>
> Después, `rel`. Es opcional, pero es una buena práctica. Dentro de `rel` escribimos `noopener noreferrer`; esto es para que, al abrir el sitio, no se le envíe información de referencia.
>
> Después cerramos la etiqueta y añadimos el texto del enlace dentro del párrafo: «Visitar el sitio oficial de Fortnite». Lo ejecutamos: aquí se ve el enlace, le damos clic y nos lleva al sitio de Fortnite.

---

## Escena 7 — Repaso y cierre (7:05–8:24)

**En pantalla:** el código con un cuarto juego y otro enlace; después, un resumen con el texto, las listas, la imagen y los enlaces, y «¡Ahora te toca!» (8 segundos sin voz).
**Texto en pantalla:** «Texto · Listas · Imagen · Enlaces»

> Ahora hagamos un repaso de todo lo que hicimos. Primero vamos a añadir otro juego a la lista: reutilizamos este código y lo cambiamos por un juego que también nos gusta, Factorio.
>
> Después agregamos el enlace de la página de Factorio: copiamos la dirección y la reemplazamos en el enlace de Fortnite.
>
> Luego presionamos Run. Primero vemos que se actualizaron la lista sin números y la numerada. Miramos el enlace y nos lleva al sitio de Factorio.
>
> Hemos construido el catálogo por partes: primero el texto, luego las listas, luego la imagen y finalmente los enlaces, que funcionan correctamente. Probar cada paso con práctica nos ayuda a mejorar y a detectar errores a tiempo.
