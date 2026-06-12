# Japan Souvenir Tracker

A single-file web app to track souvenir gifts for a trip. No build step, no dependencies. Open `index.html` in any browser or host it on GitHub Pages.

## What it does

- **People tab**: list everyone you’re buying for (yourself included), assign a gift idea per person, cycle status To buy → Bought → Packed
- **Items & ideas tab**: log any item, idea, or request, cycle status Idea → Bought → Request, tag who it’s for
- **Coverage counter**: shows who and what is still unsorted
- **Copy to text**: dumps the full list as plain text for backup or pasting into trip notes
- **Print**: clean printable checklist

Data saves to your browser via `localStorage`. It does not sync across devices. Use “Copy to text” for a portable backup.

## Run locally

Open `index.html` in a browser. That’s it.

## Deploy to GitHub Pages

This repo deploys automatically via GitHub Actions. The workflow in
`.github/workflows/deploy-pages.yml` runs on every push, enables Pages if it
isn't already on, and publishes the site.

Live URL: https://allhaile.github.io/jp-2026/

Pages can take a minute or two to go live after the first deploy. You can watch
the run under the repo's **Actions** tab.

## Files

- `index.html` — the entire app
- `README.md` — this file