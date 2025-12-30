# Project Structure

## Root Level

```
├── src/                    # Source code
├── public/                 # Static assets
├── dist/                   # Built output (generated)
├── node_modules/           # Dependencies
├── .astro/                 # Astro cache and types
├── .kiro/                  # Kiro configuration
├── astro.config.mjs        # Astro configuration
├── tailwind.config.mjs     # Tailwind configuration
├── server.js               # Production Express server
├── package.json            # Dependencies and scripts
└── README.md               # Project documentation
```

## Source Structure (`src/`)

```
src/
├── components/             # Reusable UI components
│   ├── Header.astro       # Site navigation
│   ├── Hero.astro         # Landing page hero section
│   ├── Features.astro     # Feature showcase
│   ├── SocialProof.astro  # Testimonials/logos
│   └── CTA.astro          # Call-to-action sections
├── layouts/               # Page layout templates
├── pages/                 # Route-based pages
│   └── index.astro        # Homepage
└── env.d.ts              # TypeScript environment types
```

## Component Organization

- **Components**: Single-responsibility UI components in `.astro` format
- **Layouts**: Shared page templates and structure
- **Pages**: File-based routing (each file = route)

## Naming Conventions

- **Files**: PascalCase for components (`Hero.astro`, `Features.astro`)
- **CSS Classes**: Tailwind utility classes with responsive prefixes
- **Colors**: Use `primary-*` variants from custom theme

## Asset Management

- **Static Assets**: Place in `public/` directory (logo.svg, images)
- **Built Assets**: Generated in `dist/assets/` during build
- **Fonts**: Inter (sans) and JetBrains Mono (mono) from theme

## Page Structure Pattern

```astro
---
// Component imports at top
import Layout from '../layouts/Layout.astro';
import Component from '../components/Component.astro';
---

<Layout title="Page Title">
  <Component />
  <!-- Additional components -->
</Layout>
```

## Styling Approach

- Utility-first with Tailwind CSS
- Component-scoped styles when needed
- Responsive design with mobile-first approach
- Custom primary color palette for brand consistency