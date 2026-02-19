# KC Services Website

A professional bookkeeping and financial services website built with **Eleventy (11ty)** static site generator.

## Design
- **Aesthetic**: Editorial Warm Luxury — deep forest green, warm cream, gold accents
- **Fonts**: Cormorant Garamond (display) + Outfit (body) + DM Mono (accents)
- **Features**: Animated hero with floating stat cards, layered about images, scroll reveal animations, mobile-responsive

## Project Structure

```
kc-services/
├── .eleventy.js          # 11ty configuration
├── package.json          # Dependencies & scripts
├── index.njk             # Main homepage template (Nunjucks)
├── index.html            # Standalone HTML preview (works without 11ty)
├── _includes/
│   └── base.njk          # Base layout (nav + footer)
├── _data/
│   └── site.json         # All site content (services, pricing, testimonials)
├── css/
│   └── style.css         # Full stylesheet
└── js/
    └── main.js           # Interactivity (nav scroll, reveal, form, etc.)
```

## Getting Started

### Install dependencies
```bash
npm install
```

### Development server (with hot reload)
```bash
npm start
# Opens at http://localhost:8080
```

### Production build
```bash
npm run build
# Output in _site/
```

## Updating Content

All site content (services, pricing, testimonials, contact info) lives in **`_data/site.json`** — no template editing needed for content changes.

## Customization

- **Colors**: Edit CSS variables at the top of `css/style.css`
- **Images**: Replace Unsplash URLs in `index.njk` with your own images
- **Content**: Edit `_data/site.json`
- **Layout**: Modify `_includes/base.njk` for nav/footer changes

## Standalone Preview

Open `index.html` directly in a browser — no server required. This file is a self-contained version for previewing or deployment without a build step.
