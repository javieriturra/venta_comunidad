# Venta — artículos para la comunidad

Sitio estático, sin dependencias ni build step. Funciona localmente y en GitHub Pages.

## Personalizar
- Abre `index.html` y cambia el texto de contacto (`[WhatsApp / teléfono / mensaje]`).
- Los artículos se encuentran en el array `products` dentro de `index.html`.
- Cada producto admite una foto principal y varias fotos secundarias.
- La foto principal se define en `mainImage`; las secundarias, en el arreglo `secondaryImages` del producto correspondiente.
- Guarda los JPG en `fotos/`. Ejemplo: `mainImage: "fotos/producto-01.jpg"` y `secondaryImages: ["fotos/producto-01-detalle-1.jpg", "fotos/producto-01-detalle-2.jpg"]`.
- Las fotos secundarias aparecen como miniaturas; al pulsarlas, cambian la foto principal de la tarjeta.
- Si no hay foto principal, se mostrará “Foto principal por agregar”.
- Los artículos marcados `No ahora` en la hoja `Venta` del Excel se excluyeron.
- El botón **Exportar a PDF / Imprimir** abre el diálogo de impresión del navegador. Elige “Guardar como PDF”. Para exportar todo, deja vacía la búsqueda.

## Publicar en GitHub Pages
1. Crea un repositorio y sube `index.html`, `README.md` y la carpeta `fotos/`.
2. En GitHub: **Settings → Pages**.
3. En “Build and deployment”, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
4. Guarda y espera la URL que entrega GitHub Pages.

No necesita Node, frameworks ni backend.
