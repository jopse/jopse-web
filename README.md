# jopse.es

Site personal de José Ángel González Mejías: arquitectura de software, gobierno del dato, equipos de ingeniería y lo que dé para escribir. Construido con [Astro](https://astro.build) y desplegado en Cloudflare.

## Stack

- [Astro](https://astro.build) 7 + [MDX](https://docs.astro.build/en/guides/integrations-guide/mdx/) para las entradas del blog
- Sitemap y RSS generados automáticamente ([`@astrojs/sitemap`](https://docs.astro.build/en/guides/integrations-guide/sitemap/), [`@astrojs/rss`](https://docs.astro.build/en/guides/rss/))
- Tipografía Atkinson servida localmente vía `astro:assets`
- Despliegue en [Cloudflare](https://developers.cloudflare.com/workers/) mediante `wrangler` (config en `wrangler.jsonc`)

## Estructura

```text
├── public/
├── src/
│   ├── assets/        # imágenes y fuentes locales
│   ├── components/    # Header, Footer, BaseHead...
│   ├── content/blog/  # entradas del blog en Markdown/MDX
│   ├── layouts/        # BlogPost.astro
│   └── pages/          # index, sobre-mi, blog/...
├── astro.config.mjs
├── wrangler.jsonc
└── package.json
```

## Comandos

Todos se ejecutan desde la raíz del proyecto:

| Comando           | Acción                                              |
| :----------------- | :--------------------------------------------------- |
| `npm install`       | Instala dependencias                                  |
| `npm run dev`       | Arranca el servidor de desarrollo en `localhost:4321` |
| `npm run build`     | Genera el sitio de producción en `./dist/`            |
| `npm run preview`   | Previsualiza el build localmente antes de desplegar   |
| `npm run deploy`    | Publica `./dist/` en Cloudflare vía `wrangler deploy` |
| `npm run astro ...` | Ejecuta comandos de la CLI de Astro (`astro check`...) |

Requiere Node >= 22.12.0.
