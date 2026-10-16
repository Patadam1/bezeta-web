# BEZETA Barberstudio — web

Web de una sola página para BEZETA Barberstudio (Carrer de la Font 23, 17200 Palafrugell).

## Cambiar los datos

Todos los datos de la barbería (Booksy, dirección, horario, redes, teléfono) están en un solo sitio:
el bloque `const BEZETA = { ... }` al final de `index.html`. Cambia el valor entre comillas y la web se actualiza sola.

## Fotos de la galería

Pon las fotos en `assets/fotos/` y sustituye cada `<figure class="shot" data-ph>…</figure>` de la sección "El trabajo" por:

```html
<figure class="shot"><img src="assets/fotos/corte-1.jpg" alt="Descripción del corte"></figure>
```

## Publicar

GitHub Pages: Settings → Pages → Branch `main`, carpeta `/ (root)`.

## Diseño

- `DESIGN.md` y `.impeccable/design.json`: sistema de diseño (solo blanco y negro, rayas a −39,3°, Archivo + Bodoni Moda).
- `PRODUCT.md`: qué es la web y para quién.
