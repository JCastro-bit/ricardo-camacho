# CLAUDE.md

## Proyecto

Boilerplate para lead generation con Astro 6 y Tailwind CSS 4.

## Stack y configuracion

- **Astro 6** con configuracion en `astro.config.mjs`
- **Tailwind CSS 4** via `@tailwindcss/vite` plugin (NO usa `tailwind.config.js`, usa la nueva API de Tailwind 4)
- **Node.js >= 22.12.0** (requerido por `engines` en package.json)
- Entry point de estilos: `src/styles/global.css` (importado en `src/layouts/Layout.astro`)

## Comandos

```bash
npm run dev      # Servidor de desarrollo en localhost:4321
npm run build    # Build de produccion
npm run preview  # Preview del build
```

## Convenciones

- Usar clases de Tailwind directamente en los componentes `.astro`
- El layout principal es `src/layouts/Layout.astro` y ya importa `global.css`
- Todos los estilos globales van en `src/styles/global.css`
- Las paginas van en `src/pages/`
- Los componentes reutilizables van en `src/components/`

## MCP Servers

- **astro-docs** - Documentacion oficial de Astro accesible via MCP. Usar para consultar APIs, guias y referencias de Astro.
  ```bash
  claude mcp add --transport http astro-docs https://mcp.docs.astro.build/mcp
  ```

## Skills

- `/frontend-design` - Para crear interfaces con diseno distintivo y produccion-grade
- `/seo-audit` - Para auditar SEO con SEOmator CLI (`npm install -g @seomator/seo-audit`)
