# WDD 331R Practice Site

**Student:** Parker Woolsey  
**Semester:** Spring 2026  
**Live Site:** https://pwoolls1.github.io/WDD331R/index.html

## About

This repository contains my portfolio for WDD 331R: Advanced CSS. Throughout the semester, I built responsive, accessible webpages while exploring modern CSS techniques. The site now serves as a professional portfolio that highlights my strongest work, provides quick access to every assignment, and demonstrates the design system and component architecture developed throughout the course.

Recent additions include advanced CSS Grid techniques using **subgrid**, component-level responsiveness with **container queries**, **sticky positioning**, and a redesigned portfolio homepage featuring a hero section, featured work, and an organized project archive.

The site is automatically deployed to GitHub Pages whenever changes are pushed to the `main` branch.

---

## Portfolio Organization

The homepage serves as the main entry point to the portfolio with a personal introduction, featured projects, and links to my resume and contact page. Coursework completed throughout the semester remains organized and accessible through the project archive, ensuring every assignment can still be reached while presenting the site as a polished portfolio rather than a homework log.

## Pages

- [Home](https://pwoolls1.github.io/WDD331R/index.html)
- [Resume / CV](https://pwoolls1.github.io/WDD331R/resume.html)
- [Contact](https://pwoolls1.github.io/WDD331R/contact.html)
- Unit 1 — Custom Properties and Nesting
- Unit 2 — Layered Components
- Unit 3 — Visual Effects Showcase
- Unit 3 — Blend Modes
- Unit 4 — Editorial Layout
- Unit 4 — Responsive Card Grid with Subgrid
- Unit 4 — Container Query Demo
- Unit 4 — Sticky Module Demo
- Form Controls
- Meaningful Motion
- SVG CSS Demo

---

## Portfolio Improvements

For the Unit 7 Portfolio Launch, I redesigned the homepage into a professional landing page with a hero section, featured projects, and an organized project archive. I also refined the resume and contact pages, improved shared navigation and reusable components, and applied a consistent visual design system across the site using CSS layers, design tokens, and reusable components.

---

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
│   ├── homepage.css
│   ├── icons.css
│   ├── theme-toggle.css
│   ├── effects.css
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

---

## Build Tool

This project uses Lightning CSS to bundle and minify all imported CSS files into a single production stylesheet.

## Build Commands

```bash
npm run build
npm run watch
```

- `npm run build` bundles and minifies the CSS into `dist/styles.css`.
- `npm run watch` automatically rebuilds the CSS while developing.

---

## Design System

This site uses:

- CSS Layers
- Design Tokens
- Reusable Components
- Responsive Layouts
- Bundled Production Stylesheets
- CSS Grid and Flexbox Layout Patterns
- Subgrid for aligned card layouts
- Container Queries for component-based responsiveness
- Sticky Positioning for persistent interface modules

---

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

---

## Typography System

This site uses a modular typography scale controlled through `css/tokens/variables.css`. I replaced the older fixed font-size tokens with a larger type scale that includes small text, body text, headings, and display text.

The larger type sizes use `clamp()` so headings scale fluidly between smaller and larger viewport widths. Smaller text sizes stay fixed so captions and body text remain readable.

The type system also uses semantic role tokens, such as:

- `--font-size-body`
- `--font-size-caption`
- `--font-size-heading-sm`
- `--font-size-heading-md`
- `--font-size-heading-lg`
- `--font-size-display`

This allows the site to reference typography by purpose instead of by raw size. I also added Merriweather as a custom heading font with `display=swap`, while keeping a system sans-serif stack for body text.

---

## Major Features

- Added `resume.html` with semantic resume/CV content.
- Added `contact.html` with a styled contact form.
- Added print styles for a clean resume PDF.
- Updated form controls to use the site accent color.
- Audited token files for unused or duplicate custom properties.
- Redesigned the homepage into a professional portfolio landing page.
- Added featured project sections and a project archive.
- Refined reusable buttons, cards, navigation, and shared components.
- Improved spacing, typography, and responsive layouts across the portfolio.
- Added Meaningful Motion with reduced-motion accessibility support.
- Added CSS-styled SVG demonstrations.

### Meaningful Motion

**Meaningful Motion with Reduced-motion Support** (`/unit-6/motion/index.html`) demonstrates explicit transitions, custom cubic-bezier easing, staggered card animations, keyframe animations, and reduced-motion accessibility support.