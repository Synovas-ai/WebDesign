# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## What This Repository Is

This is a **design specification repository** for FindInsureWise (a Synova product), not a code project. There are no build commands or tests.

```
docs/
├── specs/          ← 9 .md files — one per page/component + site-map index
└── design/
    ├── shared/             ← CTA Card (used across pages)
    ├── home-page/          ← desktop + mobile references together
    ├── contact-page/
    ├── faq-page/
    ├── buying-guides-page/
    ├── blog-landing-page/
    └── blog-post-page/
```

Each spec file contains copy, section structure, inline CSS values, and responsive rules. Each design folder contains:
- `{page}-reference-full.png` — full-page composite
- `{page}-reference-{n}.png` — section-level screenshots for visual QA
- `{page}-hero-{n}.png` / `{page}-card-{n}.png` / `{page}-asset-{n}.png` — production image assets

When implementing, read the spec first, then use reference images to validate visual fidelity. Start with `docs/specs/site-map.md` for implementation order and the full route → spec → asset mapping.

---

## Page Inventory

| Spec file | Route | Content |
|-----------|-------|---------|
| `specs/home.md` | `/` | Full desktop landing page |
| `specs/home-mobile.md` | `/` (mobile) | Mobile-specific layout (differs significantly from desktop) |
| `specs/contact.md` | `/contact` | Hero, form, commitment card, direct contact cards, newsletter band |
| `specs/faq.md` | `/faq` | Accordion groups, sticky sidebar (topic nav, soft CTA, popular questions) |
| `specs/buying-guides.md` | `/buying-guides` | Situation cards, 3-column comparison table, calculator CTA strip |
| `specs/blog-landing.md` | `/blog` | Featured row, topic filter chips, article grid |
| `specs/blog-post.md` | `/blog/:slug` | Editorial layout, sticky sidebar (TOC, related articles, quote CTA, email) |
| `specs/cta-card.md` | component | Reusable quote CTA card for blog sidebar, mid-article blocks, resource pages |
| `specs/site-map.md` | — | Master index: implementation order + full route → spec → asset table |

---

## Design System

### Colors

```css
/* Backgrounds */
--bg-page:        #F6F8F5;
--bg-card:        #FFFFFF;
--bg-dark-footer: linear-gradient(135deg, #041F17, #0A3527, #0E4A35);

/* Brand greens */
--green-dark:     #0B3A2B;   /* hero text, headings */
--green-action:   #0E5B37;   /* primary buttons */
--green-accent:   #27500A;   /* eyebrows, check icons */
--green-light:    #16723A;   /* inline links, labels */

/* Gold */
--gold:           #C9972A;   /* primary CTA buttons */
--gold-hover:     #BF7F10;
--gold-bg:        #FEF6E7;   /* TL;DR callout background */

/* Borders & muted */
--border:         #D8E2D4;
--text-1:         #2C3B2A;
--text-2:         #5A6B58;
--text-3:         #8A9B88;
```

### Typography

- **Serif** (`Editorial Serif`, Georgia fallback): all H1/H2 headings, large serif display text
- **Sans-serif** (modern, e.g. Inter): body copy, buttons, labels
- **Eyebrows**: `font-size: 14–16px; font-weight: 600–700; letter-spacing: 0.06–0.12em; text-transform: uppercase; color: var(--green-accent)`
- **H1 desktop**: 64–72px; **H1 mobile**: 40–46px
- **H2**: 38–54px desktop; 32px mobile
- **Body**: 18–22px desktop; 17–18px mobile; `line-height: 1.7–1.9`

### Spacing Rhythm

- Section vertical padding: `72–88px` desktop, `56px` mobile (`padding: 56px 20px`)
- Max content width: `1180–1400px`; always `margin: 0 auto`
- Cards: `border-radius: 18–20px`; `box-shadow: 0 8px 24px rgba(18,61,42,0.08)`
- Inputs: `height: 56–58px; border-radius: 12px; border: 1px solid #E7ECE8`
- Primary CTA buttons: `background: var(--gold); border-radius: 12–14px; height: 54–58px; font-weight: 600`
- Dark action buttons: `background: var(--green-action); color: #FFFFFF`

### Responsive Breakpoints

- **Tablet** `< 1100px`: multi-column grids collapse to 1 or 2 columns; sidebar moves below content
- **Mobile** `< 768px`: single column; hero images max-height 320–360px; all buttons full-width; sticky bottom CTA on blog posts

---

## Recurring Patterns Across Pages

**Header** (identical across all pages): sticky, 84px height, white bg, `border-bottom: 1px solid #D8E2D4`, logo left, centered nav, gold CTA button right.

**Footer** (identical across all pages): dark green gradient, 4-column layout (Brand + tagline, Company links, Resources links, Legal links) with a gold outline "Get a Free Quote →" button.

**Hero layout**: desktop always two-column (`grid-template-columns: 1fr 1fr`), eyebrow + H1 + supporting copy + CTA left, lifestyle photo right. Mobile: single column, image becomes background or stacks below.

**Newsletter band**: full-width horizontal strip (`#F5F8F2` bg, `border-radius: 18px`), icon + headline + subtext left, email field + subscribe button right.

**CTA Copy conventions**:
- Primary: `Get My Free Quote →`
- Secondary: `Compare My Options →`, `Use Coverage Calculator →`
- Trust note: `🔒 Your information is safe and secure.`

---

## Image & Asset Direction

All photography should be: realistic (not AI-generated hands), warm natural light, age 28–45, authentic emotion, clean upscale-but-relatable environments. Avoid stock-photo smiles, staged poses, cluttered backgrounds.

Asset exports: card images at `1080×660px` (16:10 ratio). Hero images full-width at `height: 520–620px`. Mobile hero background images scaled to `height: 360px`.
