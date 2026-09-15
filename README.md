# EGNT thesis — static site

Deploy as-is: no build step, no JavaScript, no external requests.

- `index.html` — the page
- `styles.css` — design-system tokens + page styles, single file
- `fonts/` — self-hosted Google Sans Flex (woff2)
- `img/` — icons, Europe map

## Two images still to add

The logo and founder photo are referenced but not included (they live on egnt.ai and could not be copied here). Drop these two files into `img/`:

- `img/egnt_logo.png` — from https://egnt.ai/img/egnt_logo.png
- `img/egnt_eg.png` — from https://egnt.ai/img/egnt_eg.png

Optionally add `img/favicon.png` and re-add a `<link rel="icon">` in `index.html`.

## Notes

- `<head>` OG tags point at `https://egnt.ai/thesis/` — change the canonical/og:url if you deploy elsewhere.
- Vercel: drop the folder in as the project root, framework preset "Other", no build command, output directory `.`
- GitHub Pages: push the folder contents to the `gh-pages` branch (or /docs on main).
