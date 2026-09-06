# Amine Ouaddi — Portfolio

A single-page personal portfolio site by Amine Ouaddi

**Live site:**

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

