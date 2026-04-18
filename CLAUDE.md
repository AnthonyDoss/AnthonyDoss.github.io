# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Static personal portfolio website hosted on GitHub Pages. No build tools, frameworks, or package managers — files are served directly.

## Development

To preview locally, open `index.html` in a browser or run a simple HTTP server:

```bash
python3 -m http.server 8080
```

Deploying is just pushing to the `master` branch on GitHub — GitHub Pages publishes automatically.

## Architecture

Single-page site with three files driving the UI:

- [index.html](index.html) — all page structure and inline JS (navigation/hamburger menu logic)
- [main.css](main.css) — custom styles using CSS variables for the color palette and Google Fonts (Montserrat, Poppins, Cinzel Decorative)
- [reset.css](reset.css) — Meyer Web CSS reset

External dependencies are loaded via CDN (no local install needed):
- **Bulma 0.7.4** — CSS framework for layout/grid
- **Font Awesome v5.6.3** — icons
- **AniJS** — scroll-triggered animations

Color palette is defined as CSS variables in `main.css`: `--white`, `--light-gray`, `--gray`, `--dark-gray`, `--accent`, `--dark-blue`.
