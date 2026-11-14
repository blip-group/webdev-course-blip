# Guion de la Lección 5 · Construyamos una página de perfil personal

**Curso:** Fundamentos de Desarrollo Web · **Lección 5 de 6** · **Editor:** JSFiddle
**Duración:** unos 14 minutos · **Público:** estudiantes de 12 a 17 años, sin experiencia previa.

Este es el texto de la narración y lo que se ve en pantalla en cada escena. Entre corchetes van las indicaciones; no se leen en voz alta. El código terminado está en [`completed-examples/leccion-5/perfil-personal`](../completed-examples/leccion-5/perfil-personal) y el de partida, en [`starter-files/leccion-5/perfil-personal`](../starter-files/leccion-5/perfil-personal).

---

## Resumen de escenas

| # | Escena | Minuto | Duración aprox. |
|---|---|---|---|
| 1 | Introducción | 0:00 | 0:40 |
| 2 | La estructura: foto, nombre y descripción | 0:40 | 3:05 |
| 3 | Gustos y enlace | 3:44 | 2:48 |
| 4 | CSS: estilo de la página y la tarjeta | 6:32 | 1:21 |
| 5 | CSS: foto, títulos, lista y botón | 7:53 | 2:52 |
| 6 | Personalizar la página | 10:45 | 1:55 |
| 7 | El botón abre otro sitio | 12:40 | 1:09 |
| 8 | Reto y cierre | 13:49 | 0:39 |

---

## Escena 1 — Introducción (0:00–0:40)

**En pantalla:** el título de la lección y una tarjeta de perfil que se arma con cinco ingredientes (foto, nombre, descripción, gustos y botón); después, «Usamos todo lo que aprendimos»: HTML organiza el contenido y CSS da colores y estilos.
**Texto en pantalla:** «Foto · Nombre · Descripción · Gustos · Botón»

> Hola a todos y bienvenidos a esta nueva lección. Hoy vamos a crear nuestra página de perfil personal utilizando HTML y CSS. Nuestra página va a contener una fotografía, nuestro nombre, una pequeña descripción, una lista de nuestros gustos favoritos y un botón que nos llevará a otros sitios web.
>
> Para ello vamos a utilizar todo lo que hemos aprendido a lo largo de las lecciones anteriores. Recuerda que HTML nos permite organizar el contenido, mientras que CSS nos ayuda a darle colores y estilos.

---

## Escena 2 — La estructura: foto, nombre y descripción (0:40–3:45)

**En pantalla:** JSFiddle con los paneles de HTML, CSS y el resultado; el código se escribe paso a paso y se ejecuta cada pocas líneas.
**Texto en pantalla:** «main class="tarjeta"» · «img class="foto"» · «h1» · «p class="descripcion"»

> Comencemos. Abrimos JSFiddle en el navegador. Vemos que tenemos la sección de HTML, la de JavaScript y la de CSS, y esta parte de color blanco es donde va a salir el resultado. Aquí vamos a usar solamente HTML y CSS. JavaScript todavía no lo vamos a usar.
>
> Empezamos creando el espacio de nuestro trabajo con `main`: escribimos `main` y presionamos Tab, y automáticamente se abre la etiqueta. Le damos un espacio, porque esta va a ser nuestra área de trabajo. Le damos la clase `tarjeta`.
>
> Vamos a empezar con algo sencillo y rápido: insertar una imagen. Aquí tenemos la etiqueta `img`, que es una etiqueta que no necesita cierre. Dentro le asignamos la clase `foto`, que sirve para darle un estilo personalizado a esta imagen, y la dirección de la imagen, que es este enlace. También agregamos una descripción: «Foto de perfil». Si lo ejecutamos, ya aparece la foto cargada desde ese enlace.
>
> Ahora vamos a agregar nuestro nombre y una descripción. Para el nombre usamos `h1`, que es el título de nuestra página. Escribimos `h1`, presionamos Tab y dentro escribimos «¡Hola, soy Alex!». Si ejecutamos, ya nos muestra el título en grande.
>
> A continuación agregamos una pequeña descripción. La descripción va a ser un párrafo, así que usamos la etiqueta `p`. Como le vamos a dar estilos personalizados, le agregamos la clase `descripcion` y escribimos: «Soy estudiante y me encantan la tecnología, los videojuegos y la música».
>
> Ya tenemos nuestra foto de perfil, nuestro nombre como presentación y una descripción nuestra.

---

## Escena 3 — Gustos y enlace (3:44–6:32)

**En pantalla:** el panel de HTML con `h2`, `ul` con la clase `gustos`, tres `li` con emojis, y el enlace `a` con `href`; y el resultado a la derecha.
**Texto en pantalla:** «h2 = subtítulo» · «ul y li = lista con viñetas» · «a href = enlace»

> Ahora vamos a crear una lista con todos los gustos favoritos que tenemos. Para ello usamos `h2`, que sirve para agregar subtítulos. Debajo del párrafo escribimos «Mis cosas favoritas». Si ejecutamos, se ve más pequeño porque es un subtítulo.
>
> Ahora usamos la etiqueta `ul`, que sirve para crear una lista con viñetas. Dentro de esta lista vamos a colocar una etiqueta llamada `li`, que representa cada elemento de la lista. Le agregamos unos emojis para que sea más vistoso. Le damos a `ul` la clase `gustos`, para agregarle estilos después. Y en cada `li` escribimos un gusto: jugar videojuegos, escuchar música y aprender a programar. Si ejecutamos, sale así, con viñetas.
>
> Listo. Ahora vamos a agregar un enlace que nos llevará a un sitio web. Agregamos la etiqueta `a`, que nos permite dirigirnos hacia otra página web. Dentro de `href` va la dirección a la que vamos a ir. En esta ocasión vamos a utilizar la dirección de Wikipedia. Tú puedes cambiarla por otra página que te guste: solamente copias la dirección.
>
> Finalmente cerramos todas las etiquetas y, dentro de `a`, escribimos el texto del botón: «Visita mi sitio favorito». Si ejecutamos, ya salen nuestras cosas favoritas y el botón.
>
> Con esto, en HTML ya tendríamos todo. Ahora vamos a pasar a CSS.

---

## Escena 4 — CSS: estilo de la página y la tarjeta (6:32–7:53)

**En pantalla:** el panel de CSS con las reglas `body` y `.tarjeta`, y el resultado que cambia con cada propiedad.
**Texto en pantalla:** «body = toda la página» · «.tarjeta = la tarjeta» · «box-shadow = sombra»

> En CSS vamos a empezar dándole estilos al cuerpo de la página, que es `body`. Le damos un margen de cero y un `padding` de 40 píxeles arriba y abajo y 16 a los lados. Agregamos también la tipografía, `sans-serif`, que cambia bastante el aspecto. Y le damos un color de fondo a toda la página. Estos son estilos generales de la página.
>
> Ahora le agregamos estilos a la tarjeta. ¿Recuerdas que a `main` le pusimos una clase llamada `tarjeta`? Aquí la tenemos: la tarjeta con estos valores. Un fondo de color blanco; un `border-radius` de 20 píxeles, que es lo que le da el efecto curvo a las esquinas; y `text-align` con el valor `center`, para centrar todo el texto. Y usamos `box-shadow`, para generar un poco de sombra alrededor de la tarjeta.

---

## Escena 5 — CSS: foto, títulos, lista y botón (7:53–10:45)

**En pantalla:** el panel de CSS con las reglas `.foto`, `h1, h2`, `.descripcion`, `.gustos` y `.boton`, y el resultado.
**Texto en pantalla:** «.foto: forma circular» · «object-fit: cover» · «border-radius: 50%» · «padding = espacio interior»

> Vamos a darle estilos a la fotografía y al texto que tenemos dentro. Usamos la clase `foto`, y con esto le damos una forma circular a nuestra foto, para que se parezca a un perfil. Dentro usamos `object-fit` con el valor `cover`, que ajusta la imagen sin deformarla, y también `border-radius` de 50 %, que es lo que le da el efecto circular.
>
> Ahora vamos a darle un color azul a los títulos, `h1` y `h2`, separados por una coma. Como ves, ya cambió de color. Y también le damos estilo a la descripción: un color más oscuro. Podemos configurarlo; elegimos un tono más oscuro y, como ves, cambia el color.
>
> Ahora le damos estilo también a la lista de nuestros gustos. Y listo, queda mejor ordenada.
>
> Pero, como puedes ver, la página se desordenó un poco; ahora tenemos que arreglar la parte del botón. Le damos estilo al botón: con `background-color` lo cambiamos a azul, con `border-radius` redondeamos las esquinas, como lo hicimos con la tarjeta, y con `padding` le damos espacio entre el borde del botón y el texto.
>
> Y ya lo tendríamos listo. Este sería nuestro perfil. Como ves, es más vistoso y más completo que tenerlo solo en HTML.

---

## Escena 6 — Personalizar la página (10:45–12:40)

**En pantalla:** el panel de HTML donde se cambia el nombre, la descripción y los gustos; el panel de CSS donde se cambia el color del botón; y el resultado. Donde el ejemplo lleva el nombre del autor, se ve «tu nombre».
**Texto en pantalla:** «Cambia tu nombre» · «Cambia la descripción» · «Cambia los colores»

> Ya que está todo terminado, vamos a aprender cómo personalizarlo. Primero podemos cambiar el nombre «Alex» por uno diferente. Lo buscamos aquí y lo cambiamos: «Hola, soy» y tu nombre. Ejecutamos y, como ves, ya cambió: «Hola, soy» tu nombre, «soy estudiante y me encantan la tecnología, los videojuegos y la música».
>
> También podemos cambiar el nombre por un apodo que usemos, quizás en algunos juegos. Podemos modificar la descripción, o agregar otra cosa a la lista, por ejemplo, leer. Ejecutamos y ya vemos que se agregó correctamente. De esta manera, cada uno de nosotros puede crear una página única, con su propio estilo.
>
> Y, de verdad, no es tan complicado: solamente hay que practicar bastante. Ya lo tenemos todo completo, HTML y CSS.
>
> También podemos cambiar el color del botón: actualmente es un azul oscuro. Hacemos clic y escogemos otro color; por ejemplo, un verde. Como puedes ver, ya cambió a un verde oscuro. Esto lo podemos hacer a nuestro gusto: personalizarlo y agregar más cosas favoritas. Aquí se ve un poco separado, pero lo juntamos y ya se ve mejor.

---

## Escena 7 — El botón abre otro sitio (12:40–13:49)

**En pantalla:** «¡Felicitaciones!» con lo que se aprendió con HTML; una lámina que dice que el botón abre una pestaña nueva y cómo cambiar el enlace; el editor con la nueva dirección en `href`; y otra lámina con el botón abriendo la nueva dirección.
**Texto en pantalla:** «¡Felicitaciones!» · «Imágenes · Títulos · Párrafos · Listas · Enlaces»

> Felicitaciones: hemos terminado nuestra primera página de perfil personal. Durante esta lección aprendimos a utilizar HTML para agregar imágenes, títulos, párrafos, listas y enlaces, y con eso creamos un pequeño botón.
>
> Vamos a probar el botón: nos lleva al enlace de Wikipedia. Aquí podemos cambiar el enlace por otro. Podemos poner uno diferente, por ejemplo, la página principal de otro sitio que nos guste. Solamente copiamos el enlace, vamos aquí y lo modificamos. Lo pegamos y listo. Ejecutamos, hacemos clic en «Visita mi sitio favorito» y nos lleva a la nueva página.

---

## Escena 8 — Reto y cierre (13:49–14:28)

**En pantalla:** «Reto: crea tu propia tarjeta» y «Experimenta, practica y sigue aprendiendo».
**Texto en pantalla:** «Reto: crea tu propia tarjeta»

> Ahora te dejo un pequeño reto: crea tu propia tarjeta. Cámbiale el nombre, la fotografía y quizás algunos de tus gustos, y también los colores. Recuerda que no necesitas compartir información privada para tener una página creativa.
>
> Lo importante es experimentar, practicar y seguir aprendiendo. Muchas gracias por acompañarme en esta lección, y nos vemos en la próxima.
