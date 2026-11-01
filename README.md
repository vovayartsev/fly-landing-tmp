# Krugalia landing page

A static, single-page English landing page. No framework, build step, or runtime JavaScript is required.

## Files

- `index.html` — complete page and inline styles
- `assets/logo-landing.png` — horizontal Krugalia wordmark
- `assets/landing-hero.jpg` — hero illustration
- `assets/mascot.png` — assistant avatar
- `assets/favicon.ico` — favicon
- `wrangler.jsonc` — Cloudflare Workers Static Assets configuration

The logo, hero image, and mascot in this draft were cropped from existing Krugalia brand-concept images available in the project library because the separately named source exports were not attached in this chat. They are visually consistent draft assets; replace them with the final original exports under the same filenames when available. The HTML paths will not need to change.

## Local preview

Open `index.html` in a browser, or serve this directory with any static HTTP server.

## Cloudflare Workers

The included `wrangler.jsonc` points Workers Static Assets at the project root; `.assetsignore` keeps project notes and deployment configuration out of the public asset set. From this directory, deploy with Wrangler:

```sh
npx wrangler deploy
```

Connect the repository to the Worker through Cloudflare's Git integration or deploy from the command line. Add `krugalia.com` as the Worker custom domain in the Cloudflare dashboard after the Worker is deployed. No build command is needed.
