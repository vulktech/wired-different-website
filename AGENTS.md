# AGENTS.md

This file provides guidance for AI coding agents (Claude Code, Cursor, etc.) when working with this repository.

## Project Overview

"I'm Wired Different" coming soon landing page - Astro 5.x static site with animated gradients, email signup, and progress tracking.

## Package Manager

**IMPORTANT**: Always use `pnpm` for this project (not npm or yarn).

```bash
pnpm install    # Install dependencies
pnpm dev        # Development server
pnpm build      # Production build
pnpm preview    # Preview production build
```

## Architecture & Tech Stack

**Framework**: Astro 5.x (static site generator)
**Language**: TypeScript (strict mode enabled)
**Styling**: Tailwind CSS 3.x (installed package, not CDN)
**Fonts**: Google Fonts - Space Grotesk

## Project Structure

```
src/
├── components/           # Reusable Astro components
│   ├── BackgroundEffects.astro  # Animated gradient backgrounds
│   ├── EmailSignup.astro        # Email capture form
│   ├── Footer.astro             # Site footer with social links
│   ├── Hero.astro               # Main hero section
│   └── ProgressBar.astro        # Progress indicator (66%)
├── layouts/
│   └── BaseLayout.astro         # Base HTML layout with SEO meta tags
└── pages/                       # File-based routing
    └── index.astro              # Homepage (coming soon page)

public/                          # Static assets served as-is
```

## Design System

**Theme**: Dark mode with purple/indigo gradients
**Colors**:
- Primary: Purple (#9333ea, #a855f7)
- Secondary: Indigo (#4f46e5, #6366f1)
- Background: Dark gray (#0a0a0a, #1a1a1a)

**Typography**: Space Grotesk font family (400, 500, 700 weights)

**Animation Patterns**:
- Floating animations for visual elements
- Gradient shifts for backgrounds
- Smooth transitions on hover states
- Custom keyframe animations defined inline in components

## Development Guidelines

1. **Component Structure**: Keep components small and focused. Each component should have a single responsibility.

2. **Styling**: Use Tailwind utility classes. For complex animations, define CSS keyframes in `<style>` blocks within the component.

3. **TypeScript**: Strict mode is enabled. Ensure all props and data are properly typed.

4. **Astro Patterns**:
   - Use component props for configuration
   - Leverage Astro's component script section for data processing
   - Keep client-side JavaScript minimal (currently zero JS shipped)

5. **Performance**: This is a static site. All HTML is pre-rendered at build time.

## Current State

Single-page coming soon site with:
- Hero section with animated title
- Email signup form (currently frontend only)
- Progress bar showing 66% completion
- Animated gradient background effects
- Footer with placeholder social links

## Future Expansion

As the project grows, follow standard Astro conventions:
- `src/content/` for content collections (blog, etc.)
- `src/utils/` for shared utility functions
- `src/types/` for TypeScript type definitions
- Consider adding API routes in `src/pages/api/` for email signup backend
