# GEMINI.md

This file provides context and instructions for AI assistants working in this repository.

## Project Overview

This is a static personal portfolio website for Karthikeya Sai. It is built using plain HTML, CSS, and vanilla JavaScript without the need for build tools, bundlers, or package managers. 

The website is a single-page application with the following key sections:
- Landing/Home
- About Me
- Skills
- Process & Metrics
- Projects (with interactive category overlays for Web, AI, and Design)
- Contact/Footer

**Key Technologies:**
- **HTML5 & CSS3** for structure and styling.
- **Vanilla JavaScript** for interactive elements like the custom cursor and project overlays.
- **GSAP (GreenSock)** for scroll-driven animations and reveal effects.
- **HTML Canvas** for the fluid gradient background animation.
- **Bootstrap 5.3.3** (via CDN) for grid layout, responsive navbar, and form components.
- **Google Fonts** (Playfair Display, Urbanist).

## Building and Running

This project does not require any build steps, package installations, or local servers to run basic features.

To view the project locally:
1. Open the `index.html` file directly in a modern web browser.
2. Alternatively, you can use a simple local server (like VS Code Live Server or Python's `http.server`) to avoid potential CORS issues if loading external local assets dynamically in the future.

## Architecture & Structure

- `index.html`: Contains the entire structure of the single-page site. Navigation uses anchor links (`#home`, `#about`, etc.).
- `style.css`: Contains all custom styles. Sections are stacked vertically using standard document flow and specific sizing. Includes custom cursor styles and complex CSS animations (e.g., gradient borders).
- `Assets/`: Directory for all images, organized by section (`BackgroundImg`, `SkillsSection`, `Projects`, `ConactSection` [sic]).

## Development Conventions

- **Styling:** The design uses a dark theme with purple accents (e.g., `#3c00ff`, `#44006e`, `#2a0060`, `#a855f7`).
- **Animations:** Heavy use of GSAP for scroll animations (`.reveal-left`, `.reveal-right`, `.reveal-up`, `.reveal-weight`) and CSS keyframes for continuous effects (gradients, custom cursor).
- **Responsive Design:** A primary media query breakpoint exists at `768px` for mobile layout adjustments.
- **Simplicity:** Maintain the zero-build-step philosophy unless a major architectural shift (like migrating to React/Next.js as hinted in `CLAUDE.md`) is explicitly requested. Additions should ideally use vanilla JS, CSS, or lightweight CDN scripts.

## Future Goals (from CLAUDE.md)
The project aims to showcase skills in graphic design, web dev, and AI. Future design aspirations include:
- Smooth page transitions (e.g., Framer Motion).
- Dark/light mode toggle.
- Advanced micro-interactions (CSS 3D transforms).
- Variable font animations.
- Potential migration to React-specific technologies (Scroll-driven animations, live filtering, 3D elements with Three.js).
