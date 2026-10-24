# Calendario de Adviento de Julia

Un calendario de Adviento inventado por Julia: 24 puertas, cielo gris arriba y suelo dorado abajo, y la historia de Drácula (¡con corona!), la Momia, la Chica Guerrera, Mira y la Bruja que los mete en la gavia.

**En vivo:** https://adviento.sergioredondocabanillas.com

## Cómo está hecho
- `index.html`: toda la app en un único archivo (HTML, CSS, JS y dibujos SVG), sin dependencias externas.
- Publicado como un Cloudflare Worker (`julia-adviento`) que sirve ese HTML, con el dominio propio `adviento.sergioredondocabanillas.com`.
- `cloudflare/worker.js`: el Worker generado (el HTML incrustado). `cloudflare/deploy.js`: el script usado para subirlo con la API de Cloudflare.
