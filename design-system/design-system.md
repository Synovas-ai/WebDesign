# FindInsureWise Design System

Derived from `docs/specs/home.md` and `docs/specs/home-mobile.md`. All tokens apply site-wide.

---

## Color Palette

### Brand Greens

| Token | Hex | Usage |
|-------|-----|-------|
| `--color-heading` | `#123d2a` | H1, H2, display text |
| `--color-footer-bg` | `#0f3a25` | Footer + final CTA background |
| `--color-action` | `#0e5b37` | Dark action buttons (Contact Us, Subscribe) |
| `--color-eyebrow` | `#1f7a45` | Eyebrow labels, inline links |
| `--color-accent` | `#27500a` | Check icons, active states |

### Gold

| Token | Hex | Usage |
|-------|-----|-------|
| `--color-gold` | `#c98a1e` | Primary CTA buttons |
| `--color-gold-hover` | `#b07618` | Primary CTA hover state |
| `--color-gold-bg` | `#fef6e7` | TL;DR callout background |
| `--color-gold-border` | `#e8c98b` | TL;DR callout border |

### Neutrals

| Token | Hex | Usage |
|-------|-----|-------|
| `--color-bg-page` | `#f6f8f5` | Page / section background |
| `--color-bg-card` | `#ffffff` | Cards, inputs |
| `--color-border` | `#d8e2d4` | Card borders, dividers, header bottom |
| `--color-text-1` | `#2c3b2a` | Primary body text |
| `--color-text-2` | `#5a6b58` | Supporting / secondary copy |
| `--color-text-3` | `#8a9b88` | Muted labels, timestamps, captions |

---

## Typography

### Typefaces

- **Serif** — `"Editorial Serif"`, Georgia, serif — all H1 / H2 / display headings
- **Sans-serif** — Inter, system-ui, sans-serif — body copy, buttons, labels, nav

### Scale

| Element | Desktop | Mobile | Properties |
|---------|---------|--------|------------|
| H1 | 64–72px | 40px | `font-family: serif; font-weight: 600; line-height: 1.08; color: var(--color-heading)` |
| H2 | 40–54px | 32px | `font-family: serif; font-weight: 600; line-height: 1.08` |
| H3 | 28–32px | 24px | `font-family: serif; font-weight: 600; line-height: 1.2` |
| Eyebrow | 12–16px | 12px | `font-weight: 700; letter-spacing: 0.12em; text-transform: uppercase; color: var(--color-eyebrow)` |
| Body | 18–22px | 16–17px | `line-height: 1.7–1.9; color: var(--color-text-1)` |
| Body muted | 18–22px | 16–17px | `color: var(--color-text-2)` |
| Caption / meta | 14px | 14px | `color: var(--color-text-3)` |

---

## Spacing

| Token | Value | Usage |
|-------|-------|-------|
| `--section-padding-desktop` | `72px 48px` | All full-width sections |
| `--section-padding-mobile` | `56px 20px` | All full-width sections on mobile |
| `--section-header-gap` | `28px` | Between section header and content |
| `--card-gap` | `28px` | Grid gap between cards |
| `--content-max-width` | `1180–1400px` | Always paired with `margin: 0 auto` |

---

## Buttons

### Primary — Gold CTA

```css
background: #c98a1e;
color: #ffffff;
height: 54–58px;
border-radius: 12px;
font-weight: 700;
font-size: 17–20px;
padding: 0 28px;
transition: background 0.2s ease, transform 0.2s ease;

/* hover */
background: #b07618;
transform: translateY(-1px);

/* mobile: full width */
width: 100%;
min-height: 56px;
```

### Secondary — Green Outline

```css
background: transparent;
border: 1.5px solid #0e5b37;
color: #0e5b37;
height: 48–54px;
border-radius: 10–12px;
font-weight: 600;
```

### Dark Action — Solid Green

```css
background: #0e5b37;
color: #ffffff;
height: 48–54px;
border-radius: 12px;
font-weight: 600;
```

### Footer CTA — Gold Outline

```css
background: transparent;
border: 1.5px solid #c98a1e;
color: #c98a1e;
border-radius: 12px;
font-weight: 600;
```

---

## Cards

### Standard Card (benefit, step, review, help)

```css
background: #ffffff;
border-radius: 20px;
box-shadow: 0 12px 32px rgba(18, 61, 42, 0.08);
width: 100%;
```

### Bordered Card (comparison, sidebar modules)

```css
background: #ffffff;
border: 1px solid #d8e2d4;
border-radius: 18px;
box-shadow: 0 8px 24px rgba(44, 59, 42, 0.04);
```

### Icon Circle (benefit / process cards)

```css
width: 56–64px;
height: 56–64px;
border-radius: 50%;
background: #eaf3de;
border: 1px solid #c0dd97;
color: #27500a;
```

---

## Form Inputs

```css
height: 56–58px;
border: 1px solid #e7ece8;
border-radius: 12px;
padding: 0 18px;
font-size: 16px;
background: #ffffff;

/* focus */
border-color: #0e5b37;
outline: none;
```

Textarea:
```css
height: 160px;
padding: 16px 18px;
resize: vertical;
```

---

## Layout Patterns

### Desktop Hero — Two Column
```css
display: grid;
grid-template-columns: 1fr 1fr;
min-height: 520–620px;
```
Left: eyebrow + H1 + copy + CTA. Right: lifestyle photo.

### Three-Column Card Grid
```css
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 28px;
```
Collapses to 2 columns at `< 1100px`, single column at `< 768px`.

### Main + Sidebar
```css
display: grid;
grid-template-columns: minmax(0, 1fr) 360px;
gap: 56–72px;
align-items: start;
```
Sidebar stacks below content at `< 1100px`.

---

## Header

```css
height: 84px;                      /* desktop */
height: 64–72px;                   /* mobile */
padding: 0 48px;                   /* desktop */
padding: 0 16–20px;                /* mobile */
background: #ffffff;
border-bottom: 1px solid #d8e2d4;
position: sticky;
top: 0;
z-index: 50;
```

Structure: logo left — nav center — gold CTA right (desktop). Logo + CTA + hamburger (mobile).

---

## Footer

```css
background: #0f3a25;               /* or gradient: linear-gradient(135deg, #041f17, #0a3527, #0e4a35) */
color: #ffffff;
padding: 64px 48px;                /* desktop */
padding: 32px 20px 40px;           /* mobile */
```

Structure: 4 columns — Brand + tagline, Company links, Resources links, Legal links — plus a gold outline "Get a Free Quote →" button. Stacks vertically on mobile.

---

## Responsive Breakpoints

| Breakpoint | Behavior |
|-----------|---------|
| `< 1100px` (tablet) | Multi-column grids → 1–2 columns; sidebar moves below content |
| `< 768px` (mobile) | Full single column; hero image becomes full-bleed background with dark green overlay; all buttons full-width; Final CTA and Footer share `#0f3a25` background and visually merge |

---

## Trust & Micro-copy Patterns

| Pattern | Text |
|---------|------|
| Security note | `🔒 Your information is safe and secure.` |
| Trust bullets | `✔ No obligation · ✔ Multiple carriers · ✔ Licensed experts · ✔ Nationwide coverage` |
| Primary CTA | `Get My Free Quote →` |
| Secondary CTA | `Compare My Options →` |
| Eyebrow style | ALL CAPS, tight letter-spacing, `var(--color-eyebrow)` |
