# FindInsureWise Blog Post Page Layout Spec (Spacious Version)

**Style Direction:** Clean, premium, editorial, trust-focused  
**Goal:** SEO traffic + Quote conversions  
**Primary CTA:** Get a Free Quote  
**Secondary CTA:** Subscribe / Free Guide

---

# 1. Header

## Structure

Left:
- FindInsureWise logo

Center:
- Term Life Insurance
- Living Benefits
- About Us
- Resources ▼

Right:
- Gold CTA Button

Text:
Get a Free Quote →

## Specs

- Height: 84px
- Background: #FFFFFF
- Bottom border: light gray
- Sticky on scroll
- Horizontal padding: 48px

---

# 2. Main Layout Container

## Max Width

1400px

## Grid

```css
grid-template-columns: minmax(0, 1fr) 360px;
gap: 72px;
align-items: start;
```

## Padding

```css
padding-top: 56px;
padding-left: 48px;
padding-right: 48px;
padding-bottom: 80px;
```

More breathing room than previous version.

---

# 3. Left Content Column

Recommended max readable width:

```css
max-width: 760px;
```

---

# 4. Article Header Section

## Back Link

← Back to all articles

Muted green small text

Margin bottom: 32px

---

## Category Label

LIVING BENEFITS

- Uppercase
- Small size
- Green color
- Letter spacing slight

Margin bottom: 18px

---

## H1 Title

Can Term Life Insurance Pay While You're Alive?

## Specs

```css
font-size: 64px;
line-height: 1.08;
font-family: serif;
font-weight: 600;
max-width: 720px;
```

Margin bottom: 28px

---

## Subtitle

Living benefits can help you access life insurance money when you need it most. Here's how it works and who qualifies.

## Specs

```css
font-size: 22px;
line-height: 1.7;
color: #5E665F;
max-width: 680px;
```

Margin bottom: 36px

---

## Author Meta Row

Left:
- Avatar
- Jeff Lin
- May 12, 2026
- 6 min read

Right:
- Social icons

Margin bottom: 48px

---

# 5. Hero Image

## Specs

```css
width: 100%;
height: 520px;
border-radius: 20px;
object-fit: cover;
```

Margin bottom: 44px

Style:
- Warm family photo
- Realistic
- Natural daylight

---

# 6. TL;DR Gold Callout Box

Keep this section.

## Purpose

Fast skim summary + high visual contrast.

## Style

```css
background: #FFF9F1;
border: 1px solid #E8C98B;
border-radius: 18px;
padding: 32px;
```

Margin bottom: 56px

## Layout

Top Row:
- Gold shield icon
- TL;DR label

Below:
3 bullet points

## Example Content

- Some term life policies offer living benefits that let you access part of your death benefit early.
- These benefits can help with serious illness, chronic conditions, or terminal illness.
- Not all policies include living benefits—check your policy details.

---

# 7. Body Content Typography

## Paragraph

```css
font-size: 20px;
line-height: 1.9;
color: #27312A;
margin-bottom: 26px;
```

## H2

```css
font-size: 46px;
line-height: 1.2;
font-family: serif;
margin-top: 72px;
margin-bottom: 28px;
```

## H3

```css
font-size: 30px;
margin-top: 48px;
margin-bottom: 18px;
```

---

# 8. Benefit Bullet List

Use spacious stacked list.

Each row:

- Green check icon
- Bold label
- Supporting sentence

Gap between rows:

```css
16px
```

---

# 9. Mid-Article CTA Card

Placed after major section.

## Layout

Left:
- Shield icon
- Supporting text

Right:
- Gold CTA button

## Style

```css
background: #F9FAF8;
border: 1px solid #E6ECE7;
border-radius: 18px;
padding: 28px 32px;
display: flex;
justify-content: space-between;
align-items: center;
```

## Text

See how much coverage can protect your family and your future.

Button:

Get My Free Quote →

---

# 10. Tags Section

Simple chips.

Examples:

- living benefits
- term life
- critical illness
- life insurance basics

Margin top: 56px

---

# 11. Right Sidebar

Width:

```css
360px
```

Sticky:

```css
position: sticky;
top: 120px;
```

Vertical gap between cards:

```css
28px
```

---

# 12. Sidebar Card Style

Use for all cards:

```css
background: #FFFFFF;
border: 1px solid #EEF1EE;
border-radius: 18px;
padding: 28px;
box-shadow: 0 4px 18px rgba(0,0,0,0.03);
```

---

# 13. Sidebar Modules

## A. On This Page

Heading:
On This Page

List:
- What Are Living Benefits?
- How Do They Work?
- Who Qualifies?
- Benefits vs Riders
- Should You Add It?
- The Bottom Line

---

## B. Related Articles

3 stacked article cards with thumbnails.

---

## C. Quote CTA Card

Image top

Headline:

Ready to protect what matters most?

Text:

Get your free, no-obligation quote in minutes.

Gold button:

Get My Free Quote →

---

## D. Email Capture

Icon top

Headline:

Get expert tips & guides in your inbox

Input field

Green button:

Subscribe

---

# 14. Footer

## Style

Dark green gradient background

```css
padding: 56px 48px;
margin-top: 96px;
```

## Columns

### Brand

FindInsureWise  
Simple. Honest. Protection for what matters most.

### Company
- About Us
- How It Works
- Contact Us

### Resources
- Blog
- Guides
- FAQ

### Legal
- Privacy Policy
- Terms of Use
- Licensing

### CTA

Gold button:

Get a Free Quote →

---

# 15. Responsive Rules

## Tablet (< 1100px)

- Sidebar moves below article
- Gap reduced to 48px

## Mobile (< 768px)

- Single column
- Header simplified
- H1 = 40px
- Body = 18px
- Hero image height = 300px
- Sticky bottom CTA button enabled

---

# 16. UX Notes

This spacious version improves:

- Better readability
- Premium feel
- Less clutter
- Higher trust perception
- Easier scanning
- Better conversion pacing

---

# Final Design Principle

Feels like a high-end financial publication,  
converts like a lead generation landing page.