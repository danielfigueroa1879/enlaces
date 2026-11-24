# enla.netlify.app — Enlaces con vista previa para WhatsApp

Oficina de Seguridad Privada O.S.10 Coquimbo

## Estructura
- `img/`  imágenes de vista previa (1200x630, JPG, menos de 300 KB)
- `docs/` PDF o archivos que se abren al tocar el enlace
- `plantilla.html` base para cada respuesta nueva
- `prueba.html` página de prueba

## Agregar una respuesta nueva
1. Sube el PDF a `docs/` (ej: `docs/requisitos.pdf`)
2. Sube la imagen a `img/` (ej: `img/requisitos.jpg`)
3. Copia `plantilla.html` como `requisitos.html` y reemplaza TITULO, IMAGEN, NOMBRE-PAGINA y ARCHIVO
4. Commit + push, y Netlify publica solo
5. En AutoResponder pega: `https://enla.netlify.app/requisitos.html`

## Notas
- Nombres de archivo sin espacios, tildes ni ñ
- El enlace debe ser el PRIMER link del mensaje (solo el primero genera vista previa)
- WhatsApp guarda en caché la vista previa: si cambias la imagen, cámbiale el nombre

## Páginas generadas (44)
Ver la lista completa en https://enla.netlify.app/ (index.html).
Cada página `X.html` usa la imagen `img/X.jpg` y redirige al documento original.
