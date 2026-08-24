# Cómo montar esto en tu proyecto

Copia cada fichero a su ruta dentro del repo de Astro:

| Fichero | Destino |
|---|---|
| `src/consts.ts` | sustituye el del starter |
| `src/pages/index.astro` | sustituye el del starter |
| `src/pages/sobre-mi.astro` | nuevo (borra `src/pages/about.astro`) |
| `src/content/blog/el-catalogo-de-datos-dejo-de-ser-un-inventario.md` | nuevo |

## Después de copiar

**1. Borra los posts de ejemplo.** El starter trae tres o cuatro entradas de relleno en `src/content/blog/`. Bórralos todos.

**2. Ajusta el menú.** En `src/components/Header.astro`, cambia los enlaces a: Inicio (`/`), Blog (`/blog`), Sobre mí (`/sobre-mi`). Quita el de `/about` si existe.

**3. Pon tu dominio.** En `astro.config.mjs`:

```js
site: 'https://jopse.es',
```

Sin esto, el sitemap y el RSS generan URLs incorrectas.

**4. Comprueba el formato de fecha.** Si `pubDate: 'Aug 25 2026'` da error de validación, mira el formato que usan los posts de ejemplo antes de borrarlos y usa ese.

**5. Redes sociales del footer.** El starter trae enlaces de Astro. Cámbialos por los tuyos o quítalos.

## Comprobar antes de desplegar

```bash
npm run build && npm run preview
```

Revisa que existan `dist/sitemap-index.xml` y `dist/rss.xml`.

## Pendiente tras el despliegue

- Regla de redirección de `www.jopse.es` a `jopse.es`
- Dar de alta `jopse.es` en Google Search Console y enviar el sitemap
- Poner en privado el WordPress antiguo
- Cloudflare Web Analytics (sin cookies, sin banner)
