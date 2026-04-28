# FindInsureWise FAQ Page Layout Spec (V2)

**Page Type:** FAQ / SEO / Trust / Assisted Conversion  
**Primary Goal:** Answer common questions clearly  
**Secondary Goal:** Move qualified visitors toward quote or advisor help

**Style Direction:** Clean editorial layout, premium whitespace, calm confidence

---

# 1. Header

## Structure

Left:
- FindInsureWise logo

Center Navigation:
- Term Life Insurance
- Living Benefits
- About Us
- Resources ▼

Right CTA:
- Get a Free Quote →

## Specs

```css
height: 84px;
padding: 0 48px;
background: #FFFFFF;
border-bottom: 1px solid #EEF1EE;
position: sticky;
top: 0;
z-index: 50;
```

---

# 2. Hero Section

## Layout

Two-column split.

Left:
- FAQ messaging
- Search bar
- Topic pills

Right:
- Lifestyle hero image

```css
grid-template-columns: 1fr 1fr;
min-height: 560px;
```

---

## Left Content

### Eyebrow

FAQ

```css
font-size: 15px;
font-weight: 700;
letter-spacing: 0.06em;
text-transform: uppercase;
color: #1A7A42;
margin-bottom: 18px;
```

### H1

Frequently Asked Questions

```css
font-size: 68px;
line-height: 1.06;
font-family: serif;
font-weight: 600;
color: #0E2A1F;
max-width: 520px;
margin-bottom: 24px;
```

### Supporting Copy

Find answers to the most common questions about term life insurance and living benefits.

```css
font-size: 22px;
line-height: 1.75;
color: #58645C;
max-width: 560px;
margin-bottom: 34px;
```

---

## Search Bar

Placeholder:

Search questions...

```css
height: 58px;
border: 1px solid #E8ECE9;
border-radius: 999px;
padding: 0 22px;
font-size: 17px;
background: #FFFFFF;
max-width: 620px;
margin-bottom: 26px;
```

---

## Topic Pills

Examples:

- Term Life Basics
- Living Benefits
- Application
- Coverage & Cost
- Policy Management

```css
display: flex;
flex-wrap: wrap;
gap: 12px;
```

Pill style:

```css
height: 40px;
padding: 0 18px;
border-radius: 999px;
background: #F6F8F5;
border: 1px solid #E6ECE8;
font-size: 15px;
```

---

## Right Hero Image

Use approved couple discussion image.

```css
width: 100%;
height: 560px;
object-fit: cover;
object-position: center;
```

Image style:

- warm daylight
- planning conversation
- premium home interior
- trustworthy lifestyle scene

---

# 3. Main Content Section

## Layout

Two columns.

Left:
- FAQ content

Right:
- Smart sidebar modules

```css
grid-template-columns: minmax(0, 1fr) 360px;
gap: 56px;
max-width: 1400px;
margin: 0 auto;
padding: 76px 48px 96px;
align-items: start;
```

---

# 4. Left Column: FAQ Category Blocks

Use accordion groups.

## Block Structure

1. Icon + category title  
2. One-line intro  
3. Question accordion list

## Spacing

```css
margin-bottom: 64px;
```

---

## Example Category A

### Title

About Term Life Insurance

### Intro

Learn how term life insurance works, how long it lasts, and who it's best for.

### Questions

- What is term life insurance?
- How does term life insurance work?
- How long does term life insurance last?
- Can I renew my term life insurance policy?
- What happens if I outlive my term life policy?

---

## Example Category B

### Title

Living Benefits

### Intro

Understand how certain policies may provide access to benefits while you're alive.

### Questions

- What are living benefits?
- How do living benefits work?
- What illnesses may qualify?
- Will using benefits reduce my death benefit?
- Do all policies include living benefits?

---

## Example Category C

Application & Approval

## Example Category D

Coverage & Cost

## Example Category E

Policy Management

---

# 5. Accordion Style

## Closed Row

```css
height: 58px;
padding: 0 22px;
border: 1px solid #EBEFEC;
border-radius: 14px;
background: #FFFFFF;
display: flex;
align-items: center;
justify-content: space-between;
```

## Expanded Row

```css
padding: 22px;
line-height: 1.8;
background: #FAFCFA;
border-radius: 14px;
```

---

# 6. Right Sidebar

Sticky desktop sidebar.

```css
position: sticky;
top: 112px;
display: flex;
flex-direction: column;
gap: 28px;
```

---

# 7. Sidebar Module A

## Browse by Topic

List categories + question counts.

Examples:

- Term Life Basics (12)
- Living Benefits (10)
- Application & Approval (8)
- Coverage & Cost (9)
- Policy Management (6)

Card style:

```css
background: #FFFFFF;
border: 1px solid #EBEFEC;
border-radius: 18px;
padding: 28px;
```

---

# 8. Sidebar Module B

## Soft CTA Card

### Heading

Still can't find what you're looking for?

### Copy

Speak with a licensed advisor for personalized guidance—no pressure, just answers.

### Button

Get Help →

```css
background: #F7FAF6;
border-radius: 18px;
padding: 28px;
```

Button style:

```css
height: 48px;
border-radius: 12px;
background: #0E5B37;
color: #FFFFFF;
font-weight: 600;
width: 100%;
```

---

# 9. Sidebar Module C

## Popular Questions This Week

Examples:

- Is term life insurance worth it at 35?
- Can I use living benefits for cancer?
- How much coverage do I really need?
- What happens if I miss a payment?
- Can I convert my term policy later?

Link:

View more popular questions →

---

# 10. Sidebar Module D

## Newsletter

### Heading

Stay informed

### Copy

Tips, guides, and resources straight to your inbox.

### Fields

- Email input
- Subscribe button

---

# 11. Bottom Newsletter Band

Full width trust strip.

Left:
- icon
- headline
- subtext

Right:
- email field
- subscribe button

```css
max-width: 1400px;
margin: 0 auto 88px;
padding: 26px 34px;
background: #F5F8F2;
border-radius: 18px;
display: grid;
grid-template-columns: 1fr 420px;
gap: 24px;
```

Headline:

Get expert tips & guides in your inbox

Subtext:

Join thousands of families making smarter insurance decisions.

---

# 12. Footer

Dark green gradient.

```css
padding: 64px 48px;
background: linear-gradient(135deg,#04281D,#0B5635,#03231A);
color: #FFFFFF;
```

Columns:

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

Get a Free Quote →

Gold outline button.

---

# 13. Responsive Rules

## Tablet (< 1100px)

- Hero stacks vertically
- Sidebar moves below FAQ content
- Grid becomes single column

## Mobile (< 768px)

- H1 = 42px
- Hero image = 320px
- Pills horizontal scroll
- Accordions full width
- Sidebar modules stack below
- Buttons full width

---

# 14. UX Strategy

This page should support 3 user types:

### Researcher

Uses search + accordions.

### Warm Lead

Clicks soft CTA for help.

### Returning Visitor

Uses topic navigation and popular questions.

---

# 15. Final Design Principle

Feels like a premium knowledge center,  
not a cluttered insurance support page.
```