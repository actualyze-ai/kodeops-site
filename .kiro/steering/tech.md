# Technology Stack

## Framework & Build System

- **Astro 4.15+**: Static site generator with component islands architecture
- **Node.js 18+**: Required runtime environment
- **Express**: Production server for Heroku deployment

## Styling & UI

- **Tailwind CSS 3.4+**: Utility-first CSS framework
- **@tailwindcss/typography**: Enhanced typography plugin
- **Custom Design System**: Primary color palette (blue variants), Inter font family

## Development & Deployment

- **Static Output**: Pre-rendered at build time for optimal performance
- **Heroku**: Production hosting with Express server
- **Cloudflare Pages**: Automatic deployment on main branch push to kodeops.dev

## Common Commands

```bash
# Development
npm install          # Install dependencies
npm run dev         # Start development server (localhost:4321)

# Building
npm run build       # Build static site to dist/
npm run preview     # Preview built site locally

# Production
npm start           # Start Express server (uses server.js)
```

## Configuration Files

- `astro.config.mjs`: Astro configuration with Tailwind and sitemap
- `tailwind.config.mjs`: Custom theme, colors, and typography
- `server.js`: Express server for production deployment
- `package.json`: Dependencies and build scripts

## Performance Considerations

- Static site generation for fast loading
- Image optimization built-in
- SEO optimization with sitemap generation
- Component-based architecture for maintainability