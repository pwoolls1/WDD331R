WDD 331R Practice Site
Student: Parker Woolsey
Semester: Spring Semester 2026
Live Site: View Site

About
This repository is my Practice Site for WDD 331R: Advanced CSS.
Each week I add new pages and styles as I work through the course assignments.
The site deploys automatically to GitHub Pages on every push to main.

Pages
Home
Unit 1 — Custom Properties and Nesting
Unit 2 — Layered Components
CSS Architecture
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
Build Tool
This project uses Lightning CSS to bundle and minify all imported CSS files into a single production stylesheet.

Build Commands
npm run build
npm run watch
npm run build bundles and minifies the CSS into dist/styles.css
npm run watch automatically rebuilds the CSS while developing
Design System
This site uses:

CSS layers
design tokens
reusable components
responsive layouts
a bundled production stylesheet
Tokenized Color System and Dark Mode
This Practice Site now supports light mode, dark mode, and a system default theme option. The theme toggle is available on the homepage and assignment pages, and the selected preference is saved with localStorage so it persists between page loads.

The main color system is controlled through semantic CSS tokens. The color tokens live in:

unit-2/layered-components/css/tokens/colors.css

This file defines the background, surface, text, muted text, accent, link, border, header, theme toggle, and shadow colors. The site uses these semantic tokens instead of hardcoded color values so the design can switch between light and dark mode consistently.

The spacing, font, radius, transition, icon, and focus tokens live in:

unit-2/layered-components/css/tokens/variables.css
