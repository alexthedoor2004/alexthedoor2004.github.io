# Personal site

Alex's personal website. Minimal, text-first (inspired by jaytel). Static HTML + CSS, no build step, no framework.

## Files
- `index.html` — intro, experience, recent thoughts, links.
- `about.html` — longer "about me" story.
- `thoughts/` — writing. `index.html` lists posts; each post is its own file. Copy `_template.html` to add one, then add a row to `thoughts/index.html` and the "Recent thoughts" list on the home page (newest first).
- `projects/index.html` — project list. Copy the commented `<div class="project">` block (newest first) and remove the "Nothing here yet" box once there's one project.
- `style.css` — all styling. Blush palette and fonts (Fraunces for headings, DM Sans for body) are CSS variables at the top (`:root`). Light only, no dark mode.

## Run locally
`python3 -m http.server 8000` then open http://localhost:8000

## Deploy
Hosted on GitHub Pages from the `main` branch. Pushing to `main` updates the live site in ~1 minute.
Links are relative (no leading `/`) so it works as a user or project Pages site.

## Conventions
- Keep it dependency-free: no npm, no frameworks, no build tools unless Alex asks.
- Minimal style: serif headings, sans body, muted rose for secondary text, lots of whitespace. Must look good on mobile. Keep text readable (body text in `--text`, not too pale).
- Experience blurbs are 2–3 casual sentences, not resume bullets.
- Never put Alex's email, phone number or address in the page. Contact goes through the form on the home page (Web3Forms; the access key in `index.html` is public-safe and routes to Alex's inbox).
