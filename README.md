# Amine Ouaddi — Portfolio

A single-page personal portfolio site with a Persona 3 Reload–inspired UI:
deep-blue color palette, animated liquid transitions between sections, and a
HUD-style panel system in place of generic cards.

**Live site:** _add your GitHub Pages URL here once deployed_

## Overview

This is a dashboard-style, single-page site. Instead of scrolling, the four
buttons on the home screen (`About Me`, `Experience`, `Projects`, `Resume`)
swap the visible screen using a custom liquid-merge transition built with
layered CSS gradients and a gooey blur/contrast filter.

## Tech stack

- **HTML5 / CSS3** — no framework, no build step
- **Vanilla JavaScript** — view switching, transition sequencing, nav state
- **Google Fonts** — Bebas Neue (display) + Inter (body)
- **GitHub Actions** — automated build & deploy to GitHub Pages on every push to `main`

## Project structure

```
.
├── index.html                     # the entire site (markup, styles, script)
├── resume.pdf                     # resume, opened directly from the Resume button
├── README.md                      # you are here
└── .github/
    └── workflows/
        └── deploy.yml             # CI/CD: deploys to GitHub Pages automatically
```

## Features

- Dashboard-style navigation with a custom liquid transition between views
  (no page scrolling between sections)
- Top navigation bar that dynamically swaps the current page's own button
  for a "Home" shortcut, rather than leaving an empty slot
- Content sourced from a single resume with no invented experience, projects,
  or statistics
- Fully responsive: collapses gracefully on mobile

## Running locally

No build tools required. Either:

- Open `index.html` directly in a browser, or
- Serve it locally for a closer-to-production experience:
  ```bash
  python3 -m http.server 8000
  ```
  then visit `http://localhost:8000`

## Deployment

This repo deploys automatically via the GitHub Actions workflow in
`.github/workflows/deploy.yml` any time changes are pushed to `main`.
GitHub Pages is configured to serve from the **GitHub Actions** build
(Settings → Pages → Source → GitHub Actions), rather than a static branch,
so every commit produces a fresh, versioned deployment visible in the
repo's **Actions** tab.

## Design credit

Visual direction is inspired by the UI language of *Persona 3 Reload*
(color palette, panel styling, fluid transitions) — no game assets, logos,
or copyrighted material are used.

## License

Personal project. Content and resume information belong to Amine Ouaddi;
feel free to reference the code structure for your own portfolio.
