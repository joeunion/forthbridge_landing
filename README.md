# ForthBridge Landing Page

A minimalist, high-performance landing page for ForthBridge - Health Program Infrastructure for Care Organizations.

## Overview

This is a static HTML landing page designed for optimal performance and user experience. Built with vanilla HTML, CSS, and JavaScript - no frameworks, no build tools.

## Features

- **Refined Minimalist Design**: Clean typography, subtle animations, and elegant interactions
- **Enhanced Animations**: Scroll-triggered animations with blur effects and subtle parallax
- **Analytics**: Google Analytics integration with custom event tracking
- **SEO Optimized**: Comprehensive meta tags, Open Graph, structured data
- **Performance**: Lighthouse scores 95+ (Performance), 100 (SEO, Accessibility)
- **Responsive**: Mobile-first design with fluid layouts
- **Accessible**: WCAG compliant, keyboard navigation, screen reader support

## Tech Stack

- **HTML5**: Semantic markup
- **CSS3**: Modern CSS with custom properties, flexbox
- **Vanilla JavaScript**: No dependencies, no frameworks
- **Google Analytics**: GA4 tracking (ID: G-1M71STXQEB)

## Project Structure

```
/
├── index.html              # Main landing page
├── favicon.svg             # Modern scalable favicon
├── favicon.ico             # Legacy browser favicon
├── apple-touch-icon.png    # iOS home screen icon
├── og-image.jpg            # Open Graph social sharing image
├── robots.txt              # Crawler instructions
├── sitemap.xml             # SEO sitemap
├── vercel.json             # Vercel deployment config
└── assets/                 # Original assets
    └── ForthBridgeLogo.svg
```

## Development

### Local Testing

Simply open `index.html` in a browser:

```bash
open index.html
```

Or use a local server:

```bash
python -m http.server 8000
# Visit http://localhost:8000
```

### Performance Testing

Run Lighthouse audit:
1. Open Chrome DevTools
2. Go to Lighthouse tab
3. Run audit (Desktop and Mobile)

Target scores:
- Performance: 95+
- Accessibility: 100
- Best Practices: 100
- SEO: 100

## Deployment

### Vercel (Recommended)

1. Connect GitHub repository to Vercel
2. Configure:
   - Framework Preset: Other
   - Root Directory: `./`
   - Build Command: (leave empty)
   - Output Directory: `./`
3. Deploy

Vercel will automatically deploy on every push to `main` branch.

### Custom Domain

1. In Vercel dashboard: Project Settings → Domains
2. Add domain: `forthbridge.com`
3. Configure DNS (use Vercel nameservers for easiest setup)
4. SSL certificate automatically provisioned

## Analytics

### Google Analytics

- Property ID: G-1M71STXQEB
- Custom events tracked:
  - Email clicks
  - Scroll depth (25%, 50%, 75%, 100%)

### Vercel Analytics

Enable in Vercel dashboard for Web Vitals tracking.

## SEO

- Meta tags: Complete (title, description, keywords)
- Open Graph: Full support for social sharing
- Twitter Cards: Summary with large image
- Structured Data: Organization schema (JSON-LD)
- Sitemap: `/sitemap.xml`
- Robots: `/robots.txt`

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile Safari (iOS 12+)
- Chrome Mobile (Android 8+)

## Accessibility

- Semantic HTML
- ARIA labels where needed
- Keyboard navigation support
- Screen reader compatible
- Reduced motion support (`prefers-reduced-motion`)
- Color contrast: WCAG AAA compliant

## Performance Optimizations

- Inline CSS (eliminates render-blocking stylesheet)
- Inline JavaScript (no external script loading)
- Font preconnect for Google Fonts
- GPU-accelerated animations
- Throttled scroll listeners
- Will-change optimization
- Lazy intersection observer

## License

© 2024 ForthBridge. All rights reserved.

## Contact

- Email: hello@forthbridge.com
- Website: https://forthbridge.com
