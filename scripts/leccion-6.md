# Guion de la Lección 6 · ¡Mi código no funciona!

**Curso:** Fundamentos de Desarrollo Web · **Lección 6 de 6** · **Editor:** CodePen
**Duración:** unos 10 minutos · **Público:** estudiantes de 12 a 17 años, sin experiencia previa.

Este es el texto de la narración y lo que se ve en pantalla en cada escena. Entre corchetes van las indicaciones; no se leen en voz alta.

---

## Resumen de escenas

| # | Escena | Minuto | Duración aprox. |
|---|---|---|---|
| 1 | Gancho | 0:00 | 0:45 |
| 2 | El método de 3 pasos | 0:45 | 1:00 |
| 3 | Error 1 · Etiqueta sin cerrar | 1:45 | 1:05 |
| 4 | Error 2 · Nombre mal escrito | 2:50 | 0:50 |
| 5 | Error 3 · Falta el punto y coma | 3:40 | 1:05 |
| 6 | Error 4 · Comilla sin cerrar | 4:45 | 0:50 |
| 7 | Error 5 · El estilo no se aplica | 5:35 | 0:40 |
| 8 | Reto "Encuentra el error" | 6:15 | 2:15 |
| 9 | Cierre y próximos pasos | 8:30 | 1:30 |

---

## Escena 1 — Gancho (0:00–0:45)

**En pantalla:** la página de perfil dividida en dos mitades, o una detrás de otra. Primero la sana ("Lo que quería"), luego la rota por el error 5 ("Lo que apareció").
**Texto en pantalla:** "Lo que quería" → "Lo que apareció"

> ¡Hola! ¿Alguna vez escribiste código y, al ejecutarlo, no salió lo que esperabas? Mira: esto es lo que yo quería… [pausa corta] …y esto es lo que apareció.
>
> Tranquilo: le pasa a todo el mundo, incluso a personas que programan desde hace muchos años. Equivocarse no significa que lo estés haciendo mal. Significa que la computadora te está pidiendo una pista.
>
> En esta última lección vas a aprender a ser un detective de código: encontrar el error, arreglarlo y seguir adelante. Al final tendrás un reto para practicar, así que ten tu navegador a mano. ¡Empecemos!

---

## Escena 2 — El método de 3 pasos (0:45–1:45)

**En pantalla:** una tarjeta limpia con tres pasos que aparecen uno por uno, al ritmo de la voz.
**Texto en pantalla:** "1. Mira" · "2. Busca la pista" · "3. Cambia una sola cosa" · al final, la palabra "Depurar = buscar y arreglar errores".

> Antes de ver errores concretos, necesitas un método. Son tres pasos y los vas a usar siempre.
>
> Paso uno: mira. Pregúntate: ¿qué esperaba ver y qué estoy viendo? Compararlo te dice dónde está el problema.
>
> Paso dos: busca la pista. Casi siempre es algo pequeño: una etiqueta que falta, una comilla, un punto y coma o una letra mal escrita.
>
> Y paso tres: cambia una sola cosa y vuelve a ejecutar. Solo una. Si cambias cinco cosas a la vez, no sabrás cuál arregló el problema.
>
> A este proceso, en programación, se le llama depurar. Depurar es simplemente buscar y arreglar errores. Ahora vamos a ver cinco errores clásicos. Casi todos los principiantes los cometen, y desde hoy tú ya los vas a reconocer.

---

## Escena 3 — Error 1: etiqueta sin cerrar (1:45–2:50)

**En pantalla:** CodePen con el código base. Señala con el cursor `<h2>Mis cosas favoritas</h2>`, borra `</h2>`, muestra el resultado y vuelve a escribirlo.
**Texto en pantalla:** "Error 1 · Etiqueta sin cerrar" → al arreglarlo: "Solución: cerrar la etiqueta `</h2>`"

> Error número uno: olvidar cerrar una etiqueta. Fíjate en el título "Mis cosas favoritas". Voy a borrar su etiqueta de cierre, la que lleva la barra. [borrar `</h2>`]
>
> Mira lo que pasó: la lista y el botón ahora tienen letra de título, enorme y en negrita. Para el navegador, el título nunca terminó, así que todo lo que escribí después sigue dentro de él.
>
> La pista: cuando de pronto todo lo que sigue cambia de tamaño o de estilo, revisa si olvidaste cerrar algo antes.
>
> La solución es escribir la etiqueta de cierre. [escribir `</h2>`] ¡Listo!
>
> Un truco: apenas abras una etiqueta, escribe de una vez su cierre y luego rellena lo que va en medio. Muchos editores lo hacen por ti, pero no siempre.

---

## Escena 4 — Error 2: nombre mal escrito (2:50–3:40)

**En pantalla:** acerca el zoom a la línea de la imagen. Cambia `src` por `scr`, muestra que la foto desaparece (queda el texto alternativo) y corrígelo.
**Texto en pantalla:** "Error 2 · Nombre mal escrito" → "`scr` ≠ `src`"

> Error número dos: escribir mal el nombre de algo. Aquí cambié la palabra "src" por "scr", con las letras cambiadas de lugar. [mostrar] La foto desapareció, y en su lugar solo queda el texto alternativo.
>
> Fíjate que el navegador no te avisa con un cartel rojo. Simplemente no entiende, y sigue de largo.
>
> La pista: si algo no aparece, compara letra por letra con lo que aprendimos en la lección de imágenes. Las computadoras son muy literales: una letra fuera de lugar y ya no entienden. Lo corrijo: "src". ¡La foto volvió!

---

## Escena 5 — Error 3: falta el punto y coma (3:40–4:45)

**En pantalla:** la regla `.descripcion` con dos propiedades. Borra el `;` después de `#6c5ce7`. Resalta que el párrafo vuelve a ser negro y pequeño. Vuelve a poner el `;`.
**Texto en pantalla:** "Error 3 · Falta el punto y coma `;`" → "Cada propiedad termina con `;`"

> Error número tres, el favorito de los principiantes: olvidar el punto y coma en CSS. Tengo dos propiedades: color morado y tamaño de letra de veinte píxeles. Si borro el punto y coma de la primera… [borrar] mira: el párrafo volvió a letra negra y pequeña.
>
> Y fíjate en algo curioso: se perdieron las dos propiedades, no solo una. Eso pasa porque el punto y coma es la señal que le dice al navegador "aquí termina esta instrucción". Sin esa señal, junta las dos líneas en una sola frase que no tiene sentido, y la ignora completa.
>
> La solución: ponerlo de vuelta. [escribir `;`] La regla fácil: cada propiedad termina con punto y coma. Siempre.

---

## Escena 6 — Error 4: comilla sin cerrar (4:45–5:35)

**En pantalla:** la línea `<p class="descripcion">`. Borra la comilla de cierre. Muestra que desaparecen el párrafo y el título. Vuelve a poner la comilla.
**Texto en pantalla:** "Error 4 · Comilla sin cerrar" → "Una comilla abre, otra cierra"

> Error número cuatro: una comilla que no se cierra. Los valores de los atributos, como el nombre de una clase, van entre comillas: una al abrir y otra al cerrar.
>
> Si borro la comilla final… [borrar] mira: desaparecieron el párrafo y también el título. El navegador sigue buscando la comilla que cierra, y se "come" todo el código que encuentra por el camino.
>
> Por eso, cuando una parte de tu página desaparece sin explicación, busca comillas que falten. En el editor te ayuda el color: el texto entre comillas tiene un color distinto, y si de pronto cambia el color de todo lo de abajo, ahí está la pista.
>
> Vuelvo a poner la comilla… y todo regresa.

---

## Escena 7 — Error 5: el estilo no se aplica (5:35–6:15)

**En pantalla:** en el CSS, cambia `.tarjeta` por `tarjeta`. La tarjeta pierde su fondo blanco y su forma. Luego ponle el punto y muestra la variante `class="Tarjeta"` con mayúscula.
**Texto en pantalla:** "Error 5 · El estilo no se aplica" → "`.tarjeta` lleva punto" · "Mayúsculas ≠ minúsculas"

> Error número cinco: el estilo existe, pero no se aplica. Mira: escribí la regla de la tarjeta, pero le quité el punto. [mostrar]
>
> En CSS, para elegir algo por su clase, el nombre empieza con un punto. Sin punto, el navegador busca una etiqueta llamada "tarjeta", que no existe, y no le da estilo a nada.
>
> Otro detalle: las mayúsculas importan. "Tarjeta" con te mayúscula no es lo mismo que "tarjeta" con te minúscula.
>
> Si tu estilo no se aplica, compara el nombre en el HTML con el nombre en el CSS, letra por letra, y fíjate en el punto. Arreglado.

---

## Escena 8 — Reto "Encuentra el error" (6:15–8:30)

**En pantalla:** primero el resultado final correcto (tarjeta amarilla con foto, frase y botón). Luego la página con errores y su código. Durante la pausa, una tarjeta con una **cuenta regresiva de 60 s** y el texto "Pausa el video".
**Texto en pantalla:** "Reto: 3 errores escondidos" · "Pausa el video · 1 minuto" · en la solución, marca cada línea con un círculo.
**Enlace:** el enlace al CodePen del reto va en la descripción del video, y el mismo código en `/starter-files` del repositorio.

### Código del reto
```html
<div class="tarjeta">
  <h1>Mi página de perfil</h1>
  <p>Soy estudiante y me gusta dibujar.</p>
  <img scr="https://picsum.photos/id/1025/200/200" alt="Mi dibujo" width="200">
  <p class="aviso>Gracias por visitar mi página.</p>
  <a class="boton" href="https://es.wikipedia.org">Visitar Wikipedia</a>
</div>
```
```css
.tarjeta {
  background-color: lightyellow
  padding: 20px;
  border-radius: 12px;
  border: 2px solid orange;
  text-align: center;
}

.boton {
  color: darkgreen;
}
```
**Errores escondidos:** `scr` en lugar de `src` · la comilla sin cerrar en `class="aviso>` · falta el `;` después de `lightyellow`.
**Lo que se ve con errores:** no aparece la foto; falta la frase "Gracias por visitar mi página" y el enlace queda como texto normal; la tarjeta no es amarilla y no tiene espacio interior.

> ¡Ahora es tu turno! Te toca ser detective. En la descripción de este video hay un enlace a una página con tres errores escondidos: dos en el HTML y uno en el CSS. Tu misión es encontrarlos y arreglarlos hasta que la tarjeta se vea así. [mostrar el resultado final]
>
> Recuerda los tres pasos: mira, busca la pista y cambia una sola cosa a la vez.
>
> Pausa el video ahora. Tienes un minuto. [cuenta regresiva de 60 segundos, sin voz]
>
> ¡Se acabó el tiempo! Veamos juntos.
>
> Primer error: la imagen no aparece. Mira la palabra "scr": está con las letras cambiadas. Debe decir "src".
>
> Segundo error: falta una frase y el enlace ya no se ve como enlace. La pista es la comilla de "aviso": nunca se cerró, y se tragó lo que venía después.
>
> Tercer error, en el CSS: la tarjeta perdió el color amarillo y el espacio interior. Falta el punto y coma después de "lightyellow".
>
> ¿Encontraste los tres? ¡Excelente! Y si encontraste uno o dos, también estás aprendiendo. Eso es depurar.

---

## Escena 9 — Cierre y próximos pasos (8:30–10:00)

**En pantalla (en este orden):**
1. Lista animada de lo aprendido (15 s).
2. El repositorio del curso en GitHub, solo la guía de depuración abierta (≈ 15 s). **No demuestres código ahí;** solo muestra el documento.
3. Texto con el nombre del recurso: "MDN Web Docs (en español)".
4. Pantalla final: "¡Comparte tu página!" y los enlaces de la descripción.
**Texto en pantalla:** "HTML: estructura, listas, imágenes, enlaces" · "CSS: colores, fuentes, bordes" · "Tu página de perfil" · "Depurar".

> Llegamos al final del curso. Mira todo lo que lograste. Aprendiste qué es una página web y cómo está hecha. Escribiste tu primera estructura con HTML. Agregaste listas, imágenes y enlaces. Le diste color y estilo con CSS. Construiste tu propia página de perfil. Y hoy aprendiste algo que hasta los profesionales hacen todos los días: depurar.
>
> Para que no lo olvides, preparamos una guía de depuración con los cinco errores de este video: qué se ve en pantalla cuando ocurren y cómo arreglarlos. La encuentras en el repositorio del curso; el enlace está en la descripción. Allí también hay enlaces útiles para seguir aprendiendo.
>
> Mi recomendación principal es MDN Web Docs: tiene explicaciones gratuitas y una versión en español.
>
> Y si quieres seguir practicando, prueba cosas nuevas: cambia colores, agrega otra sección, equivócate a propósito y arréglalo. Así se aprende.
>
> Si te quedó una página que te gusta, compártela con tu familia y tus amigos; seguro les va a encantar. Gracias por acompañarnos en este curso. ¡Nos vemos en tu próxima página web!
