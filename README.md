# nevil enyola — personal site

Source for **https://enyolanev-bit.github.io** (and eventually `enyola.ai`).

Single static page, monospace, ayomide-style. Bilingual (EN-first + FR). Hosted via GitHub Pages, auto-deployed on push to `main`.

## What's here

- `index.html` — the whole site, one file. EN/FR toggle persists in localStorage.
- `agent-log.json` — live signal feed surfaced in the AGENT LOG section. Updated daily by the GitHub Action below.
- `.github/workflows/refresh-agent-log.yml` — daily cron (06:17 UTC) that pulls latest commits across my public repos and rewrites `agent-log.json`.
- `LICENSE` — site copy is CC BY 4.0, code (HTML/CSS/JS, workflow) is MIT.

## Why a single HTML file

Building this site is itself a discipline test : I want a portfolio that proves the AI-native pattern (humans + agents + memory + eval + customer loop) without dragging in a framework that hides it. Plain HTML loads in <500 ms, has zero build step, runs anywhere, and the entire source fits in one editor tab.

The AGENT LOG section is the differentiator. Most personal sites are static snapshots written once and decayed. This one updates daily from the actual activity of my public repos. It's a small claim made every day automatically.

## Local preview

```bash
open index.html
```

That's it.

## Updating content

- **Copy** : edit the `<div data-lang="en">` and `<div data-lang="fr">` blocks in `index.html`. Keep parity.
- **Projects** : append to the `selected work` list in both languages. Keep one line per project, link first.
- **Agent log lines** : updated automatically. To curate manually, edit `agent-log.json` directly (the workflow regenerates it every 24h, so any manual edit will be replaced — for permanent additions, add a "pinned" section to the workflow).

## License

Site copy (text, story, voice) : CC BY 4.0. Reuse freely with attribution.
Code (HTML / CSS / JS / workflow) : MIT.
