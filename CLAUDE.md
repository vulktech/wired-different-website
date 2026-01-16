# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build & Development Commands

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build locally

## Architecture

This is an Astro 5.x static site project for a "coming soon" landing page.

**Tech Stack:**
- Astro (static site generator)
- TypeScript (strict mode)
- Tailwind CSS (via CDN)
- Google Fonts (Space Grotesk)

**Project Structure:**
- `src/pages/` - Astro pages (file-based routing)
- `public/` - Static assets served as-is
- `astro.config.mjs` - Astro configuration
- `tsconfig.json` - TypeScript config extending Astro's strict preset

**Current State:** Single-page site with no components directory yet. As the project grows, standard Astro conventions apply:
- `src/components/` for reusable Astro/framework components
- `src/layouts/` for page layouts
- `src/content/` for content collections (blog posts, etc.)

**Styling Approach:** Dark theme with purple/indigo gradients. Custom CSS animations are defined inline in page files alongside Tailwind utility classes.
