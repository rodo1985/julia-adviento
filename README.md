# Calendario de Adviento de Julia

Un calendario de Adviento inventado por Julia: 24 puertas, cielo gris arriba y suelo dorado abajo, y la historia de Drácula (¡con corona!), la Momia, la Chica Guerrera, Mira y la Bruja que los mete en la gavia.

**Versión 2: ¡personajes de chocolate!** Todos los personajes (Drácula, la Momia, la Chica Guerrera, la Bruja y Mira), en las 24 escenas, en las puertas y en la cabecera, están hechos de chocolate: chocolate con leche, chocolate negro y chocolate blanco, con brillo y bordes de molde. La corona de Drácula sigue siendo dorada, como de papel de aluminio. La historia, las puertas y los colores del calendario son los mismos que en la versión 1 (que sigue en el historial de git).

**En vivo:** https://adviento.sergioredondocabanillas.com

## Cómo está hecho
- `index.html`: toda la app en un único archivo (HTML, CSS, JS y dibujos SVG), sin dependencias externas.
- Publicado como un Cloudflare Worker (`julia-adviento`) que sirve ese HTML, con el dominio propio `adviento.sergioredondocabanillas.com`.
- `cloudflare/worker.js`: el Worker generado (el HTML incrustado). `cloudflare/deploy.js`: el script usado para subirlo con la API de Cloudflare.
