# Kicked the Bucket!

A deadly funny party game. It's a single self-contained HTML file — no install, no server, no accounts.

## Play it / share it

**https://ghachmon-lang.github.io/kicked-the-bucket-/**

Send that link to anyone. It opens straight into the game in their phone or desktop browser.

On iPhone, players can tap Share → "Add to Home Screen" to get an app icon that opens it full-screen.

## How it's published

GitHub Pages is set to **Deploy from a branch → `main` → `/docs`**, so the published site is whatever is in `docs/`.

- `docs/index.html` — the file that gets served at the link above
- `docs/.nojekyll` — tells Pages to serve the folder as-is instead of running it through Jekyll
- `kicked_the_bucket_20260809_151446.html` — the original export, kept at the repo root for reference

To publish a change, update `docs/index.html` on `main`. Pages redeploys automatically within a minute or two.
