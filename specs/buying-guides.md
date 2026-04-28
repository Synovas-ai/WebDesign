# FindInsureWise Buying Guides Page Layout Spec

**Page Type:** Buying Guides / Decision Hub  
**Goal:** Help users find the right term life insurance guidance based on their life situation  
**Primary CTA:** Get My Free Quote  
**Secondary CTA:** Use Coverage Calculator  

---

# 1. Header

## Layout

Left:
- FindInsureWise logo

Center navigation:
- Buying Guides
- Calculator
- Blog
- FAQ
- About Us

Right:
- Get My Free Quote →

## Style

```css
height: 84px;
padding: 0 48px;
background: #FFFFFF;
border-bottom: 1px solid #D8E2D4;
position: sticky;
top: 0;
z-index: 50;
```

Active nav:
```css
color: #2C3B2A;
border-bottom: 3px solid #27500A;
```

Primary button:
```css
background: #C9972A;
color: #FFFFFF;
border-radius: 12px;
```

---

# 2. Hero Section

## Purpose

Introduce Buying Guides as a decision helper, not a blog archive.

## Layout

Two-column hero:

Left:
- Eyebrow
- H1
- Supporting text
- Optional search input

Right:
- Warm family lifestyle image

```css
display: grid;
grid-template-columns: 1fr 1fr;
min-height: 520px;
background: #F6F8F5;
```

## Left Content

Eyebrow:
```text
BUYING GUIDES
```

H1:
```text
Find the Right Coverage for Your Life
```

Supporting copy:
```text
Smart, easy-to-follow guides built around real life decisions—not insurance jargon.
```

Search placeholder:
```text
What would you like help with?
```

## Hero Image Direction

- Black family of four
- Warm outdoor golden-hour light
- Hopeful, joyful, natural moment
- Right side image placement
- Soft beige fade into left content area

---

# 3. Situation Cards Section

## Section Heading

```text
What best describes you right now?
```

## Subheading

```text
Choose a situation to find the most relevant guides for you.
```

## Layout

```css
max-width: 1180px;
margin: 0 auto;
padding: 56px 48px 64px;
```

Grid:

```css
display: grid;
grid-template-columns: repeat(3, 1fr);
gap: 28px;
```

---

## Card Style

Each card includes:

- 5:3 image
- floating circular icon
- title
- short description
- arrow

```css
background: #FFFFFF;
border: 1px solid #D8E2D4;
border-radius: 18px;
overflow: hidden;
box-shadow: 0 8px 24px rgba(44,59,42,0.04);
```

Image:

```css
aspect-ratio: 5 / 3;
object-fit: cover;
width: 100%;
```

Floating icon:

```css
width: 64px;
height: 64px;
border-radius: 50%;
background: #EAF3DE;
color: #27500A;
border: 1px solid #C0DD97;
```

Content:

```css
padding: 28px 24px 24px;
```

---

## Six Cards

### 1. We just had a baby

Description:
```text
Protect income, future expenses, and peace of mind.
```

Image direction:
- Young parents with newborn
- Warm home setting
- Natural hands holding baby

---

### 2. We bought a home

Description:
```text
Coverage ideas for mortgage and family protection.
```

Image direction:
- Beautiful suburban family home
- No people required
- No sold sign / no for-sale sign

---

### 3. I rely on work benefits

Description:
```text
Is group term life insurance enough?
```

Image direction:
- Indian professional
- Modern workspace
- Calm planning moment

---

### 4. I want affordable coverage

Description:
```text
See what protection may cost at your age.
```

Image direction:
- Young woman outdoors or lifestyle setting
- Confident, optimistic, independent
- Not just phone/laptop scene

---

### 5. I want benefits while alive

Description:
```text
Learn why living benefits matter.
```

Image direction:
- Couple around age 40
- Reviewing papers together
- Warm patio / garden / kitchen table setting
- Mature but not elderly

---

### 6. I’m not sure where to start

Description:
```text
Start with our beginner buying guide.
```

Image direction:
- Thoughtful person outdoors
- Mountain lake / trail / quiet planning mood
- Optimistic, reflective

---

# 4. Comparison Section

## Purpose

Help users compare common coverage options before choosing.

This section should feel related to the homepage comparison table, but more decision-focused.

## Container

```css
max-width: 1180px;
margin: 0 auto 32px;
padding: 42px;
background: #F6F8F5;
border-radius: 22px;
border: 1px solid #D8E2D4;
display: grid;
grid-template-columns: 280px 1fr;
gap: 36px;
```

---

## Left Copy

Eyebrow:
```text
THE FINDSUREWISE DIFFERENCE
```

Headline:
```text
What smart buyers compare before choosing coverage.
```

Supporting copy:
```text
The lowest price isn’t always the best fit. Here’s how the options stack up.
```

---

## Table Columns

```text
With Living Benefits
Traditional Term
Group Term (Work Coverage)
```

---

## Table Rows

```text
Pays your family if you pass away
May provide access after critical illness
May help if chronic illness affects daily living
Helps during life, not only after death
Portable if you change jobs
Coverage amount you can choose
Easy, no-obligation online quote
```

---

## Table Visual Style

Highlighted first column:

```css
background: #0B3A2B;
color: #FFFFFF;
border-radius: 12px 12px 0 0;
```

Check icons:

```css
background: #27500A;
color: #FFFFFF;
border-radius: 50%;
```

Muted dash:

```css
color: #8A9B88;
```

Footer note:

```text
Many families use Group Term as a supplement—not their only coverage.
```

Use small gold shield icon.

---

# 5. Calculator CTA Strip

## Purpose

Catch users who are interested but unsure how much coverage they need.

## Layout

```css
max-width: 1180px;
margin: 0 auto 24px;
padding: 30px 36px;
background: #FFFFFF;
border: 1px solid #D8E2D4;
border-radius: 18px;
display: grid;
grid-template-columns: auto 1fr auto;
gap: 24px;
align-items: center;
```

## Content

Headline:
```text
Not sure how much coverage to consider?
```

Copy:
```text
Use our free calculator to get a personalized estimate in minutes.
```

Button:
```text
Use Coverage Calculator →
```

Button style:
```css
background: transparent;
border: 1.5px solid #27500A;
color: #27500A;
border-radius: 10px;
```

---

# 6. Final Quote CTA Band

## Purpose

End the decision journey with a strong but clean quote action.

## Layout

```css
max-width: 1180px;
margin: 0 auto 56px;
padding: 34px 40px;
background: linear-gradient(135deg, #041F17 0%, #0A3527 45%, #0E4A35 100%);
border-radius: 18px;
display: grid;
grid-template-columns: auto 1fr auto;
gap: 28px;
align-items: center;
```

## Content

Headline:
```text
Ready to explore your options?
```

Copy:
```text
Get a fast, no-obligation quote in minutes.
```

Button:
```text
Get My Free Quote →
```

Trust note:
```text
Secure. Private. No spam.
```

Button style:
```css
background: #C9972A;
color: #FFFFFF;
border-radius: 12px;
```

---

# 7. Footer

## Style

Must match homepage footer exactly.

```css
background: linear-gradient(
  135deg,
  #041F17 0%,
  #0A3527 38%,
  #0E4A35 68%,
  #06241B 100%
);
color: #FFFFFF;
padding: 64px 48px;
```

## Columns

### Brand

```text
FindInsureWise
Simple. Honest. Protection for what matters most.
```

Social icons:
- Facebook
- Instagram
- LinkedIn

### Company
- About Us
- How It Works
- Contact Us
- Careers

### Resources
- Buying Guides
- Calculator
- Blog
- FAQ

### Legal
- Privacy Policy
- Terms of Use
- Licensing
- Sitemap

### Footer CTA

```text
Get My Free Quote →
```

Gold outline button.

---

# 8. Responsive Rules

## Tablet

```css
hero: single column;
cards: repeat(2, 1fr);
comparison: single column;
```

## Mobile

```css
cards: 1 column;
hero image height: 320px;
h1: 42px;
CTA bands: stacked;
footer: stacked;
```

---

# 9. Design System Notes

Use FindInsureWise design system:

```css
--bg-page: #F6F8F5;
--bg-card: #FFFFFF;
--border: #D8E2D4;
--text-1: #2C3B2A;
--text-2: #5A6B58;
--text-3: #8A9B88;
--gold: #C9972A;
--gold-bg: #FEF6E7;
--sage-dark: #27500A;
```

Avoid:
- bright blue / purple / pink icons
- teal footer gradients
- overly saturated green
- too many competing CTA boxes
- blog carousel clutter

---

# Final UX Principle

The Buying Guides page should feel like a calm decision guide:

```text
Identify your situation → understand your options → calculate coverage → get a quote.
```