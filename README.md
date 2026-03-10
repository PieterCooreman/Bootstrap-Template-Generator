# Bootstrap Design Generator

A single-file Bootstrap 5 website template generator that produces complete, randomized SaaS landing pages with **36 million+ unique visual combinations**. Every click generates a fully functional, responsive, dark-mode-ready website you can download as a standalone HTML file. 

Download or use on https://pietercooreman.github.io/Bootstrap-Template-Generator/

Next step: Upload any generated template to any AI and ask to replace/add/remove texts and images. 

---

## Quick Start

1. Open `index.html` in any modern browser
2. Click the generate button (or wait -- it auto-generates on load)
3. Click the download button to save the template as a standalone `.html` file

No build tools, no dependencies, no server required.

---

## Feature Overview

### Design System

| Category | Count | Details |
|----------|-------|---------|
| Color Palettes | 10 | 8 light + 2 dark themes, each with 8 tokens (primary, secondary, accent, background, dark, text, light, dark flag) |
| Font Pairings | 10 | All Google Fonts -- 3 serif/sans combos, 7 sans/sans combos. Includes variable/optical-sizing fonts (Fraunces, Bricolage Grotesque) |
| Brand Identities | 16 | Complete SaaS personas across 8 industries, each with name, tagline, description, 3 feature names, CTAs |
| Hero Layouts | 5 | Full-background glass, split, centered, magazine, gradient banner |
| Nav Styles | 5 | Dark, colored, glass-dark, glass-light, minimal-light |
| Button Variants | 5 | Rounded-pill, square, rounded, outline-first, mixed |
| Card Styles | 5 | Shadow-hover, glass-card, flat-border, gradient-tint, image-top |
| Grid Layouts | 4 | Equal 3-col, equal 2-col, asymmetric, narrow-narrow-wide |
| Feature Layouts | 3 | Three-column icons, alternating image-text rows, four-column compact grid |
| Testimonial Layouts | 3 | Three-column cards, featured + sidebar, single large centered quote |

### Sections (13 total)

Every generated template includes a selection of these sections, assembled in a weighted random order:

| Section | Always Included | Inclusion Rate | Description |
|---------|:-:|:-:|---|
| Announcement Bar | | 50% | Gradient banner with icon, text, link to detail modal, dismiss button |
| Navigation | x | | Sticky responsive navbar with dropdown, scrollspy, conditional pricing link |
| Hero | x | | One of 5 layout variants with stats, badges, floating cards |
| Logo Bar | | 75% | Scrolling marquee of company names with edge-fade masks |
| Features | x | | One of 3 layout variants with icon boxes and descriptions |
| Stats Strip | | 70% | Full-width gradient band with large stat numbers and decorative blur blobs |
| Solutions (Cards) | x | | Image cards with badges in one of 5 styles across 4 grid layouts |
| Testimonials | | 80% | One of 3 layout variants with avatars and star ratings |
| Pricing | | 60% | Three-tier pricing cards with feature lists, tooltips, and gradient-border popular tier |
| CTA Banner | | 65% | Full-width gradient section with decorative blobs and dual CTAs |
| FAQ | | 55% | Bootstrap accordion with themed styling |
| Contact Form | x | | Split layout with feature list + full form panel (6 fields) |
| Footer | x | | 4-column footer with social links, newsletter signup, legal links to modals |

### Bootstrap 5 Components Used

The generated templates use 13 distinct Bootstrap component types:

- **Navbar** -- Responsive with collapse toggler, 5 visual styles
- **Dropdown** -- "More" nav item with icon-labeled items and divider
- **Modal** -- Privacy Policy (7 sections), Terms of Service (7 sections), Announcement detail
- **Accordion** -- FAQ section with themed dark-mode support
- **Tooltip** -- Pricing feature explanations, footer social icon labels
- **ScrollSpy** -- Auto-highlights active nav link while scrolling
- **Collapse** -- Navbar mobile menu, accordion panels
- **Badge** -- Card image overlays, pricing "Most Popular" pill
- **Cards** -- 5 style variants including glassmorphism and gradient tint
- **Forms** -- Text, email, select, textarea, checkbox, input-group (newsletter)
- **Buttons** -- 5 shape variants, primary/secondary/outline/light, glow shadows
- **Grid** -- Full responsive grid with gutters, offsets, order classes
- **Utilities** -- Flex, spacing, text, position, shadow, border, display, sizing

### Interactive Features (15)

| Feature | Description |
|---------|-------------|
| Dark / Light Mode Toggle | Fixed button toggles `data-theme` on the generated page; all colors transition smoothly via CSS custom properties |
| Image Lightbox | Click any image to open a full-screen overlay with zoom-out close |
| Scroll-to-Top | Floating button fades in after scrolling 380px |
| Scroll Progress Bar | Thin gradient bar at top tracks scroll position |
| Cookie Consent Toast | Bottom-center glassmorphism toast with Accept/Decline and link to Privacy Policy modal |
| Announcement Bar | Dismissible gradient banner above navbar, links to detail modal |
| Privacy Policy Modal | Scrollable modal with 7 sections of legal text, dynamic brand name and dates |
| Terms of Service Modal | Scrollable modal with 7 sections, dynamic brand references |
| Pricing Tooltips | Hover technical features (SSO, SLA, API access, etc.) for plain-English explanations |
| Social Icon Tooltips | Hover footer social icons for platform names |
| ScrollSpy | Active nav link auto-highlights as user scrolls through sections |
| Card Hover Lift | Cards translate upward with enhanced shadow on hover |
| Feature Icon Hover | Icon background fills to primary color on hover |
| Image Hover Zoom | Card and hero images scale subtly on hover |
| AOS Scroll Animations | Fade-up, fade-left, fade-right, zoom-in with custom cubic-bezier easing |

### CSS Techniques (17)

| Technique | Details |
|-----------|---------|
| Gradient Text | `background-clip: text` with primary-to-secondary gradient on hero headings |
| Animated Section Bars | Tri-color gradient bar with infinite shimmer animation on every section heading |
| Glassmorphism | `backdrop-filter: blur()` + semi-transparent backgrounds on navbar, cards, floating stat cards, cookie toast, form panel |
| Noise Texture Overlay | SVG `feTurbulence` fractal noise as `body::after` at 1.8% opacity |
| Marquee Logo Scroll | CSS `@keyframes` translateX animation with duplicated elements and edge gradient masks |
| CSS Custom Properties | 20+ design tokens (colors, backgrounds, text, borders, inputs) with light/dark mode switching |
| Gradient Backgrounds | Hero, stats strip, CTA banner, announcement bar, pricing popular card border |
| Decorative Blur Blobs | Absolute-positioned large circles with `filter: blur(65-80px)` for ambient color |
| Selection Styling | `::selection` uses palette primary color |
| Gradient Border | Popular pricing card uses `background-clip: padding-box, border-box` trick |
| Parallax | Full-bg-glass hero uses `background-attachment: fixed` |
| Fluid Typography | `clamp()` on hero headings for responsive scaling without breakpoints |
| Spring Easing | Buttons use `cubic-bezier(.34, 1.56, .64, 1)` for springy overshoot |
| Smooth Scrolling | `scroll-behavior: smooth` on `<html>` |
| Scroll Margin | `scroll-margin-top: 80px` prevents anchors from hiding behind sticky nav |
| Button Glow | Primary buttons have palette-colored `box-shadow` that intensifies on hover |
| Transition Orchestration | All theme-sensitive properties transition on dark/light mode switch (background, color, border-color) |

### Responsive Design

- **Navbar collapse** at `<lg` breakpoint with Bootstrap hamburger toggler
- **Fluid typography** via `clamp()` on all hero headings (5 different clamp values)
- **Responsive grid** with `col-6` / `col-md-*` / `col-lg-*` for mobile-first layouts
- **Glass float cards** hidden on mobile (`display: none` at `<768px`)
- **Reduced heading sizes** at `<768px` (`h1: 2rem`, `h2: 1.6rem`)
- **Flex wrap** on button groups and CTA sections for mobile stacking
- **Cookie toast** width adapts: `max-width: 540px; width: calc(100% - 2rem)`
- **Viewport meta tag** on all generated pages

### Accessibility

- `prefers-reduced-motion` media query disables all animations and transitions
- `aria-label` on all close buttons
- `aria-labelledby` connecting modal titles to their headers
- `aria-hidden="true"` on modals
- `tabindex="0"` on `<body>` (required for ScrollSpy)
- `lang="en"` on `<html>`
- `alt` attributes on all images (hero, cards, avatars)
- `title` attribute on dark mode toggle
- Semantic HTML throughout (`<nav>`, `<section>`, `<footer>`, `<label>`)
- `<iframe title="Preview">` on generator preview

### Legal / Compliance

- **Privacy Policy** -- 7-section modal: Information Collection, Usage, Cookies & Tracking, Data Sharing, Data Security, Your Rights (GDPR, SOC 2, ISO 27001 references), Contact (dynamic email)
- **Terms of Service** -- 7-section modal: Acceptance, Registration, Acceptable Use, Intellectual Property, Payment & Billing, Limitation of Liability, Governing Law (Delaware)
- **Cookie Consent** -- Bottom toast with Accept/Decline + link to Privacy Policy
- **Dynamic dates** -- Policy dates and copyright year use `new Date()`
- **Dynamic brand references** -- All legal text references the generated brand name

---

## Content Data

### Images

| Type | Per Industry | Industries | Total |
|------|:-:|:-:|:-:|
| Hero images | 4 | 8 | 32 |
| Card images | 6 | 8 | 48 |
| Avatar portraits | -- | -- | 12 |
| **Total** | | | **92** |

All images sourced from Unsplash with verified working URLs.

### Text Content

| Content Type | Sets/Variants | Items per Set | Total Items |
|---|:-:|:-:|:-:|
| Testimonials | -- | -- | 12 |
| Feature descriptions | 6 | 3 | 18 |
| Card body texts | 5 | 3 | 15 |
| Card badges | -- | -- | 8 |
| Hero stat sets | 6 | 3 | 18 |
| Floating stats | -- | -- | 8 |
| Feature section headings | -- | -- | 6 |
| Card section headings | -- | -- | 6 |
| Testimonial section headings | -- | -- | 6 |
| Section subtitles | -- | -- | 8 |
| Solutions subtitles | -- | -- | 6 |
| Logo brand sets | 3 | 6 | 18 |
| Logo headers | -- | -- | 4 |
| Pricing tier sets | 2 | 3 | 6 |
| Pricing features | -- | -- | 35 |
| Pricing headings | -- | -- | 4 |
| Pricing subtitles | -- | -- | 4 |
| FAQ sets | 2 | 5 | 10 |
| FAQ headings | -- | -- | 4 |
| CTA headings | -- | -- | 6 |
| CTA subtitles | -- | -- | 4 |
| Announcements | -- | -- | 6 |
| Pricing tooltip definitions | -- | -- | 6 |
| Bootstrap icons (feature) | -- | -- | 9 |

---

## Combination Math

The generator randomly selects from independent pools for each design dimension:

```
10 palettes x 10 fonts x 16 brands x 5 heroes x 5 nav styles
x 5 button variants x 5 card styles x 4 grids x 3 feature layouts
x 3 testimonial layouts = 36,000,000 base combinations
```

With conditional sections (7 independent toggles), data pool selections, and section ordering randomization, the effective number of distinct templates is orders of magnitude higher.

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Bootstrap 5.3.3 (CSS + JS Bundle with Popper) |
| Icons | Bootstrap Icons 1.11.3 |
| Fonts | Google Fonts (10 families, dynamically loaded) |
| Animations | AOS 2.3.4 (Animate On Scroll) |
| Generator | Vanilla JavaScript (single file, no build step) |
| Output | Self-contained HTML files (no external dependencies beyond CDN links) |

---

## Generator UI

The generator itself has a minimal dark-themed sidebar interface:

- **Generate button** -- Produces a new randomized template (auto-runs on page load)
- **Download button** -- Saves the current template as `bootstrap-template.html`
- **Mode toggle** -- Three-state cycle: Auto / Force Dark / Force Light
- **Generation counter** -- Tracks templates generated in the current session
- **Browser chrome** -- Preview frame with URL bar showing palette, layout, and mode info

---

## Browser Support

Generated templates work in all modern browsers that support:

- CSS Custom Properties
- `backdrop-filter` (glassmorphism)
- CSS `clamp()`
- `scroll-behavior: smooth`
- Bootstrap 5.3.3 requirements

Graceful degradation for `prefers-reduced-motion` and browsers without `backdrop-filter` support.

---

## License

MIT
