# FindInsureWise Contact Page Layout Spec

**Page Type:** Contact / Trust / Lead Capture  
**Primary Goal:** Encourage users to reach out confidently  
**Secondary Goal:** Quote requests + brand trust

**Style Direction:** Warm, modern, premium, human support focused

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

Two-column desktop split:

Left:
- Contact messaging

Right:
- Support hero image

```css
grid-template-columns: 1fr 1fr;
min-height: 620px;
```

---

## Left Content

### Eyebrow

CONTACT US

```css
font-size: 16px;
letter-spacing: 0.06em;
font-weight: 600;
color: #16723A;
text-transform: uppercase;
margin-bottom: 20px;
```

### H1

We're here to help.

```css
font-size: 72px;
line-height: 1.05;
font-family: serif;
font-weight: 600;
color: #0F2A1F;
max-width: 520px;
margin-bottom: 28px;
```

### Supporting Copy

Have questions about term life insurance or living benefits?  
Our team is ready to help you find the right coverage for your family.

```css
font-size: 22px;
line-height: 1.75;
color: #516056;
max-width: 560px;
margin-bottom: 44px;
```

### Trust Row

- Licensed Experts
- 100% Secure
- No Obligation

```css
display: flex;
gap: 36px;
font-size: 16px;
color: #2C3A31;
```

---

## Right Hero Image

Friendly licensed support advisor image.

```css
width: 100%;
height: 620px;
object-fit: cover;
object-position: center;
```

Image direction:
- warm lighting
- premium office environment
- smiling professional
- approachable not salesy

---

# 3. Section: Contact Form + Commitment Card

## Layout

Two columns

Left:
- Send us a message form

Right:
- Our Commitment trust panel

```css
grid-template-columns: minmax(0, 1fr) 420px;
gap: 48px;
padding: 88px 48px;
max-width: 1400px;
margin: 0 auto;
```

---

# 4. Left Column: Contact Form

## Heading

Send us a message

```css
font-size: 54px;
font-family: serif;
margin-bottom: 18px;
color: #0F2A1F;
```

## Intro Text

Fill out the form below and a member of our team will get back to you shortly.

```css
font-size: 19px;
line-height: 1.75;
color: #5A665F;
margin-bottom: 36px;
max-width: 620px;
```

## Form Grid

Row 1:
- First Name
- Last Name

Row 2:
- Email Address
- Phone Number

Row 3:
- Subject

Row 4:
- Message textarea

## Inputs

```css
height: 56px;
border: 1px solid #E7ECE8;
border-radius: 12px;
padding: 0 18px;
font-size: 16px;
background: #FFFFFF;
```

## Textarea

```css
height: 160px;
padding: 16px 18px;
resize: vertical;
```

## Submit Button

Send Message →

```css
height: 54px;
padding: 0 28px;
border-radius: 12px;
background: #0E5B37;
color: #FFFFFF;
font-weight: 600;
margin-top: 20px;
```

---

# 5. Right Column: Commitment Card

## Card Style

```css
background: #F8FAF7;
border: 1px solid #E8EEE9;
border-radius: 20px;
padding: 34px;
height: fit-content;
```

## Heading

Our Commitment

```css
font-size: 38px;
font-family: serif;
margin-bottom: 26px;
```

## Items

### Your Privacy Matters

We don't share your information with anyone. Ever.

### Expert Guidance

Our licensed advisors provide honest, unbiased advice.

### No Pressure

We're here to help, not to sell. You're in control.

## Item Layout

- icon left
- text right
- 28px gap between rows

---

# 6. Section: Direct Contact Cards

Placed below form section.

## Layout

Two cards side by side

```css
grid-template-columns: repeat(2, 1fr);
gap: 28px;
padding: 0 48px 72px;
max-width: 1400px;
margin: 0 auto;
```

---

## Card A: Email Us

Email us anytime and we'll get back to you as soon as possible.

info@findinsurewise.com

---

## Card B: Call Us

Give our team a call during business hours.

(888) 123-4567  
Mon–Fri 8am–8pm ET

---

## Card Style

```css
background: #FFFFFF;
border: 1px solid #E9EEEA;
border-radius: 18px;
padding: 32px;
min-height: 220px;
```

---

# 7. Newsletter Band

## Layout

Full width container.

Left:
- icon
- headline + subtext

Right:
- email field
- subscribe button

```css
max-width: 1400px;
margin: 0 auto 88px;
padding: 28px 36px;
background: #F5F8F2;
border-radius: 18px;
display: grid;
grid-template-columns: 1fr 420px;
gap: 28px;
```

## Headline

Get expert tips & guides in your inbox

## Subtext

Join thousands of families making smarter insurance decisions.

---

# 8. Footer

## Style

Dark green gradient footer.

```css
padding: 64px 48px;
background: linear-gradient(135deg,#052B1E,#0C5536,#03251A);
color: #FFFFFF;
```

---

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

Get a Free Quote →

Gold outlined button.

---

# 9. Responsive Rules

## Tablet (< 1100px)

- Hero stacks vertically
- Form + commitment become single column
- Contact cards stack

## Mobile (< 768px)

- Header simplified
- H1 = 46px
- Body copy = 18px
- Hero image height = 360px
- All sections single column
- Buttons full width

---

# 10. UX Priorities

This page should communicate:

1. Easy to reach us  
2. Safe to contact us  
3. Real people will help  
4. No pressure sales tactics  
5. Fast path to quote if preferred

---

# Final Design Principle

Feels like a premium financial brand with real human support,  
not a generic insurance lead form page.