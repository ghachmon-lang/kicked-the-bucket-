# Kicked the Bucket!

A deadly funny party game. It's a single self-contained HTML file — no install, no server, no accounts.

## Play it / share it

**https://ghachmon-lang.github.io/kicked-the-bucket-/**

Send that link to anyone. It opens straight into the game in their phone or desktop browser.

On iPhone, players can tap Share → "Add to Home Screen" to get an app icon that opens it full-screen.

## How it's published

GitHub Pages is set to **Deploy from a branch → `main` → `/docs`**, so the published site is whatever is in `docs/`.

- `docs/index.html` — the file that gets served at the link above
- `docs/he/index.html` — the Hebrew app (see below), served at `/he/`
- `docs/.nojekyll` — tells Pages to serve the folder as-is instead of running it through Jekyll
- `kicked_the_bucket_20260809_151446.html` — the original export, kept at the repo root for reference

## Hebrew edition — "הלך לעולמו!"

**https://ghachmon-lang.github.io/kicked-the-bucket-/he/**

A separate app, not a translation layer: its own file, its own link, its own deck. Same rules and
mechanics, but the writing is adult (18+) and the scenarios are Israeli rather than generic —
the deck is built around things like משרד הפנים, מילואים, קבוצת ווטסאפ משפחתית and ארונות איקאה.

Notes for editing it:

- The page is `dir="rtl"` with a Hebrew-capable font stack, so it works on iOS, Android and desktop
  without loading a web font.
- `HOW_CARDS` are deliberately phrased as verbal nouns ("התחשמלות מ…", "בליעה של…") so any card pairs
  with any character without זכר/נקבה disagreement.
- Every card carries exactly one `<u>…</u>` — that's the word the team has to guess.

To publish a change, update `docs/index.html` on `main`. Pages redeploys automatically within a minute or two.
