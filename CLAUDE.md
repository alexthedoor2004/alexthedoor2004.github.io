# Personal site

Alex's personal website. Minimal, text-first (inspired by jaytel). Static HTML + CSS, no build step, no framework.

## Files
- `index.html` — intro, experience, recent thoughts, links.
- `story.html` — longer "about me" story.
- `thoughts/` — writing. `index.html` lists posts; each post is its own file. Copy `_template.html` to add one, then add a row to `thoughts/index.html` and the "Recent thoughts" list on the home page (newest first).
- `travel/index.html` — photo galleries, one `<article class="trip">` per trip. Photos go in `assets/travel/<place>/`, resized to ~2000px wide. Clicking a photo opens a lightbox.
- `style.css` — all styling. Colors are CSS variables at the top (`:root`), with a dark-mode block below.

## Run locally
`python3 -m http.server 8000` then open http://localhost:8000

## Deploy
Hosted on GitHub Pages from the `main` branch. Pushing to `main` updates the live site in ~1 minute.
Links are relative (no leading `/`) so it works as a user or project Pages site.

## Conventions
- Keep it dependency-free: no npm, no frameworks, no build tools unless Alex asks.
- Minimal style: one font size, muted grey for secondary text, lots of whitespace. Must look good on mobile and in dark mode.
- Experience blurbs are 2–3 casual sentences, not resume bullets.
- Don't put a personal email address in the page without Alex confirming which one.
