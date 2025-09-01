# Astro Notion Notes Template

Plantilla ligera para crear un sitio personal de apuntes (estilo Notion) con Astro, Markdown/MDX, etiquetas, listado por tags y búsqueda en el cliente.

## Características

- Contenido en `src/content/notes` con frontmatter (title, description, tags, updated, draft)
- Página de notas, tags y búsqueda
- Rutas anidadas para notas (`notes/[...slug].astro`)
- Estilos oscuros limpios y accesibles
- MDX soportado con `@astrojs/mdx`
- Sitemap automático

## Empezar

1. Instala dependencias
2. Arranca el entorno de desarrollo
3. Crea tus primeras notas en `src/content/notes/`

```bash
# Windows PowerShell
npm install
npm run dev
```

Visita http://localhost:4321

## Estructura

- `src/content/config.ts`: colecciones de contenido (notes, pages)
- `src/pages/notes/[...slug].astro`: página para cada nota a partir del contenido
- `src/pages/notes/index.astro`: listado de notas
- `src/pages/tags/*`: listado por etiquetas
- `src/pages/search.astro`: búsqueda con filtrado client-side

## Publicar como tema en Astro

Sigue la guía oficial: https://docs.astro.build/es/themes/publish/

Checklist para publicar:

- package.json con `name`, `description`, `keywords` y `license` (MIT)
- `README.md` con demo, instalación y uso
- Demo deploy (por ejemplo, Vercel/Netlify)
- Etiquetas sugeridas: astro, theme, notes, notion

## Configuración

Edita `astro.config.mjs` y define `site` con la URL de producción.

## Licencia

MIT