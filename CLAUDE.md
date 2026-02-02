# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Interactive Dutch-language educational web tutorial teaching Business Administration students about emergent/organic strategy vs. classical strategy approaches. Built with vanilla HTML, CSS, and JavaScript — no frameworks or dependencies.

## Development

**Run locally:**
```bash
python -m http.server
# or
npx http-server
```
Then open http://localhost:8000 (or the port shown).

No build process, npm install, or compilation required. Open `index.html` directly in a browser also works (though some video features may need a server).

## Architecture

Single-page static site with three files:
- `index.html` — Tutorial content with 5 sections, quiz, and interactive elements
- `styles.css` — CSS variables, Grid/Flexbox layouts, responsive breakpoint at 768px
- `script.js` — Intersection Observer for scroll detection, quiz logic, feedback loop animation

**Key interactive components:**
- Progress bar (top) — scroll-based reading progress
- Navigation dots (right sidebar) — section jumping
- Concept cards — hover tooltips with definitions
- Feedback loop visualization — auto-play animation showing complexity dynamics
- Knowledge quiz — 3 questions with instant feedback and scoring

## Content Language

All tutorial content is in Dutch. The tutorial covers:
- Klassieke Strategie (Vision → Mission → Strategy)
- VUCA concept
- Organische/Emergent Strategy (Mintzberg)
- Feedback loops in complex systems
- Classical vs. Organic comparison

## Deployment

Ready for any static hosting (GitHub Pages, Netlify, Vercel). Video files (.mp4) are embedded locally and must be included in deployment.
