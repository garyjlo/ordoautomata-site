# Ordo Automata — site mockup

Static site. No build step.

## Deploy to Cloudflare (Workers, static assets)
1. Commit the contents of this folder to the root of `garyjlo/ordoautomata-site` (main).
2. Cloudflare dashboard → Workers & Pages → Create → Worker → Connect to Git → pick the repo.
3. Build command: *(empty)*. Deploy command: `npx wrangler deploy`. Root directory: `/`.
4. `wrangler.toml` tells wrangler to serve this folder as static assets; no code bundle.
5. Settings → Domains & Routes → add the custom domain.

If the project was created as **Pages** instead: framework preset None, no build command, output directory `/`, and `wrangler.toml` is ignored.

## Files
- `index.html` — the page
- `support.js` — runtime the page needs
- `image-slot.js` — partner portrait slots (replace with <img> once photos exist)
- `assets/` — seal and trace artwork
- `_headers` — Cloudflare cache and security headers
- `wrangler.toml` — Worker config: serves the folder as static assets

## Before going public
- The contact form only shows the stamp animation; it does not send anywhere yet. Wire it to a form service or a Cloudflare Pages Function.
- Replace the SAMPLE results, the pull quote, partner names and photos, and the email address.
- The seal is a raster cut from the concept diagram; swap in a vector version when available.
 