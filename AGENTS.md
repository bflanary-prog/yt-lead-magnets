# yt-lead-magnets

Static, client-side finance calculators used as YouTube video lead magnets. No backend, no tracking, no signup.

## Stack
- Vanilla HTML + inline CSS + inline JavaScript. No framework, no build step, no dependencies.
- Hosted via GitHub Pages.

## Run / test
- Open any `.html` file directly in a browser, or serve locally: `python3 -m http.server` then visit `index.html`.
- No tests, no build.

## Layout
- `index.html` — landing page linking to the calculators.
- `ss-breakeven.html` — Social Security Break-Even Calculator (Money After 50).
- `scorp-vs-solo401k.html` — S-Corp vs Solo 401(k) Tax Calculator (Freelance Finance).
- `README.md` — overview and deploy note.

## Conventions / gotchas
- All logic and styles are inline in each HTML file; keep them self-contained (no shared assets).
- Deploy by pushing to `main` — GitHub Pages serves from `/` on the default branch.
- Educational tools only; each page carries a "not tax/financial advice" disclaimer — keep it.
