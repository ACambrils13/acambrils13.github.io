# Entre páginas — sitio Jekyll para GitHub Pages

Plantilla inicial en español para llevar un diario de lecturas.

## Páginas incluidas

- `index.md`: portada.
- `leidos.md`: libros terminados.
- `por-leer.md`: lista de próximas lecturas.
- `resenas.md`: índice automático de reseñas.
- `archivo.md`: archivo cronológico.
- `sobre-mi.md`: presentación del proyecto.

También incluye estilos propios, configuración Jekyll, `Gemfile` y una plantilla para crear reseñas.

## Publicarlo en GitHub Pages

1. Crea un repositorio llamado `TU_USUARIO.github.io` (o uno normal si prefieres una URL de proyecto).
2. Descomprime estos archivos y sube el contenido a la raíz del repositorio.
3. En GitHub, entra en **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarda y espera a que termine la publicación.

Si el repositorio no se llama `TU_USUARIO.github.io`, configura `baseurl` en `_config.yml` con el nombre del repositorio, por ejemplo `baseurl: "/mi-bitacora"`.

## Añadir una reseña

1. Copia `PLANTILLA_RESEÑA.md`.
2. Crea un archivo dentro de `_posts` con este formato: `AAAA-MM-DD-titulo-del-libro.md`.
3. Completa el front matter (título y fecha) y escribe tu reseña.
4. Haz commit y push. La reseña aparecerá en **Reseñas** y **Archivo**.

Para que Jekyll publique una entrada, el archivo debe estar dentro de `_posts` y empezar por la fecha `AAAA-MM-DD-`.

## Personalización rápida

- Cambia `title` y `description` en `_config.yml`.
- Edita el texto de `index.md` y `sobre-mi.md`.
- Sustituye las filas de ejemplo en `leidos.md` y los elementos de `por-leer.md`.
- Modifica los colores en `assets/css/style.scss` (variables `--green`, `--paper` y `--accent`).

La plantilla no inventa reseñas ni libros: los ejemplos están señalados para que los sustituyas por tus lecturas reales.
