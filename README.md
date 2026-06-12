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

With the GitHub CLI installed and authenticated (`gh auth login`), run from this folder:

```bash
gh repo create japan-souvenirs --public --source=. --remote=origin --push
gh api -X POST repos/{owner}/japan-souvenirs/pages -f "source[branch]=main" -f "source[path]=/"
```

Live URL: `https://[yourusername].github.io/japan-souvenirs`

Pages can take a minute to go live after the first push.

## Files

- `index.html` — the entire app
- `README.md` — this file