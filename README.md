# jasonlim.design

Personal portfolio — a rotating 3D ring of product work over a grid background, with an About view.

## Deploy (GitHub Pages)

1. Push this repo to GitHub.
2. Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The `CNAME` file points the site at **jasonlim.design** — set that DNS record (CNAME → `<user>.github.io`) at your registrar.

No build step. `index.html` is served as-is; `.nojekyll` tells Pages to serve every file verbatim.

## Structure

- `index.html` — the landing screen (rotating ring + About)
- `support.js` — the single runtime loaded by the landing page and every case study
- `assets/` — shared styles plus all fonts, logos, videos, root images, and `work/<slug>/` case-study media
- `work/` — finished case-study pages only (`<slug>.dc.html`)
- `CNAME` — custom domain

`uploads/`, `screenshots/`, local development notes, and the original Ouster source backup are gitignored working files and are not part of the deployed site.
