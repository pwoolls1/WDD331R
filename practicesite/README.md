# WDD 331R Practice Site

**Student:** Parker Woolsey  
**Semester:** Spring Semester 2026  
**Live Site:** [View Site](https://pwoolls1.github.io/WDD331R/index.html)

## About

This repository is my Practice Site for WDD 331R: Advanced CSS.  
Each week I add new pages and styles as I work through the course assignments.  
The site deploys automatically to GitHub Pages on every push to `main`.

## Pages

- [Home](index.html)
- [Unit 1 — Custom Properties and Nesting](unit-1/custom-properties/index.html)
- [Unit 2 — Layered Components](unit-2/layered-components/index.html)

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

- `npm run build` bundles and minifies the CSS into `dist/styles.css`
- `npm run watch` automatically rebuilds the CSS while developing

## Design System

This site uses:
- CSS layers
- design tokens
- reusable components
- responsive layouts
- a bundled production stylesheet