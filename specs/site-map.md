# FindInsureWise — Site Map

## Recommended Implementation Order

Build shared components first, then pages roughly in funnel order:

| Step | Deliverable | Rationale |
|------|-------------|-----------|
| 1 | Shared: header, footer, newsletter band | Every page depends on these |
| 2 | Shared: CTA Card component | Used in blog sidebar + resource pages |
| 3 | Homepage (desktop) | Primary conversion page, defines visual language |
| 4 | Homepage (mobile) | Separate spec — layout differs significantly |
| 5 | Contact | Simple, validates form + commitment card patterns |
| 6 | FAQ | Accordion + sidebar pattern; reuses newsletter band |
| 7 | Buying Guides | Situation cards + comparison table |
| 8 | Blog Landing | Article grid + featured row |
| 9 | Blog Post | Two-column editorial + sticky sidebar |

---

## Route → Spec → Design Assets

| Route | Spec file | Design folder |
|-------|-----------|---------------|
| `/` | `specs/home.md` | `ux-mockup/home-page/` |
| `/` (mobile) | `specs/home-mobile.md` | `ux-mockup/home-page/` |
| `/contact` | `specs/contact.md` | `ux-mockup/contact-page/` |
| `/faq` | `specs/faq.md` | `ux-mockup/faq-page/` |
| `/buying-guides` | `specs/buying-guides.md` | `ux-mockup/buying-guides-page/` |
| `/blog` | `specs/blog-landing.md` | `ux-mockup/blog-landing-page/` |
| `/blog/:slug` | `specs/blog-post.md` | `ux-mockup/blog-post-page/` |
| Component (no route) | `specs/cta-card.md` | `ux-mockup/shared/` |

---

## Design Asset Index

### `ux-mockup/home-page/` — 15 files

| File | Type | Description |
|------|------|-------------|
| `home-reference-full.png` | reference | Full-page desktop composite |
| `home-reference-1.png` … `home-reference-5.png` | reference | Section-by-section desktop screenshots |
| `home-reference-mobile-1.png` … `home-reference-mobile-6.png` | reference | Section-by-section mobile screenshots |
| `home-hero-desktop.png` | asset | Hero background image (desktop) |
| `home-hero-alt.png` | asset | Alternate hero image |
| `home-footer-contact.png` | asset | Contact/footer area asset |

### `ux-mockup/contact-page/` — 5 files

| File | Type | Description |
|------|------|-------------|
| `contact-reference-full.png` | reference | Full-page reference screenshot |
| `contact-reference-1.png`, `contact-reference-2.png` | reference | Section-level screenshots |
| `contact-hero-1.png`, `contact-hero-2.png` | asset | Hero image assets |

### `ux-mockup/faq-page/` — 5 files

| File | Type | Description |
|------|------|-------------|
| `faq-reference-full.png` | reference | Full-page reference screenshot |
| `faq-reference-1.png` … `faq-reference-3.png` | reference | Section-level screenshots |
| `faq-hero.png` | asset | Hero image asset |

### `ux-mockup/buying-guides-page/` — 12 files

| File | Type | Description |
|------|------|-------------|
| `buying-guides-reference-full.png` | reference | Full-page reference screenshot |
| `buying-guides-reference-1.png` … `buying-guides-reference-3.png` | reference | Section-level screenshots |
| `buying-guides-hero-1.png`, `buying-guides-hero-2.png` | asset | Hero image assets |
| `buying-guides-card-1.png` … `buying-guides-card-6.png` | asset | Six situation card images |

### `ux-mockup/blog-landing-page/` — 4 files

| File | Type | Description |
|------|------|-------------|
| `blog-landing-reference-full.png` | reference | Full-page reference screenshot |
| `blog-landing-reference-1.png`, `blog-landing-reference-2.png` | reference | Section-level screenshots |
| `blog-landing-hero.png` | asset | Hero image asset |

### `ux-mockup/blog-post-page/` — 3 files

| File | Type | Description |
|------|------|-------------|
| `blog-post-reference-full.png` | reference | Full-page reference screenshot |
| `blog-post-reference-1.png`, `blog-post-reference-2.png` | reference | Section-level screenshots |

### `ux-mockup/shared/` — 3 files

| File | Type | Description |
|------|------|-------------|
| `cta-card-reference-full.png` | reference | Component reference screenshot |
| `cta-card-asset-1.png` | asset | Family + home image variant (best default) |
| `cta-card-asset-2.png` | asset | Couple planning variant |
