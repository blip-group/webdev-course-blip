# Guion de la Lección 4 · Pintando y decorando con CSS

**Curso:** Fundamentos de Desarrollo Web · **Lección 4 de 6** · **Editor:** JSFiddle
**Duración:** unos 12 minutos · **Público:** estudiantes de 12 a 17 años, sin experiencia previa.

Este es el texto de la narración y lo que se ve en pantalla en cada escena. Entre corchetes van las indicaciones; no se leen en voz alta. El código terminado está en [`completed-examples/leccion-4/tarjeta`](../completed-examples/leccion-4/tarjeta) y el de partida, en [`starter-files/leccion-4/tarjeta`](../starter-files/leccion-4/tarjeta).

---

## Resumen de escenas

| # | Escena | Minuto | Duración aprox. |
|---|---|---|---|
| 1 | Introducción: ¿qué es CSS? | 0:00 | 0:51 |
| 2 | El HTML de la tarjeta | 0:51 | 1:41 |
| 3 | Color del texto | 2:32 | 1:37 |
| 4 | Color de fondo y clases | 4:09 | 0:57 |
| 5 | Tipografía | 5:06 | 1:10 |
| 6 | Esquinas redondeadas | 6:16 | 1:18 |
| 7 | Alinear el texto | 7:34 | 1:06 |
| 8 | Ancho, espacios y márgenes | 8:40 | 0:50 |
| 9 | El botón | 9:30 | 1:20 |
| 10 | Repaso | 10:50 | 0:45 |
| 11 | Reto y cierre | 11:35 | 1:00 |

---

## Escena 1 — Introducción: ¿qué es CSS? (0:00–0:51)

**En pantalla:** el título de la lección; una página sin estilo; los contornos `<h1>`, `<p>` y `<button>` como esqueleto; y la idea de que CSS «viste, pinta y decora».
**Texto en pantalla:** «HTML pone el contenido» · «Aquí aparece CSS» · «Hoy: de una página sencilla a una tarjeta moderna»

> Hola a todos. En esta lección vamos a aprender a darle estilo a una página web utilizando CSS.
>
> Hasta ahora hemos visto que HTML nos permite colocar contenido como títulos, párrafos, imágenes o enlaces, pero una página creada solamente con HTML puede verse bastante simple. Aquí es donde aparece CSS.
>
> Vamos a imaginar que HTML es la estructura, el esqueleto de nuestra página web, mientras que CSS es el encargado de vestirla, pintarla o decorarla. Con CSS podemos cambiar colores, tipos de letra, fondos, bordes y muchas otras características visuales.
>
> Hoy vamos a transformar una página bastante sencilla en una tarjeta mucho más moderna.

---

## Escena 2 — El HTML de la tarjeta (0:51–2:32)

**En pantalla:** JSFiddle: el panel de HTML con la tarjeta, el panel de CSS vacío y el resultado.
**Texto en pantalla:** «div class="tarjeta"» · «h1 · p · button»

> Ahora vamos a crear algo sencillo utilizando HTML.
>
> Escribimos aquí un `div` con la clase `tarjeta`, y lo cerramos. Dentro vamos a abrir un título con `h1` y escribimos «Mi espacio web». Lo cerramos. Ahora abrimos también un pequeño párrafo y escribimos «Hola, estoy aprendiendo a crear páginas web». Cerramos igualmente el párrafo. Y vamos a trabajar también con un botón: lo abrimos, escribimos su texto y lo cerramos.
>
> Listo. Lo ejecutamos y funciona. Aquí tenemos una tarjeta que contiene tres elementos: un título, un pequeño texto y un botón. Sin embargo, como podemos apreciar, todavía se ve muy simple. El objetivo es mejorarla usando CSS.

---

## Escena 3 — Color del texto (2:32–4:09)

**En pantalla:** el panel de CSS con la regla `h1 { color: … }` y el resultado; una lista de propiedades que va creciendo a la derecha.
**Texto en pantalla:** «color» · «Nombres de colores» · «Códigos HEX»

> Vamos a comenzar cambiando el color del título. Para modificar el color de un elemento podemos utilizar la propiedad `color` y definimos el color; en este caso, `blue`. Como puedes apreciar, cambia casi al instante. Ejecutamos y el resultado es el mismo: ahora el título aparece de color azul.
>
> CSS también nos permite utilizar nombres de colores, como `red`, `green` o `purple`. Pero existe otra manera muy utilizada: los códigos HEX. Por ejemplo, en lugar de escribir un nombre como `green`, podemos escribir un código como este.
>
> El símbolo numeral seguido de seis caracteres representa un color específico. No es necesario conocer ni memorizar estos códigos: normalmente se pueden obtener con una paleta de colores, como esta. Lo importante es saber que CSS acepta tanto nombres de colores como códigos HEX.

---

## Escena 4 — Color de fondo y clases (4:09–5:06)

**En pantalla:** el panel de CSS con la regla `.tarjeta { background-color: … }` y el resultado.
**Texto en pantalla:** «background-color» · «.tarjeta = la clase tarjeta»

> Ahora vamos a cambiar el fondo. Para eso utilizaremos otra propiedad, llamada `background-color`. Vamos a escribirla dentro de una regla nueva; en un momento aclararé por qué.
>
> Ahora nuestra tarjeta, como se puede apreciar, tiene un fondo diferente. Algo importante que se puede observar aquí es el punto antes de la palabra `tarjeta`. Significa que estamos seleccionando una clase de HTML en nuestro CSS. En el HTML escribimos `class="tarjeta"`, y en CSS encontramos esa clase usando un punto y la palabra `tarjeta`. De esta manera definimos qué estamos decorando exactamente.

---

## Escena 5 — Tipografía (5:06–6:16)

**En pantalla:** el panel de CSS con `font-family` y el resultado, primero con Arial y luego con otra letra.
**Texto en pantalla:** «font-family = el tipo de letra»

> Ahora también podemos cambiar el tipo de letra. Usamos una propiedad llamada `font-family` y vamos a seleccionar Arial. Ahora el texto utiliza la tipografía Arial.
>
> Se puede probar también con otras tipografías, como Georgia: el título cambia. Como se puede observar, solamente cambiando una propiedad se puede modificar bastante la apariencia de nuestra página. Para este ejemplo, lo voy a dejar en Arial.

---

## Escena 6 — Esquinas redondeadas (6:16–7:34)

**En pantalla:** el panel de CSS con `border-radius` y el resultado, primero con 15 píxeles y luego con 35.
**Texto en pantalla:** «border-radius = esquinas redondeadas» · «15px · 35px»

> Ahora vamos a hacer que la tarjeta se vea un poco más moderna. Actualmente, como se aprecia, las esquinas son totalmente rectas: es como un rectángulo. Pero CSS tiene una propiedad llamada `border-radius`, que nos permite redondearlas. La añadimos aquí mismo y ponemos 15 píxeles. Ejecutamos, y ahora las esquinas están redondeadas.
>
> Se puede aumentar o disminuir según el número que coloquemos dentro de esta propiedad. Por ejemplo, probemos con 35 píxeles: es más notorio en los bordes. Vamos a dejarlo en 15.
>
> Este es un buen ejemplo de algo importante cuando aprendemos CSS: siempre podemos experimentar, ir de adelante hacia atrás y de atrás hacia adelante. Si algo no nos gusta, simplemente cambiamos el valor y observamos el resultado.

---

## Escena 7 — Alinear el texto (7:34–8:40)

**En pantalla:** el panel de CSS con `text-align: center` y el resultado.
**Texto en pantalla:** «text-align = alinear el texto» · «left · right · center»

> Vamos ahora a centrar el contenido, para que se vea más estilizado. La propiedad `text-align` nos deja centrar el texto, pero también nos permite ponerlo a la izquierda o a la derecha. Vamos a dejarlo en el centro, para que todo esté alineado.
>
> Como ves, hasta ahora no hemos cambiado nuestro HTML: solamente estamos modificando CSS. Esto demuestra una de las ventajas de CSS: podemos mantener nuestro contenido y cambiar completamente su apariencia.

---

## Escena 8 — Ancho, espacios y márgenes (8:40–9:30)

**En pantalla:** el panel de CSS con `width`, `padding` y `margin: 40px auto`, y el resultado con la tarjeta centrada.
**Texto en pantalla:** «width = ancho» · «padding = espacio interior» · «margin: 40px auto = margen y centrado»

> Vamos a realizar unos últimos cambios para que realmente parezca una tarjeta. Agregamos aquí mismo el ancho. Le damos también un pequeño espacio interior y unos márgenes.
>
> Ahora la tarjeta tiene un tamaño definido, tiene espacio alrededor del contenido y también aparece centrada.

---

## Escena 9 — El botón (9:30–10:50)

**En pantalla:** el panel de CSS con la regla `button { … }` y el resultado.
**Texto en pantalla:** «background-color · color · border · border-radius · padding»

> Vamos a darle estilo también a nuestro botón, porque está pasando muy desapercibido. Escribimos `button` y le damos un fondo; yo le voy a poner este color. Le damos el color de texto, blanco. Hacemos que no tenga borde, es decir, que no tenga una pequeña línea alrededor. Le damos esquinas redondeadas y también un espacio interior.
>
> Ahora sí: tenemos un resultado bastante diferente del que teníamos al comenzar.

---

## Escena 10 — Repaso (10:50–11:35)

**En pantalla:** «Así empezamos» (la página sin estilo) y «Así terminamos» (la tarjeta final); después, las cinco propiedades de la lección con una muestra de cada una.
**Texto en pantalla:** «color · background-color · font-family · border-radius · text-align»

> Vamos a recordar cómo empezamos: teníamos un título, un párrafo y un botón que prácticamente no tenían ningún diseño. Pero utilizando unas cuantas propiedades de CSS hemos conseguido modificar completamente esa experiencia.
>
> Hoy utilizamos principalmente `color`, para cambiar el color del texto; `background-color`, para cambiar el fondo; `font-family`, para cambiar la tipografía; `border-radius`, para redondear las esquinas; y `text-align`, para alinear nuestro contenido. No necesitamos código complicado para conseguir un resultado agradable.

---

## Escena 11 — Reto y cierre (11:35–12:36)

**En pantalla:** «Reto: personaliza tu tarjeta»; la tarjeta cambia a verde, luego de tipografía y luego de esquinas; al final, «HTML da el contenido · CSS controla cómo se ve» y «¡Ahora te toca!».
**Texto en pantalla:** «Reto: personaliza tu tarjeta»

> Antes de terminar, te propongo un pequeño reto antes de pasar a la siguiente lección. Toma esta tarjeta y personalízala. Puedes cambiar el color a verde, por ejemplo, o a algún color favorito que tengas. También puedes cambiar el texto y colocar tu nombre, probar otra tipografía y experimentar cambiando el valor de los bordes. La mejor manera de aprender CSS es probar diferentes valores y observar qué ocurre.
>
> En esta lección aprendimos que HTML proporciona el contenido de una página, mientras que CSS nos permite controlar cómo se ve. Y con solamente unas pocas propiedades logramos transformar un contenido sencillo en una tarjeta mucho más moderna. Muchas gracias.
