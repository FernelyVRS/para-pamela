# Para Pamela — página de aniversario

Sitio estático preparado para publicarse con GitHub Pages. La versión que se publica está dentro de `dist/`.

## Personalizar las fotografías

1. Guarda seis fotografías dentro de `dist/assets/images/` con estos nombres:
   - `foto-1.jpg`
   - `foto-2.jpg`
   - `foto-3.jpg`
   - `foto-4.jpg`
   - `foto-5.jpg`
   - `foto-6.jpg`
2. En `dist/index.html`, sustituye cada bloque `<div class="photo-placeholder">...</div>` por:

```html
<img src="assets/images/foto-1.jpg" alt="Descripción breve del momento" />
```

3. Agrega esta regla al final de `dist/styles.css`:

```css
.polaroid img {
  display: block;
  width: 100%;
  aspect-ratio: 4 / 5;
  object-fit: cover;
}
```

## Personalizar la carta

Busca `Mi querida Pamela:` en `dist/index.html` y reemplaza los tres párrafos con Lorem ipsum por tu carta.

## Agregar la canción

Coloca un archivo MP3 dentro de `dist/assets/audio/`, por ejemplo `nuestra-cancion.mp3`. Luego abre `dist/script.js` y cambia:

```js
musicUrl: "",
```

por:

```js
musicUrl: "assets/audio/nuestra-cancion.mp3",
```

También puedes cambiar el texto de `musicLabel` por el nombre de la canción.

## Frases iniciales alternativas

- Pamela, tengo algo que mi corazón lleva tiempo queriendo decirte.
- Para ti, que convertiste un año en una colección de momentos inolvidables.
- Todo comenzó un 5 de septiembre, y desde entonces mi vida tiene más motivos para sonreír.
- Pamela, esta es una pequeña forma de guardar todo lo bonito que hemos vivido.
- Un año, cientos de recuerdos y la misma elección: tú.

## Mensajes finales alternativos

- Elegirte aquel día fue hermoso; seguir eligiéndote cada día es aún mejor.
- Gracias por hacer de este año una historia que quiero seguir escribiendo contigo.
- Que este sea el primero de muchos aniversarios, aventuras y sueños compartidos.
- Si pudiera volver al comienzo, te elegiría otra vez, sin cambiar nada.
- Lo mejor de nuestro primer año es saber que todavía nos queda toda una vida por descubrir.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub.
2. Sube todo el contenido de esta carpeta, incluyendo `.github` y `dist`.
3. En el repositorio abre **Settings → Pages**.
4. En **Build and deployment**, selecciona **GitHub Actions**.
5. La acción incluida publicará automáticamente el contenido de `dist`.
6. Cuando finalice, GitHub mostrará una dirección similar a `https://usuario.github.io/nombre-del-repositorio/`.

Cada cambio que envíes a la rama `main` volverá a publicar la página automáticamente.
