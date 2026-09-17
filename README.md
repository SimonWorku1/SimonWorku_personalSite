# Simon Worku — Personal Site

A portfolio for recruiters & companies, built as **plain HTML/CSS/JS** (no build step) so it deploys anywhere, including GitHub Pages.

The site is a single page, `index.html`, styled as a storefront: projects are browsed like a catalog with a filter sidebar, search, sort, and an "Add to Cart" action on each project that links out to its live site or repo.

## Preview locally

Just open `index.html` in a browser, or run a tiny local server:

```bash
cd SimonWorku_personalSite
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Push to GitHub (`main` branch).
2. Repo → **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `root`**.
3. The site goes live at `https://simonworku1.github.io/SimonWorku_personalSite/`.

## Editing content

Content is written directly into `index.html` (no shared data file, so nothing can silently fail to render). Search for the text and edit in place.

- **Profile photo:** `assets/profile.jpg` (falls back to an "SW" monogram in `assets/profile.svg`).
- **Project logos:** `assets/*-logo.png`.
- **Résumé:** `assets/resume.pdf` is the downloadable/previewed résumé; replace it to update.

## Notes

- Phone number is intentionally left off the public pages to reduce spam/scraping; email, GitHub, and LinkedIn are included.
- Respects `prefers-reduced-motion` and `prefers-color-scheme` where relevant.
