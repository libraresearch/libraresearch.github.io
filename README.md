# Libra Research — Website

Static site for [libraresearch.github.io](https://libraresearch.github.io), built to the Libra Research visual identity system v1.0.

## Structure

```
index.html          Single-file site — all CSS and JS inline (services, methodology,
                    sample work, clients, about, contact)
404.html            Not-found page (served automatically by GitHub Pages)
sample-report.pdf   Anonymized sample due-diligence report (linked from Sample work)
assets/favicon.svg  Signal mark favicon (adapts to light/dark mode)
```

## Identity rules baked in

- **Colour** — ink `#16140F` on archival paper `#F3EFE6`, with a single restrained oxblood accent (`oklch(0.47 0.13 27)`) reserved for section markers and status/risk indicators.
- **Type** — Spectral (serif) for display and body; IBM Plex Mono for labels, metadata, and classification text.
- **Marks** — Signal (4×4 dot field, solid dot at row 2 / col 3) is the primary mark, defined once as an inline SVG `<symbol>` and reused via `<use>`. It renders without JavaScript.

## Local preview

Any static server works:

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploying

The site is plain static files — push the contents of this folder to the root of the `libraresearch.github.io` repository (default branch) and GitHub Pages serves it as-is. No build step.
