# WPF Dashboard — GitHub Pages (cobertura)

Carpeta hermana de `gh-pages-seo-coverage` dentro de DevCoveragePlansEngine.

- Hub: https://wbsckt3.github.io/DevCoveragePlansEngine/
- Visor: https://wbsckt3.github.io/DevCoveragePlansEngine/gh-pages-wpf-dashboard-coverage/
- Repo: https://github.com/wbsckt3/DevCoveragePlansEngine (rama `gh-pages`)

## Contenido

| Archivo | Descripción |
|---------|-------------|
| `index.html` | Visor Markdown → vista tipo PDF |
| `GUIA_INSTALACION.md` | Manual de instalación del cliente .NET AvlMonitor (Windows, .NET 8, SQL, Waze) |
| `wpf_dashboard_dinamica_usuario.plan.md` | Flujo admin en `CompanyWpfDashboardView` |
| `wpf_dashboard_epayco_wallet.plan.md` | Planes + wallet ePayco tenant `p2l-wpf` |
| `wpf_desktop_avlmonitor_licencia.plan.md` | Cliente .NET AvlMonitor + `.env` / licencia |

> El dashboard web ofrece la **guía gratis** y, tras ePayco, la **descarga ZIP** de AvlMonitor.
> DevCoveragePlansEngine **no** incluye el `.zip`: solo documenta la dinámica (ver `wpf_producto_digital_avlmonitor.plan.md`).

## Cómo publicar

Publica esta carpeta como subcarpeta de la rama `gh-pages` del repo DevCoveragePlansEngine (junto al hub y a `gh-pages-seo-coverage/`).

Los nuevos planes deben guardarse aquí como `*.plan.md` y añadirse al array `PLANS` en `index.html`.
