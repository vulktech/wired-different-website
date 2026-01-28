# I'm Wired Different - Coming Soon

A sleek, animated landing page for the "I'm Wired Different" brand, built with Astro 5.x.

## Features

- Modern "coming soon" landing page with animated gradient backgrounds
- Email signup with progress tracking
- Fully responsive design with dark theme
- Purple/indigo gradient aesthetic
- Smooth animations and visual effects
- TypeScript for type safety

## Tech Stack

- **Astro 5.x** - Static site generator
- **TypeScript** - Strict mode enabled
- **Tailwind CSS** - Utility-first CSS framework
- **Google Fonts** - Space Grotesk font family

## Getting Started

### Prerequisites

- Node.js 18+ or 20+
- pnpm (preferred package manager)

### Installation

```bash
pnpm install
```

### Development

```bash
pnpm dev
```

Visit `http://localhost:4321` to view the site.

### Build

```bash
pnpm build
```

Builds the site for production to the `dist/` directory.

### Preview

```bash
pnpm preview
```

Preview the production build locally.

## Project Structure

```
wired-different-website/
├── src/
│   ├── components/        # Reusable Astro components
│   │   ├── BackgroundEffects.astro
│   │   ├── EmailSignup.astro
│   │   ├── Footer.astro
│   │   ├── Hero.astro
│   │   └── ProgressBar.astro
│   ├── layouts/           # Page layouts
│   │   └── BaseLayout.astro
│   └── pages/             # File-based routing
│       └── index.astro
├── public/                # Static assets
├── astro.config.mjs       # Astro configuration
├── tailwind.config.mjs    # Tailwind configuration
└── tsconfig.json          # TypeScript configuration
```

## Design System

- **Theme**: Dark mode with purple/indigo gradients
- **Typography**: Space Grotesk font family
- **Animations**: Custom CSS keyframe animations for floating effects and gradients
- **Components**: Modular Astro components for maintainability

## License

All rights reserved.