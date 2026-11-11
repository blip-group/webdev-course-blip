# Guía de depuración: ¡mi código no funciona!

**Depurar** es buscar y arreglar errores en tu código. A todo el mundo le pasa, incluso a quienes programan desde hace años. Un error no significa que lo hiciste mal: significa que la computadora te está pidiendo una pista.

## El método de 3 pasos

1. **Mira.** ¿Qué esperabas ver y qué estás viendo? Compararlo te dice dónde está el problema.
2. **Busca la pista.** Casi siempre es algo pequeño: una etiqueta que falta, una comilla, un punto y coma o una letra mal escrita.
3. **Cambia una sola cosa** y vuelve a ejecutar. Si cambias cinco cosas a la vez, no sabrás cuál arregló el problema.

## Los 5 errores más comunes

| # | Error | Qué se ve en pantalla | Cómo arreglarlo |
|---|---|---|---|
| 1 | Etiqueta sin cerrar | Lo que sigue se ve con el estilo de la etiqueta abierta (por ejemplo, con letra de título) | Escribe la etiqueta de cierre |
| 2 | Nombre mal escrito | Algo no aparece, como una imagen | Compara letra por letra |
| 3 | Falta el punto y coma en CSS | Se pierden **las dos** propiedades, la anterior y la siguiente | Termina cada propiedad con `;` |
| 4 | Comilla sin cerrar | Desaparece una parte de la página | Abre y cierra siempre las comillas |
| 5 | Selector mal escrito | El estilo no se aplica | Revisa el punto y las mayúsculas |

### Error 1 · Etiqueta sin cerrar

Si olvidas cerrar una etiqueta, el navegador cree que todo lo que escribes después sigue dentro de ella.

```html
<!-- ❌ Falta </h2>: la lista y el botón se ven con letra de título -->
<h2>Mis cosas favoritas
<ul>
  <li>Dibujar</li>
</ul>

<!-- ✅ Con la etiqueta de cierre -->
<h2>Mis cosas favoritas</h2>
<ul>
  <li>Dibujar</li>
</ul>
```

**Pista:** si de pronto todo lo que sigue cambia de tamaño o de estilo, revisa si olvidaste cerrar algo antes.

### Error 2 · Nombre mal escrito

Las computadoras son muy literales: una letra fuera de lugar y ya no entienden. El navegador no te avisa con un cartel rojo; simplemente sigue de largo.

```html
<!-- ❌ "scr" en lugar de "src": la imagen no aparece -->
<img scr="https://picsum.photos/id/1025/200/200" alt="Mi dibujo">

<!-- ✅ -->
<img src="https://picsum.photos/id/1025/200/200" alt="Mi dibujo">
```

**Pista:** si algo no aparece, compara letra por letra con el ejemplo de la lección.

### Error 3 · Falta el punto y coma

El punto y coma le dice al navegador «aquí termina esta instrucción». Sin él, junta dos líneas en una sola frase sin sentido y las ignora **las dos**.

```css
/* ❌ Falta el ; después del color: se pierden el color y el tamaño */
.descripcion {
  color: #6c5ce7
  font-size: 20px;
}

/* ✅ */
.descripcion {
  color: #6c5ce7;
  font-size: 20px;
}
```

**Regla fácil:** cada propiedad termina con punto y coma.

### Error 4 · Comilla sin cerrar

Los valores de los atributos van entre comillas: una al abrir y otra al cerrar. Si falta la de cierre, el navegador sigue buscándola y se «come» el código que encuentra por el camino.

```html
<!-- ❌ Falta la comilla final: desaparecen el párrafo y el título que siguen -->
<p class="descripcion>Soy estudiante y me gusta dibujar.</p>

<!-- ✅ -->
<p class="descripcion">Soy estudiante y me gusta dibujar.</p>
```

**Pista:** en el editor, el texto entre comillas tiene otro color. Si de pronto cambia el color de todo lo de abajo, ahí falta una comilla.

### Error 5 · Selector mal escrito

En CSS, para elegir algo por su clase, el nombre empieza con un punto. Además, las mayúsculas importan.

```css
/* ❌ Sin punto: el navegador busca una etiqueta llamada "tarjeta", que no existe */
tarjeta {
  background-color: white;
}

/* ✅ */
.tarjeta {
  background-color: white;
}
```

```html
<!-- ❌ "Tarjeta" con T mayúscula no es lo mismo que "tarjeta" -->
<main class="Tarjeta">

<!-- ✅ -->
<main class="tarjeta">
```

**Pista:** compara el nombre en el HTML con el nombre en el CSS, letra por letra, y fíjate en el punto.

## Reto «Encuentra el error»

Hay una página con **3 errores escondidos** (2 en el HTML y 1 en el CSS).

- Punto de partida: [`starter-files/leccion-6/reto-encuentra-el-error`](starter-files/leccion-6/reto-encuentra-el-error)
- Solución: [`completed-examples/leccion-6/reto-corregido`](completed-examples/leccion-6/reto-corregido)

Intenta resolverlo tú primero y revisa la solución después.

## Lista de revisión rápida

- [ ] ¿Cerré todas las etiquetas?
- [ ] ¿Escribí bien cada nombre, letra por letra?
- [ ] ¿Cada propiedad de CSS termina con `;`?
- [ ] ¿Cada comilla que abrí tiene su comilla de cierre?
- [ ] ¿El nombre de la clase es igual en el HTML y en el CSS (con el punto y las mayúsculas)?
- [ ] ¿Cambié solo una cosa antes de volver a ejecutar?

## Para seguir aprendiendo

- [MDN Web Docs en español](https://developer.mozilla.org/es/): explicaciones gratuitas de HTML y CSS.
- Vuelve a abrir tus prácticas, cambia colores, agrega otra sección, equivócate a propósito y arréglalo. Así se aprende.
