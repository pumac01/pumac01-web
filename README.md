# PUMAC-01

Sitio estático de **PUMAC-01 — Puesto Unificado Móvil Autónomo de Comunicaciones**, proyecto impulsado por Ignacio García (**CD3IUF**).

**Sitio publicado:** https://pumac.cl/

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

El repositorio `pumac01/pumac01-web` ya está configurado para publicar desde la rama `main`, carpeta `/ (root)`. Para actualizar el sitio, subir los archivos modificados a esa rama; GitHub Pages volverá a publicar. Después, abrir la URL anterior y comprobar los cambios.

El dominio propio `pumac.cl` está configurado en GitHub Pages y tiene activada la opción **Enforce HTTPS**. La URL canonical y los metadatos sociales de `index.html` usan ese dominio.

## Dominio y DNS

El dominio está registrado en NIC Chile. Sus servidores DNS son `titan.ns.cloudflare.com` y `vera.ns.cloudflare.com`, administrados en la cuenta Cloudflare de PUMAC. Para que el sitio siga publicado:

- Mantener los cuatro registros `A` de `pumac.cl` hacia `185.199.108.153`, `185.199.109.153`, `185.199.110.153` y `185.199.111.153`, todos como **DNS only**.
- Mantener `www` como `CNAME` hacia `pumac01.github.io`, con el proxy de Cloudflare **activado**. La regla de Cloudflare `Redirigir www a pumac.cl con HTTPS` envía `http://www.pumac.cl` y `https://www.pumac.cl` a `https://pumac.cl`, conservando ruta y parámetros.
- Mantener el registro `TXT` `_github-pages-challenge-pumac01.pumac.cl`, que verifica el dominio en la cuenta GitHub `pumac01`.
- Mantener el archivo `CNAME` con `pumac.cl` en la raíz del repositorio.

Después de modificar DNS o Pages, comprobar que `https://pumac.cl/` carga sin advertencias y que las variantes HTTP y `www` redirigen a esa URL.

## Contacto

El botón de contacto usa la dirección verificada del proyecto: `contactopumac01@gmail.com`.
