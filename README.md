# PUMAC-01

Sitio estático de **PUMAC-01 — Puesto Unificado Móvil Autónomo de Comunicaciones**, proyecto impulsado por Ignacio García (**CD3IUF**).

## Abrir localmente

Desde esta carpeta, ejecutar un servidor HTTP estático (por ejemplo `npx serve .`) y abrir la URL local indicada. No requiere compilación ni dependencias del sitio.

## Archivos

- `index.html`: contenido y metadatos.
- `styles.css`: diseño responsive.
- `script.js`: menú móvil.
- `assets/logo-pumac01-transparente.png`: logo original con el exterior transparente, usado por el sitio.
- `assets/logo-pumac01.png`: logo original intacto.
- `assets/equipo-pumac01.png`: foto del prototipo.

## Publicar con GitHub Pages

1. Crear la cuenta de GitHub del proyecto y un repositorio público llamado `pumac01-web`.
2. Subir **el contenido de esta carpeta** a la rama `main`, con `index.html` en la raíz del repositorio.
3. En el repositorio, abrir **Settings → Pages**. En **Build and deployment**, elegir **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guardar.
4. Esperar la URL que GitHub Pages muestre en esa misma pantalla y abrirla para verificar el sitio. GitHub Pages sirve HTTPS en su dominio estándar.
5. Para cada actualización, subir los archivos modificados a `main`; Pages volverá a publicar.

Si se usa un dominio propio, configurar primero ese dominio en Pages; entonces añadir una URL canonical y generar `robots.txt` y `sitemap.xml` con el dominio definitivo.

## Contacto

El botón de contacto usa la dirección verificada del proyecto: `contactopumac01@gmail.com`.
