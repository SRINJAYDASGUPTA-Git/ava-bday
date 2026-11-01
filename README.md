# Avanti — A Little Universe

A static Astro project migrated from the Canva-generated HTML export. The original visual styling and chapter content are preserved, while Canva's editor/bootstrap scripts have been removed. The birthday candle/confetti interaction remains in the page.

## Requirements

- Node.js 18.20.8+, 20.3.0+, or 22+
- npm

## Run locally

```bash
npm install
npm run dev
```

## Build and preview

```bash
npm run build
npm run preview
```

Astro outputs the static site to `dist/`, ready for Vercel, Netlify, GitHub Pages, or a static web server.

## Customize

- Main content and chapter markup: `src/pages/index.astro`
- Design styles: `src/styles/global.css`
- Add photos/assets: `public/images/` and reference them with `/images/your-file.jpg`

The current Canva export includes image placeholders; replace those with personal photos when ready.
