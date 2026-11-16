# priyankacherukuri — personal website

A static, dependency-free personal site (HTML + CSS + a little JS). No build step.

```
index.html        page content
styles.css        design tokens, light/dark themes, layout
script.js         theme toggle, active nav, reveal-on-scroll
assets/           headshot.jpg, favicon.svg
```

## Preview locally

```bash
python3 -m http.server 8080
```

Then open http://localhost:8080.

## Deploy to GitHub Pages

The fastest route is a user site at `https://cherukuri89.github.io`:

1. On GitHub, create a public repo named **`cherukuri89.github.io`**.
2. From this folder:

```bash
git remote add origin https://github.com/cherukuri89/cherukuri89.github.io.git
```

```bash
git push -u origin main
```

3. In the repo, open **Settings → Pages**, set Source to **Deploy from a branch**, pick `main` / `(root)`. The site goes live in a minute or two.

### Custom domain (optional)
Buy a domain (e.g. `priyankacherukuri.com`), add a `CNAME` file containing the domain, and point DNS at GitHub Pages per
https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site.

## Editing content
All text lives in `index.html`. Colors are tokens at the top of `styles.css` (`--accent` changes the highlight color in light mode; the dark-mode block has its own).
