# incyashraj.github.io

Personal site for **Yashraj Bhushan Pardeshi** ([@incyashraj](https://github.com/incyashraj)).
Single static HTML page, hand-pasted zine aesthetic. No build step.

## Files

```
index.html             ← the live site
assets/me-sticker.png  ← photo sticker in the hero
variants/              ← three alternate directions (cream, broadsheet, schematic, zine)
directions.html        ← chooser page showing all four variants side-by-side
```

You can delete `variants/` and `directions.html` once you've picked your direction — only `index.html` and `assets/` are required.

## Deploy to GitHub Pages (free, custom URL at https://incyashraj.github.io)

The cleanest path is a **user site** — a repo named exactly `incyashraj.github.io`. That gets you a top-level URL with no path prefix.

1. On GitHub, create a new public repo named `incyashraj.github.io` (must match your username exactly).
2. Push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "first paste"
   git branch -M main
   git remote add origin https://github.com/incyashraj/incyashraj.github.io.git
   git push -u origin main
   ```
3. GitHub Pages auto-enables for user repos. Within ~1 minute the site is live at **https://incyashraj.github.io**.

### Or: a regular project repo

If you'd rather put it inside another repo (say `personal-site`):

1. Push to a repo of any name.
2. Go to **Settings → Pages**.
3. Source: **Deploy from a branch** · Branch: `main` · Folder: `/ (root)`.
4. Save. URL will be `https://incyashraj.github.io/personal-site`.

### Custom domain (optional)

If you own `incyashraj.com`:

1. Add a `CNAME` file at repo root containing just `incyashraj.com`.
2. In your DNS, point `incyashraj.com` to GitHub Pages (`A` records to `185.199.108.153`, `.109.153`, `.110.153`, `.111.153`, plus `AAAA` for IPv6 if you want).
3. **Settings → Pages → Custom domain** → enter `incyashraj.com` and tick **Enforce HTTPS**.

## Edit the site

It's one file: `index.html`. The Builder · Learner · Human content lives in the `MODES` object inside the `<script>` at the bottom of the file — edit the strap line or chips there.

Fonts are pulled from Google Fonts (Archivo Black, Fraunces, Caveat, Space Mono, Inter) — no install needed.

## Stack

Plain HTML/CSS/JS. No build, no framework, no tracker.
