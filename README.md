# FindInsureWise — Web Design

HTML/CSS implementation of the FindInsureWise website, a term life insurance product by [Synova](https://github.com/Synovas-ai).

**Live preview:** https://synovas-ai.github.io/WebDesign/

---

## Pages

| Page | URL |
|------|-----|
| Portfolio index | `/` |
| Home | `/pages/home.html` |
| Buying Guides | `/pages/buying-guides.html` |
| FAQ | `/pages/faq.html` |
| Contact | `/pages/contact.html` |
| Blog | `/pages/blog-landing.html` |
| Blog Post | `/pages/blog-post.html` |
| Design System | `/design-system/design-system.html` |

## Structure

```
WebDesign/
├── index.html              ← Portfolio page (start here)
├── pages/
│   ├── shared.css          ← Design tokens + all shared components
│   ├── home.html
│   ├── buying-guides.html
│   ├── faq.html
│   ├── contact.html
│   ├── blog-landing.html
│   └── blog-post.html
├── design-system/
│   ├── design-system.html  ← Living style guide
│   └── design-system.md   ← Token reference
├── specs/                  ← Page-by-page copy and layout specs
└── ux-mockup/              ← Reference screenshots and image assets
```

## Design System

All pages share a single `shared.css` with CSS custom properties for colors, typography, spacing, and pre-built components (header, footer, cards, buttons, forms, accordion, comparison table, etc.).

Key tokens:

| Token | Value | Use |
|-------|-------|-----|
| `--color-heading` | `#1b2c20` | H1–H4, strong text |
| `--color-gold` | `#cf9010` | Primary CTA buttons |
| `--color-action` | `#2c5f3a` | Secondary buttons, links |
| `--color-bg-section` | `#f5f7f4` | Alternate section backgrounds |
| `--font-serif` | Playfair Display | All headings |
| `--font-sans` | Inter | Body, buttons, labels |
