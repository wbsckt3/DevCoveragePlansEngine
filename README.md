# DevCoveragePlansEngine

Hub de **cobertura de desarrollo** de white labels P2L para GitHub Pages.

- Repo: [wbsckt3/DevCoveragePlansEngine](https://github.com/wbsckt3/DevCoveragePlansEngine)
- Site: [wbsckt3.github.io/DevCoveragePlansEngine](https://wbsckt3.github.io/DevCoveragePlansEngine/)
- Dinámica ES/EN (i18next + `p2l-locale`) igual que `docs/gh-pages-tuki`
- Cada botón del hero **cambia el modo** (toggle de contenido); el CTA del encabezado abre la carpeta de arquitectura del white label activo

## White labels actuales

| Modo | Panel hub | Arquitectura (visor PDF) | Producto |
|------|-----------|--------------------------|----------|
| SEO Coverage | `data-mode="seo"` | [`gh-pages-seo-coverage/`](./gh-pages-seo-coverage/) | `/login/seo-coverage-dashboard` |
| WPF Dashboard | `data-mode="wpf"` | [`gh-pages-wpf-dashboard-coverage/`](./gh-pages-wpf-dashboard-coverage/) | `/login/dashboard-wpf` |
| RPA IndiGO | `data-mode="indigo"` | [`gh-pages-rpa-indigo-coverage/`](./gh-pages-rpa-indigo-coverage/) | Informe + plan (sin login producto) |

## Estructura

| Ruta | Rol |
|------|-----|
| `index.html` | Hub DevCoveragePlansEngine |
| `locales/` + `scripts/` | i18n embebido |
| `gh-pages-seo-coverage/` | Visor PDF + `*.plan.md` **SEO Coverage** |
| `gh-pages-wpf-dashboard-coverage/` | Visor PDF + `*.plan.md` **WPF Dashboard** |
| `gh-pages-rpa-indigo-coverage/` | Visor PDF + informe/plan **RPA IndiGO → agente IA** |

## Cómo publicar en gh-pages

Publica el contenido de **esta carpeta** (incluyendo ambas subcarpetas de planes) en la raíz de la rama `gh-pages`.

No subir `wbsckt3-github-repos-settings` ni `*.txt` de notas locales.

## Agregar otro white label

1. Crea carpeta hermana con visor + `*.plan.md` (mismo esquema que las carpetas existentes).
2. Añade un botón `data-mode="..."` en el hero y un panel `.mode-panel`.
3. Extiende `MODE_META` / `WHITE_LABEL_LINKS` en `index.html`.
4. Extiende `locales/es.json` / `en.json` y regenera `scripts/locales-embed.js`.
