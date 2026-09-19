# System Engineer Profile

Personal profile site built with Astro and designed for static deployment.

## Local development

```bash
pnpm install
pnpm run dev
```

## Build

```bash
pnpm run build
```

The generated site is in `dist/`.

## Cloudflare Pages (Git-based deploy)

This project uses Astro static output, deployed via Cloudflare Pages connected to GitHub.

### Setup steps:
1. Push this repo to GitHub
2. Go to [Cloudflare Dashboard → Pages → Create a project](https://dash.cloudflare.com/pages/create)
3. Connect to GitHub and select this repo
4. Cloudflare auto-detects Astro:
   - **Build command**: `pnpm run build`
   - **Build output directory**: `dist`
5. Set custom domain `myjamal.com` in Cloudflare dashboard
6. Push to main branch — Cloudflare auto-deploys

### Before first deploy:
- `site` in `astro.config.mjs` set to `https://myjamal.com` ✅
- Replace `hello@example.com` in `src/pages/index.astro`
- Add real GitHub/LinkedIn links if desired
- Replace sample project descriptions with public-safe projects
