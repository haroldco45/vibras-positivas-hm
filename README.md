# vibraspositivashm.com — Casa madre de Vibras Positivas HM

PWA bilingüe (ES/EN) para promocionar y vender los servicios de Vibras Positivas HM, con el portafolio vivo de apps hechas para empresas.

## Archivos
| Archivo | Qué es |
|---|---|
| `index.html` | Toda la página (estilos y código adentro) |
| `manifest.json` | Para que se instale como app |
| `sw.js` | Service worker (funciona sin internet) |
| `icon-192.png`, `icon-512.png` | Ícono de la app instalada |
| `og-vibras.jpg` | Imagen de vista previa al compartir el enlace (1200×630) |
| `media/hero.mp4`, `media/hero-poster.jpg` | Video de portada hecho con fotos reales de las apps |

## Subir a Hostinger
1. Administrador de archivos → `public_html`.
2. Haz copia del `index.html` viejo (renómbralo `index-viejo.html`).
3. Sube los archivos de arriba a `public_html` y crea la carpeta `media` con sus 2 archivos.
4. No borres `IMG-20260323-WA0005.jpg` si otras páginas lo usan.

## Agregar una app nueva al portafolio
En `index.html`, busca `const APPS = [` y copia una línea:
```js
{n:'Nombre', c:'comida', es:'Descripción', en:'Description', u:'https://app.netlify.app/', i:'https://app.netlify.app/og.jpg'},
```
Categorías: `comida`, `belleza`, `comercio`, `educacion`, `turismo`, `autos`, `empresas`.
La foto (`i`) es la imagen de vista previa que ya tiene cada app. Si una app se pausa, su tarjeta muestra el nombre sobre los colores de la marca.

Después de cada cambio, sube la versión en `sw.js` (`const V = ...`) para que los celulares vean lo nuevo.

---
Desarrollada por Vibras Positivas HM — Derechos de Autor Reservados
