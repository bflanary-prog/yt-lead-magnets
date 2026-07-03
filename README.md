# yt-lead-magnets

Static, client-side finance calculators used as YouTube video lead magnets.

- **ss-breakeven.html** — Social Security Break-Even Calculator (Money After 50)
- **scorp-vs-solo401k.html** — S-Corp vs Solo 401(k) Tax Calculator (Freelance Finance)

No backend. Vanilla HTML + JS. Hosted via GitHub Pages. Calculators run entirely client-side; the only network call is the optional email signup form, which POSTs to Buttondown.

To deploy edits: push to `main`. GitHub Pages serves from `/` on the default branch.

## Email capture (Buttondown)

Each calculator has a "companion checklist" signup form below the results that POSTs to Buttondown's embed endpoint (`https://buttondown.com/api/emails/embed-subscribe/<username>`). A hidden `tag` field attributes the source:

- `ss-breakeven.html` → tag `ma50-ss-breakeven`
- `scorp-vs-solo401k.html` → tag `ff-scorp-solo401k`

### Setup (one-time)

1. Create a free Buttondown account at https://buttondown.com (free tier covers this).
2. Replace `BUTTONDOWN_USERNAME` with your Buttondown username in the 3 functional spots:
   - `index.html:34` (footer signup link)
   - `ss-breakeven.html:82` (form action)
   - `scorp-vs-solo401k.html:85` (form action)

   Easiest: `sed -i '' 's/BUTTONDOWN_USERNAME/yourusername/g' index.html ss-breakeven.html scorp-vs-solo401k.html` — this also cleans up the TODO comments at line 2 of each file (delete those comments after replacing).
3. Push to `main`. Done.
