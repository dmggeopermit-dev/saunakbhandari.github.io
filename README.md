# Saunak Bhandari — Portfolio

Static portfolio site (HTML + Tailwind CDN). No build step.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole site (content is in the `<script>` at the bottom) |
| `404.html` | Redirects broken links to the home page |
| `img/` | Put gallery photos here |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Before publishing

1. Open `index.html` and edit the `CONFIG` block at the top of the script: set your real `email`, `linkedin` and `researchgate` URLs. Unset values are hidden.
2. Optional: add photos to `img/` and reference them in the `gallery` array, e.g. `["🏔️","Fieldwork","img/field1.jpg"]`.

## Deploy on GitHub Pages

1. Create a new repository on GitHub (for a user site, name it `<username>.github.io`).
2. Upload all files in this folder, or from a terminal:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/<username>/<repo>.git
   git push -u origin main
   ```
3. In the repo go to **Settings → Pages**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, then **Save**.
4. After a minute the site is live at `https://<username>.github.io/` (or `/<repo>/` for a project repo).

## Local preview

Open `index.html` in a browser, or run `python3 -m http.server` in this folder and visit http://localhost:8000.
