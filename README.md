# yt-lead-magnets

Static, client-side finance calculators used as YouTube video lead magnets.

- **ss-breakeven.html** — Social Security Break-Even Calculator (Money After 50)
- **scorp-vs-solo401k.html** — S-Corp vs Solo 401(k) Tax Calculator (Freelance Finance)

No backend. Vanilla HTML + JS. Hosted via GitHub Pages. Calculators run entirely client-side and make no network calls.

To deploy edits: push to `main`. GitHub Pages serves from `/` on the default branch.

## Email capture

Removed 2026-09-14. The pages shipped from 2026-07-03 with a Buttondown signup
form whose action was the literal placeholder `BUTTONDOWN_USERNAME`; no account
was ever created, so every subscribe attempt from both channels' CTAs was
dropped. If a list is wanted later, create the account first (via
account-agent), then add the form back with the real username and the source
tags `ma50-ss-breakeven` / `ff-scorp-solo401k`.
