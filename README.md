# nevil enyola  personal site

Source for **https://enyolanev-bit.github.io** (and eventually `enyola.ai`).

Single static page, monospace, ayomide-style. Bilingual (EN-first + FR). Hosted via GitHub Pages, auto-deployed on push to `main`.

## What's here

- `index.html`  the whole site, one file. EN/FR toggle persists in localStorage.
- `LICENSE`  site copy is CC BY 4.0, code (HTML/CSS/JS) is MIT.

## Why a single HTML file

Plain HTML loads in <500 ms, has zero build step, runs anywhere, and the entire source fits in one editor tab. No framework dragged in.

## Local preview

```bash
open index.html
```

That's it.

## Updating content

- **Copy** : edit the `<div data-lang="en">` and `<div data-lang="fr">` blocks in `index.html`. Keep parity.
- **Projects** : append to the `selected work` list in both languages. Keep one line per project, link first.

## License

Site copy (text, story, voice) : CC BY 4.0. Reuse freely with attribution.
Code (HTML / CSS / JS) : MIT.
