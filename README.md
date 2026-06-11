# Libra Research — Website

Static site for [libraresearch.github.io](https://libraresearch.github.io), built to the Libra Research visual identity system v1.0.

## Structure

```
index.html        Single-page site (services, methodology, clients, about, contact)
404.html          Not-found page (served automatically by GitHub Pages)
css/main.css      All styles
js/main.js        Progressive enhancement only (mobile nav, scroll reveal)
assets/favicon.svg  Signal mark favicon (adapts to light/dark mode)
```

## Identity rules baked in

- **Colour** — ink `#1B1A17` on paper `#F7F5F0` and the exact reverse. No accents, no tints.
- **Type** — Spectral (serif) for headings and body; IBM Plex Mono for kickers, labels, prices.
- **Marks** — Signal (4×4 dot field, solid dot at row 2 / col 3) is the primary mark, defined once as an inline SVG `<symbol>` and reused via `<use>`. Scales is the secondary mark, used in the Methodology section. Both render without JavaScript.

## Local preview

Any static server works:

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploying

The site is plain static files — push the contents of this folder to the root of the `libraresearch.github.io` repository (default branch) and GitHub Pages serves it as-is. No build step.
