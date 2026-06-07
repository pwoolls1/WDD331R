# WDD 331R Practice Site

**Student:** Parker Woolsey
**Semester:** Spring 2026
**Live Site:** https://pwoolls1.github.io/WDD331R/index.html

## About

This repository contains my Practice Site for WDD 331R: Advanced CSS. Throughout the semester, I add new pages and styles as I complete course assignments and explore modern CSS techniques.

The site is automatically deployed to GitHub Pages whenever changes are pushed to the `main` branch.

## Pages

* Home
* Unit 1 — Custom Properties and Nesting
* Unit 2 — Layered Components
* Unit 3 — Visual Effects Showcase
* Unit 3 — Blend Modes
* Unit 4 — Editorial Layout
* Unit 4 — Responsive Card Grid

## CSS Architecture

```text
css/
├── base/
│   ├── elements.css
│   └── reset.css
├── components/
│   ├── buttons.css
│   ├── cards.css
│   ├── forms.css
│   ├── nav.css
│   └── temples.css
├── layout/
│   └── primary.css
├── tokens/
│   ├── colors.css
│   └── variables.css
├── utilities/
│   └── utilities.css
└── main.css
```

## Build Tool

This project uses Lightning CSS to bundle and minify all imported CSS files into a single production stylesheet.

## Build Commands

```bash
npm run build
npm run watch
```

* `npm run build` bundles and minifies the CSS into `dist/styles.css`.
* `npm run watch` automatically rebuilds the CSS while developing.

## Design System

This site uses:

* CSS Layers
* Design Tokens
* Reusable Components
* Responsive Layouts
* Bundled Production Stylesheets
* CSS Grid and Flexbox Layout Patterns

## Tokenized Color System and Dark Mode

This Practice Site supports light mode, dark mode, and a system-default theme option. The theme toggle is available on the homepage and assignment pages. The selected preference is stored in localStorage so it persists between visits.

The main color system is controlled through semantic CSS tokens located in:

```text
unit-2/layered-components/css/tokens/colors.css
```

These tokens define colors for backgrounds, surfaces, text, muted text, accents, borders, links, headers, shadows, and theme controls. Using semantic tokens instead of hardcoded colors allows the entire site to switch themes consistently.

Additional design tokens are located in:

```text
unit-2/layered-components/css/tokens/variables.css
```

These tokens manage spacing, typography, border radii, transitions, icon sizing, and focus states throughout the site.
