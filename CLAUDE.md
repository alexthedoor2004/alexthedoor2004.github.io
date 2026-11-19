# Personal site

Alex's personal website. Layout follows jay.tel: one font, one size, left-aligned, lowercase section labels, two-column rows. Static HTML + CSS, no build step, no framework.

## Files
- `index.html` — everything on one page: about, past (experience), projects, thoughts, contact. Projects are rows in the projects section (commented template there).
- `about.html` — longer "about me" story.
- `thoughts/` — writing. `index.html` lists posts; each post is its own file. Copy `_template.html` to add one, then add a row to `thoughts/index.html` and the home page's thoughts section (newest first).
- `style.css` — all styling. Pages link it as `style.css?v=N`; bump N in every HTML file after changing it so browsers drop their cached copy. Blush palette and fonts (Geist body, Instrument Serif for the name) are CSS variables at the top (`:root`). Light only, no dark mode.

## Run locally
`python3 -m http.server 8000` then open http://localhost:8000

## Deploy
Hosted on GitHub Pages from the `main` branch. Pushing to `main` updates the live site in ~1 minute.
Links are relative (no leading `/`) so it works as a user or project Pages site.

## Conventions
- Keep it dependency-free: no npm, no frameworks, no build tools unless Alex asks.
- Minimal style: Geist at one size everywhere (Instrument Serif italic only for the name), muted rose for secondary text, lots of whitespace. Elements with class `rise` fade in, staggered by `--i`. Must look good on mobile. Keep text readable (body text in `--text`, not too pale).
- Experience rows are company (linked) + one short, casual line. No BNP, Watsolve or CFA.
- Never put Alex's email, phone number or address in the page. Contact goes through the form on the home page (Web3Forms; the access key in `index.html` is public-safe and routes to Alex's inbox).
