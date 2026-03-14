# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static personal portfolio website for Karthikeya Sai. No build tools, bundlers, or package managers — just plain HTML and CSS served directly.

## Development

Open `index.html` in a browser to preview. No build or install step required.

## Architecture

- **`index.html`** — Single-page site with all sections: Landing/Home, About Me, Skills, Projects, Contact/Footer. Navigation uses anchor links (`#home`, `#about`, `#skills`, `#projects`, `#contact`).
- **`style.css`** — All styles in one file. Sections are positioned with `position: absolute` and explicit `top` percentages (100%, 170%, 250%, 340%) to stack vertically, rather than using normal document flow.
- **`Assets/`** — All images organized by section:
  - `BackgroundImg/` — Full-section background PNGs (one per section, plus navbar)
  - `SkillsSection/` — Tech stack icon PNGs
  - `Projects/` — Project card images
  - `ConactSection/` — Social media icons (note: directory is misspelled as "Conact")

## Key Dependencies (CDN)

- **Bootstrap 5.3.3** — Grid, navbar (responsive collapse), and form components
- **Google Fonts** — Playfair Display (name/headings), Urbanist (body text)

## Conventions

- Purple/dark color scheme throughout (`#3c00ff`, `#44006e`, `#2a0060`)
- CSS animations: gradient border animation on navbar and profile image, scroll-driven `appear` animation using `animation-timeline: view()`
- Hover effects: translateY(-10px) lift + box-shadow on cards and skill grids
- Media query breakpoint at 768px for mobile layout


Here are some ideas to make your portfolio stand out for that specific role — the sweet spot here is showing all three skills (graphic design, web dev, AI) working *together*, not separately.

---
# FUTURE DESIGNS I WANT.
## 🎨 Visual & Design Upgrades

- **Custom cursor** — a branded cursor that reacts to hover states (grows, changes shape, trails)
- **Smooth page transitions** — using Framer Motion for cinematic section reveals
- **Dark/light mode toggle** — with a satisfying animated switch, shows attention to UX
- **Micro-interactions everywhere** — buttons that bounce, cards that tilt on hover (CSS 3D transforms)
- **Variable font animations** — text that morphs weight/width on scroll or hover
- **Noise/grain texture overlay** — gives a premium editorial feel popular in modern design

---

## ⚛️ React-Specific Power Moves

- **Scroll-driven animations** — using Framer Motion or GSAP, sections animate in as you scroll
- **Live project filter** — filter portfolio pieces by skill tag (Design / Dev / AI) with smooth layout transitions
- **Interactive case study pages** — each project has its own route with before/after sliders, embedded prototypes
- **3D hero section** — using Three.js or React Three Fiber for a subtle 3D element that responds to mouse movement


---

## 📁 Content & Structure

- **"How I work" section** — a short process breakdown (Discover → Design → Build → Ship) specific to AI-integrated projects
- **Metrics on your work** — "Reduced load time by 40%", "Generated 3 design variants using Midjourney + Figma" — numbers build credibility
- **Playground/Lab section** — a sandbox for experimental work, showing curiosity and range
- **Testimonials or a "Collab" section** — even one or two short quotes go a long way

---

## ⚡ Performance & Tech Flex

- **Perfect Lighthouse score** — 100s across the board signals you care about craft
- **Lottie animations** — lightweight, scalable animations imported from After Effects
- **Skeleton loaders** — shows you think about perceived performance
- **Open Graph previews** — when recruiters share your link, a beautiful card preview appears

---
