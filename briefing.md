# Plastic-Craft Products -- Claude Code Project Briefing

Use this file at the start of every Claude Code session. Reference it for all design, content, and development work related to plastic-craft.com.

---

## Company Overview

| Field | Detail |
|-------|--------|
| **Company** | Plastic-Craft Products |
| **Type** | Family-owned B2B plastic fabrication and distribution company |
| **Founded** | 1934 |
| **Location** | West Nyack, NY |
| **Website** | plastic-craft.com |
| **Certifications** | ISO 9001:2015 | AS9100D |
| **Platform** | WordPress + WooCommerce + Elementor (Pro) |
| **Audience** | Engineers, procurement specialists, industrial buyers |

---

## Brand Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Navy | `#1B365D` | Primary -- headings, headers, nav, buttons, links |
| Gold | `#C8922A` | Accent -- CTAs, highlights, hover states, decorative details |
| White | `#FFFFFF` | Backgrounds, text on dark surfaces |
| Light Gray | `#F5F5F5` | Section backgrounds, alternating rows |
| Dark Gray | `#333333` | Body text |
| Medium Gray | `#666666` | Secondary text, captions |

### Color Rules

- Light backgrounds only -- no dark/black background sections
- Navy is for text and structural elements, NOT large background fills
- Gold is an accent -- use sparingly for maximum impact
- Buttons: Navy background + white text, gold hover state
- Maintain WCAG AA contrast ratios for accessibility

---

## Typography

| Element | Font | Weight |
|---------|------|--------|
| H1-H4 Headings | Montserrat | 600-700 (SemiBold/Bold) |
| Body Text | Lora | 400 (Regular) |
| Navigation | Montserrat | 500 (Medium) |
| Buttons | Montserrat | 600 (SemiBold) |
| Captions / Small | Lora | 400 (Regular) |

### Font Size Scale

- H1: 36-42px
- H2: 28-32px
- H3: 22-26px
- H4: 18-20px
- Body: 16px, line-height 1.6
- Never use more than 2 font families (Montserrat + Lora only)

### Font Import (for HTML artifacts)

```html
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@500;600;700&family=Lora:wght@400&display=swap" rel="stylesheet">
```

---

## Design Principles

1. **Clean and professional** -- inspires confidence for engineers and procurement buyers
2. **No emojis** -- anywhere on the website, ever
3. **Light and airy** -- generous white space, light backgrounds
4. **Data-driven** -- use spec tables, property charts, and comparison grids for technical content
5. **Mobile responsive** -- every design must work on mobile
6. **CTA visibility** -- every page needs a clear call to action above the fold
7. **Consistent imagery** -- product photography: clean, well-lit, white or neutral backgrounds

---

## CSS Starter Variables

Use these in every HTML artifact to stay on-brand instantly:

```css
:root {
  --navy:        #1B365D;
  --gold:        #C8922A;
  --white:       #FFFFFF;
  --light-gray:  #F5F5F5;
  --dark-gray:   #333333;
  --mid-gray:    #666666;

  --font-heading: 'Montserrat', sans-serif;
  --font-body:    'Lora', serif;
}
```

---

## Team Reference

| Person | Role |
|--------|------|
| Gabrielle | Content Marketing & Brand Catalog Manager |
| Jordan | WordPress / Elementor Developer |
| Dane | Infrastructure / NAS Administrator |
| Nibi | Controller / Accountant |
| Mo | Team member |

---

## Tech Stack Reference

| System | Details |
|--------|---------|
| CMS | WordPress + Elementor Pro |
| E-Commerce | WooCommerce |
| Hosting | Cloudways |
| CDN/Security | Cloudflare |
| SEO Plugin | Rank Math |
| NAS | Synology (192.168.1.23) |
| Database | PostgreSQL (Docker on NAS) |
| Marketplaces | Amazon, eBay, Walmart (8,000+ SKUs) |
| Certifications | ISO 9001:2015 |

---

## Active Projects (as of March 2026)

- **Website rebuild** -- plastic-craft.com full restructure
- **Capabilities pages** -- 19 pages with Rank Math SEO, 301 redirects, schema markup, internal linking
- **Industries section** -- 17 pages under /industries/, redirect mapping complete
- **WooCommerce catalog expansion** -- new products with Request a Quote (YITH plugin) strategy
- **Google Merchant Center feed** -- ~181K cut-to-size SKUs via Python script on NAS (standalone feed, not loaded into WooCommerce)

---

## How to Start a Claude Code Session

Paste this at the top of every new session:

> Read briefing.md first. This contains brand colors, typography, design rules, and project context for Plastic-Craft Products. Apply all brand standards to everything you build. Ask me what we're working on today.

---

*Last updated: March 2026*
