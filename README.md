# GlobalPetSits

Trusted pet and house sitter landing page for Alex Nodelman. 5-star reviews across Asia and Europe.

## Features

- Responsive single-page design
- Postcard homecoming animation system with GSAP scroll triggers
- Dark mode support with localStorage persistence
- Full accessibility compliance (WCAG 2.1)
- SEO optimised with schema markup and OG tags
- Performance optimised (inline CSS/JS, WebP images, Intersection Observer)

## Technology Stack

- HTML5 semantic markup
- CSS3 with CSS custom properties for theming
- Vanilla JavaScript with GSAP animations
- WebP image format for performance
- Cloudflare Pages deployment

## Structure

```
globalpetsits/
├── index.html          # Single-file app with inline CSS/JS
├── images/             # Optimised WebP images
├── robots.txt          # SEO indexing
├── sitemap.xml         # Sitemap for search engines
├── wrangler.jsonc      # Cloudflare Pages config
└── README.md           # This file
```

## Deployment

### Cloudflare Pages

Deploy via `wrangler publish`:

```bash
npm install -g wrangler
wrangler publish
```

Environment:
- Production: `globalpetsits.com`
- Staging: `globalpetsits.pages.dev`

### Configuration

Edit `wrangler.jsonc` to update:
- Domain routing
- Asset includes/excludes
- Compatibility date

## Animation System

The postcard homecoming system uses CSS transitions with JavaScript Intersection Observer to trigger reveals as elements enter the viewport.

Animation classes:
- `.pc-arrive` — Tilted arrival with settle
- `.pc-up` — Bottom-to-top enter
- `.pc-left` / `.pc-right` — Side entrances
- `.pc-scale` — Zoom + fade

## Theming

Dark mode toggle via `.theme-btn`. Theme persists in `localStorage['an-theme']`.

CSS variables control colour palette:
- Light mode: Warm parchment (#F5EDE0) + terracotta (#C4622D)
- Dark mode: Deep charcoal (#141210) + warm terracotta (#D47248)

## Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile Safari 14+

## License

Copyright 2025 Alex Nodelman. All rights reserved.

## Contact

WhatsApp: +972 523 949 964

Full profile: [TrustedHouseSitters](https://www.trustedhousesitters.com/house-and-pet-sitters/israel/southern-district/ashdod/l/4613767/)
