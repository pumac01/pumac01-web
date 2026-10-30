# PUMAC-01 — Handoff para Codex

## Objetivo
Continuar el desarrollo del sitio web de PUMAC-01 y dejarlo listo para producción sin perder la identidad visual ni el propósito social del proyecto.

## Qué es PUMAC-01
PUMAC-01 significa **Puesto Unificado Móvil Autónomo de Comunicaciones**.

Es un proyecto desarrollado por el radioaficionado **Ignacio García — CD3IUG**. Consiste en una estación portátil de comunicaciones, transportable en mochila, de bajo costo y rápido despliegue. Puede complementarse con radios portátiles, baterías, panel solar, linterna y otros elementos de apoyo.

Su propósito principal es ayudar a conectar personas y comunidades aisladas o en zonas de difícil acceso con autoridades, centros de salud, equipos de emergencia o familiares, especialmente ante terremotos, incendios forestales y otras emergencias.

El proyecto tiene una orientación social y filantrópica. La intención de Ignacio es poner el desarrollo gratuitamente a disposición de una Fundación u organización que pueda evaluar su utilidad y eventualmente fabricar unidades para ser donadas a comunidades, juntas de vecinos, Bomberos u otros equipos de emergencia.

## Propietario / autor del proyecto
- Ignacio García
- Indicativo: **CD3IUG**
- Proyecto: PUMAC-01

El indicativo CD3IUG debe mantenerse visible en la web, pero sin repetirse de forma excesiva. Actualmente aparece en portada, propósito y contacto.

## Estado actual
El sitio es estático y no requiere framework ni proceso de compilación.

Archivos principales:
- `index.html`
- `styles.css`
- `script.js`
- `assets/logo-pumac01.png`
- `assets/equipo-pumac01.png`

La versión actual ya incluye:
- Hero principal.
- Descripción del proyecto.
- Cómo funciona.
- Aplicaciones reales.
- Propósito social.
- Galería.
- Sección de contacto.
- Diseño responsive.
- Menú móvil.
- Indicativo CD3IUG.
- Corrección para que el logo PUMAC-01 se vea completo en la galería mediante `object-fit: contain`.

## Dirección visual
La web debe reflejar el lenguaje del logo PUMAC-01:
- montaña / terreno / Chile;
- comunicaciones;
- autonomía;
- seguridad;
- trabajo en terreno;
- ayuda a comunidades;
- estética outdoor y técnica, pero humana.

Paleta actual:
- azul marino / azul profundo;
- amarillo dorado;
- blanco / crema;
- tonos oscuros complementarios.

Evitar:
- estética corporativa genérica;
- exceso de efectos o animaciones;
- aspecto de landing page comercial de producto;
- saturar con iconos o texto técnico;
- cambiar el logo;
- convertir a Ignacio en el protagonista visual principal.

El protagonista debe ser **el propósito del proyecto y las personas a las que puede ayudar**.

## Mensajes clave que deben conservarse
Conceptos principales:
- **Comunicación donde más se necesita.**
- **Conectando comunidades.**
- **Tecnología al servicio de las personas.**

PUMAC-01 no debe presentarse como un producto comercial.
Debe mostrarse como un desarrollo de radioaficionados con propósito social.

## Fotografías
`assets/equipo-pumac01.png` es la fotografía elegida del prototipo y no muestra la mano de la persona.

No sustituirla por una imagen generada si no existe una necesidad concreta.
Las fotografías reales del prototipo tienen prioridad porque aportan credibilidad.

## Cambios recomendados antes de producción
Codex puede mejorar libremente implementación, accesibilidad y calidad visual, pero debe preservar contenido, mensaje y estética general.

Prioridades:

1. Revisar responsive en:
   - 360 px
   - 390 px
   - 430 px
   - 768 px
   - 1024 px
   - 1440 px

2. Revisar especialmente:
   - hero;
   - navegación móvil;
   - galería;
   - tamaños del logo;
   - tarjetas de aplicaciones;
   - footer.

3. Mejorar accesibilidad:
   - contraste;
   - foco visible;
   - navegación mediante teclado;
   - atributos ARIA cuando correspondan;
   - textos alternativos de imágenes.

4. Optimización:
   - comprimir imágenes si es posible sin degradación visible;
   - definir dimensiones de imágenes para reducir CLS;
   - revisar carga inicial;
   - evitar librerías externas innecesarias.

5. SEO básico:
   - title y description ya existen;
   - agregar Open Graph;
   - agregar favicon si se dispone de uno;
   - canonical solo cuando exista dominio definitivo;
   - robots.txt / sitemap.xml solo cuando se conozca dominio final.

6. Contacto:
   Actualmente el botón contiene `href="mailto:"`.
   NO inventar un correo.
   Mantenerlo inactivo o reemplazarlo solo cuando el usuario entregue una dirección real.

7. Seguridad / privacidad:
   - no agregar trackers, formularios de terceros ni analytics sin autorización;
   - no publicar información personal adicional de Ignacio sin aprobación.

## Producción
Por ahora el sitio puede desplegarse como hosting estático.

Opciones válidas:
- Cloudflare Pages
- GitHub Pages
- Netlify
- hosting web tradicional

Preferir un despliegue estático simple.

Antes de publicar:
- no dejar rutas locales;
- comprobar que todos los assets usen rutas relativas correctas;
- verificar que no existan links vacíos salvo el correo pendiente documentado;
- revisar consola del navegador;
- probar navegación móvil;
- ejecutar Lighthouse si está disponible;
- verificar HTTP 200 para `/`, CSS, JS e imágenes;
- probar recarga directa de la página;
- configurar HTTPS y dominio definitivo.

## Criterio para considerar la web lista
La web está lista para producción cuando:
- no hay errores visibles ni de consola;
- funciona correctamente en móvil y escritorio;
- el logo PUMAC-01 nunca aparece cortado;
- CD3IUG aparece correctamente escrito;
- el propósito social queda claro en los primeros segundos de lectura;
- las fotografías reales se ven nítidas;
- el sitio carga rápido;
- no existen datos de contacto inventados;
- el despliegue se puede repetir fácilmente.

## Instrucción de trabajo para Codex
Antes de hacer cambios grandes, inspecciona el sitio actual completo.
No rediseñes desde cero salvo que haya un problema técnico real.
Haz mejoras incrementales, prueba visualmente después de cada grupo de cambios y conserva la personalidad actual del proyecto.

Al terminar, entrega:
1. resumen de cambios;
2. archivos modificados;
3. problemas pendientes;
4. instrucciones exactas de despliegue;
5. URL de producción, si el entorno permite hacer el despliegue.
