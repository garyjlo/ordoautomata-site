# Ordo Automata — site mockup

Static site. No build step.

## Deploy to Cloudflare Pages
1. Commit the contents of this folder to the root of `garyjlo/ordoautomata-site` (main).
2. Cloudflare dashboard → Workers & Pages → Create → Pages → Connect to Git → pick the repo.
3. Framework preset: **None**. Build command: *(leave empty)*. Build output directory: `/`.
4. Deploy, then Custom domains → add your domain (Cloudflare adds the DNS record if the domain is on Cloudflare).

## Files
- `index.html` — the page
- `support.js` — runtime the page needs
- `image-slot.js` — partner portrait slots (replace with <img> once photos exist)
- `assets/` — seal and trace artwork
- `_headers` — Cloudflare cache and security headers

## Before going public
- The contact form only shows the stamp animation; it does not send anywhere yet. Wire it to a form service or a Cloudflare Pages Function.
- Replace the SAMPLE results, the pull quote, partner names and photos, and the email address.
- The seal is a raster cut from the concept diagram; swap in a vector version when available.
