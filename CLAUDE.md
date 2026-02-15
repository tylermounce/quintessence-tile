# Quintessence Tile PDX - Landing Page Project

## Client Overview

**Company:** Quintessence Tile PDX
**Website:** https://www.quintessencetilepdx.com/
**Location:** Portland, Oregon
**Contact:** quintessencetile@gmail.com

**What they do:** Custom tile work and luxury bathroom remodeling. They position themselves as "a dedicated team of local tile nerds specializing in custom tile and bathroom remodeling." They focus on artisan-level craftsmanship, premium materials, and collaborative design with homeowners.

**Services:**
- Custom tile design and installation
- Bathroom remodeling (full transformations)
- Custom shower design and installation
- Statement floors (herringbone, large-format, natural stone)
- Accent walls and backsplashes

**Target market:** High-end luxury homeowners in the Portland metro area (Lake Oswego, West Linn, West Hills, Pearl District, Tigard, Beaverton, and surrounding communities).

**Key differentiators:**
- Locally owned, passionate specialists (not generalists)
- Premium materials sourced from top suppliers
- Meticulous precision in every detail (grout lines, edges, cuts)
- Collaborative process from concept through completion
- Licensed, bonded, and insured in Oregon

---

## Landing Page Details

**File:** `quintessence-tile-landing-page.html` (single-file, self-contained HTML)

### Design Specs

- **Fonts:** Playfair Display (headings) + Raleway (body) via Google Fonts
- **Color palette:**
  - Primary BG: `#FAFAF8` (warm off-white)
  - Secondary BG: `#F0EEEB` (warm light gray)
  - Dark BG: `#0F1923` (near-black navy)
  - Navy accent: `#1B3A5C` (CTAs, highlights, labels)
  - Navy hover: `#14304D`
  - Text primary: `#2D2D2D`
  - Text secondary: `#7A7A7A`
  - Headings: `#1A1A1A`
  - Borders: `#E2E0DC`
- **Aesthetic:** Sleek, clean, minimalist. Neutral tones with navy blue accents. Luxury market positioning.
- **Responsive:** Breakpoints at 960px (tablet) and 600px (mobile)
- **Animations:** IntersectionObserver scroll-reveal, accordion FAQ toggle

### Page Architecture (top to bottom)

1. **Header** - Logo only, no nav, absolute positioned over hero
2. **Hero** - Full-bleed background image with dark navy gradient overlay. Eyebrow + H1 headline + subheadline + CTA. Trust indicators below (5-star rated, locally owned, licensed & insured).
3. **Trust Strip** - Dark section with 4 value props: Premium Materials Only, On-Time Completion, Collaborative Process, Artisan-Level Craft
4. **The Quintessence Difference** - 3 white cards with thin SVG icons: Artisan Precision, Premium Materials, Collaborative Design
5. **Image Divider** - Full-width marble bathroom photo with gradient overlay transitioning between sections
6. **Showcase (Our Work)** - 2x2 grid of project category cards with hover zoom: Luxury Bathroom Remodels, Custom Shower Design, Statement Floors, Accent Walls and Backsplashes
7. **How It Works** - 4 numbered steps with connecting lines: Consultation, Design and Selection, Expert Installation, The Reveal
8. **Mid-Page CTA** - Navy banner: "Ready to Elevate Your Space?" with secondary-style button
9. **Testimonials** - 3 cards on dark background with gold star ratings. ALL PLACEHOLDERS (wrapped in asterisks).
10. **FAQ** - 2-column layout: intro text + CTA on left, 5 accordion items on right. Questions: service area, timeline, material selection, estimate process, licensing.
11. **Final CTA + Form** - Dark section with placeholder form (First Name, Last Name, Email, Phone, Project Description, Submit). "We typically respond within one business day."
12. **Footer** - Centered logo on dark background, nothing else

### CTA Strategy

- **Primary CTA text:** "Request Your Free Estimate" (consistent across all buttons)
- **CTA placements:** Hero, FAQ sidebar, mid-page banner, final form section
- All CTAs anchor-link to `#estimate` (the final form section)

### Copy Highlights

- **Headline:** "Bespoke Tile and Bath Design for Homes That Demand More"
- **Subheadline:** "We bring precision, artistry, and genuine obsession for craft to every surface we touch. From natural stone to hand-set mosaics, your space deserves nothing less than extraordinary."
- **Section label style:** All-caps, letterspaced, navy blue, small font
- **Tone:** Confident, refined, direct. No fluff, no exclamation points, no em dashes.

---

## Before Going Live Checklist

### Images (all currently placeholders)
- [ ] **Hero background** - Replace with Quintessence's best wide-angle project photo (search for `hero__bg` img tag)
- [ ] **Image divider** - Replace with a dramatic full-width bathroom/tile photo (search for `image-divider` section)
- [ ] **Showcase card 1** "Luxury Bathroom Remodels" - Replace with their best bathroom remodel photo
- [ ] **Showcase card 2** "Custom Shower Design" - Replace with a custom shower project photo
- [ ] **Showcase card 3** "Statement Floors" - Replace with a floor tile project photo
- [ ] **Showcase card 4** "Accent Walls and Backsplashes" - Replace with a backsplash or accent wall photo

All placeholder images are marked with `<!-- PLACEHOLDER: ... -->` HTML comments for easy search.

### Testimonials (all currently placeholders)
- [ ] Replace all 3 testimonial quotes with real client reviews (currently wrapped in `*asterisks*`)
- [ ] Update author names and locations with real client info
- [ ] If only 1-2 real testimonials are available, remove the extras rather than leaving placeholders

### Form
- [ ] Replace the placeholder `<form>` in the Final CTA section with the actual form embed (HubSpot, Zoho, etc.)
- [ ] The form placeholder has fields for: First Name, Last Name, Email, Phone, Project Description
- [ ] Adjust the form container's `max-width` and styling if the embed has its own styles

### Optional Enhancements
- [ ] Add the actual Quintessence logo image to replace the text logo (header and footer)
- [ ] Add real project count or years in business to the trust strip
- [ ] Add Google Reviews badge or link if available
- [ ] Connect CTA buttons to a booking tool (Calendly, etc.) instead of the form if preferred

---

## Technical Notes

- Single HTML file with embedded CSS (`<style>`) and JavaScript (`<script>`)
- No external dependencies except Google Fonts
- All colors defined as CSS custom properties in `:root` for easy theme adjustments
- Icons are inline SVGs (thin, single-line style)
- FAQ accordion is vanilla JS with aria-expanded attributes
- Scroll animations use IntersectionObserver (no library)
- Built following the Amplis LP Builder skill design system
