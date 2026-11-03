# Personal site

Alex's personal website: About, Experience, Contact. Static HTML + CSS, no build step, no framework.

## Files
- `index.html` — all content. Sections are marked with `<!-- ABOUT -->`, `<!-- EXPERIENCE -->`, `<!-- CONTACT -->`.
- `style.css` — all styling. Colors are CSS variables at the top (`:root`), with a dark-mode block below.
- `assets/` — images and `resume.pdf` (the "View resume" button links to `assets/resume.pdf`).

## Run locally
`python3 -m http.server 8000` then open http://localhost:8000

## Deploy
Hosted on GitHub Pages from the `main` branch. Pushing to `main` updates the live site in ~1 minute.

## Conventions
- Keep it dependency-free: no npm, no frameworks, no build tools unless Alex asks.
- Clean and minimal style; must look good on mobile and in dark mode.
- Don't put a personal email address in the page without Alex confirming which one.
