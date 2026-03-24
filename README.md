# Boiler Plate Astro Lead

Boilerplate para proyectos de lead generation construido con Astro y Tailwind CSS.

## Stack

- **Astro 6** - Framework web con arquitectura de islas
- **Tailwind CSS 4** - Utility-first CSS framework (via Vite plugin)
- **Node.js >= 22.12.0**

## Estructura del proyecto

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── assets/
│   │   └── astro.svg
│   ├── components/
│   │   └── Welcome.astro
│   ├── layouts/
│   │   └── Layout.astro        # Layout principal (importa global.css)
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css           # Tailwind CSS entry point
├── astro.config.mjs             # Configuracion de Astro + Tailwind Vite plugin
└── package.json
```

## Tailwind CSS

Tailwind 4 esta configurado via el plugin de Vite en `astro.config.mjs`:

```js
import tailwindcss from '@tailwindcss/vite';

export default defineConfig({
  vite: {
    plugins: [tailwindcss()],
  },
});
```

Los estilos globales se importan desde `src/styles/global.css` en el layout principal (`src/layouts/Layout.astro`).

## Comandos

| Comando             | Accion                                          |
| :------------------ | :---------------------------------------------- |
| `npm install`       | Instala dependencias                            |
| `npm run dev`       | Inicia servidor de desarrollo en `localhost:4321`|
| `npm run build`     | Build de produccion en `./dist/`                |
| `npm run preview`   | Preview del build local                         |

## Claude Code Setup

### MCP Server (Astro Docs)

```bash
claude mcp add --transport http astro-docs https://mcp.docs.astro.build/mcp
```

Permite consultar la documentacion oficial de Astro directamente desde Claude Code.

## Skills disponibles

Este proyecto incluye los siguientes skills para Claude Code:

- **frontend-design** - Genera interfaces frontend con alto nivel de diseno, evitando esteticas genericas de IA
- **seo-audit** - Audita sitios web usando SEOmator CLI (251 reglas, 20 categorias)
