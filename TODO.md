# TODO: Portfolio Site Rebuild (Minimalist Single-Page)

**Branch:** `rebuild-tailwind-v4`
**Status:** Ready to rebuild from scratch following updated minimalist design brief
**Design Version:** 2.0 - Light, clean, single-page portfolio

---

## Build Plan

### Phase 1: Setup & Foundation
- [ ] Create HTML boilerplate for index.html
  - [ ] Add Tailwind CSS Browser v4 CDN script
  - [ ] Define @theme colors (off-white background, dark text, single accent color)
  - [ ] Include Font Awesome CDN for icons
  - [ ] System sans-serif font stack (NO Playfair Display)
  - [ ] Set up semantic HTML structure (header, main with sections, footer)

### Phase 2: Header Navigation
- [ ] Build simple header/nav bar
  - [ ] Site name/logo: "Tom Counsell" (left side, simple text)
  - [ ] Navigation links (right side): About, Achievements, Contact (anchor links)
  - [ ] Share button with clipboard functionality
  - [ ] Mobile: Consider hamburger menu if needed
  - [ ] Minimal styling, light background

### Phase 3: Hero Section
- [ ] Build hero section (first screenful)
  - [ ] Circular portrait image (100px mobile, 120px desktop)
  - [ ] Center-aligned above name
  - [ ] H1: "Tom Counsell" (large, bold, 3rem desktop)
  - [ ] Subtitle: "CTO & Technical Leader" (smaller, gray)
  - [ ] Social media icon row (5 icons, ~24px each)
    - [ ] LinkedIn, AngelList, GitHub, Stack Overflow, Telegram
    - [ ] Simple icons in gray/accent color with hover state
  - [ ] Generous padding, clean and airy

### Phase 4: About Section
- [ ] Build about section
  - [ ] Section heading H2: "About"
  - [ ] Single paragraph biography (4-5 sentences from CONTENT.md)
  - [ ] Max width 600-800px, left-aligned text
  - [ ] Centered container
  - [ ] Ample vertical padding

### Phase 5: Key Achievements Section
- [ ] Build achievements section
  - [ ] Section heading H2: "Key Achievements"
  - [ ] 3 achievement items:
    - [ ] "Leading Dev Teams" with icon
    - [ ] "Building Software" with icon
    - [ ] "Millions Served" with icon
  - [ ] Responsive grid: 1 column mobile, 3 columns desktop
  - [ ] Each item: icon (32px) + short text label
  - [ ] Center-aligned within grid cells
  - [ ] Simple outline icons, consistent style

### Phase 6: Contact Section
- [ ] Build contact section (CTA)
  - [ ] Section heading H2: "Get in Touch"
  - [ ] Intro text: "Interested in working with Tom? Let's get in touch."
  - [ ] Large CTA button linking to rates.html
  - [ ] Button text: "View Rates & Contact"
  - [ ] Button in accent color with white text
  - [ ] Center-aligned
  - [ ] Extra bottom padding

### Phase 7: Footer
- [ ] Build minimal footer
  - [ ] Copyright: "© 2025 Tom Counsell"
  - [ ] Optional: GitHub source link
  - [ ] Optional: "Back to top" link
  - [ ] Small text, centered

### Phase 8: Rates.html (Secondary Page)
- [ ] Rebuild rates.html to match minimalist aesthetic
  - [ ] Reuse header/nav from index.html
  - [ ] Hero section (portrait, tagline, social links for consistency)
  - [ ] Testimonials section
    - [ ] 5 quotes with attribution from CONTENT.md
    - [ ] Clean blockquote styling, generous spacing
  - [ ] Pricing table
    - [ ] Base Rate: $324/hr
    - [ ] FinTech: $486/hr
    - [ ] Consultancy: $648/hr
    - [ ] Simple table or card layout
  - [ ] Services sections
    - [ ] Core Services (4 items)
    - [ ] Data & Analytics (2 items)
    - [ ] Specialized Technologies (3 items)
    - [ ] Integrations & Content (3 items)
    - [ ] Clean list or card format
  - [ ] Payment Terms, Discounts, Additional Assurances
  - [ ] Reuse footer from index.html

### Phase 9: Polish & Testing
- [ ] Test anchor navigation on index.html
- [ ] Test share button clipboard functionality
- [ ] Verify all external links work (social, rates page)
- [ ] Test mobile responsiveness at all breakpoints
  - [ ] < 640px (mobile)
  - [ ] 640-768px (tablet)
  - [ ] 1024px+ (desktop)
- [ ] Check accessibility
  - [ ] Semantic HTML (proper heading hierarchy)
  - [ ] Alt text on portrait image
  - [ ] Color contrast (WCAG AA)
  - [ ] Keyboard navigation
- [ ] Test on different browsers (Chrome, Safari, Firefox)
- [ ] Verify smooth scrolling behavior
- [ ] Check all spacing/padding is consistent
- [ ] Ensure single-column layout on mobile

---

## Design System Reference (v2.0)

### Colors (Tailwind @theme)
```
--color-bg-primary: #FAFAFA       (Off-white background)
--color-text-primary: #111111     (Dark charcoal text)
--color-text-secondary: #555555   (Gray for subtitles)
--color-accent: #52796F           (Muted teal for CTAs)
```

### Typography
- **All text:** System sans-serif stack (NOT Playfair Display)
- **H1 (Name):** 3rem (48px), bold/extra-bold
- **H2 (Sections):** 1.5-2rem (24-32px), semibold
- **H3 (Sub-points):** 1.125rem (18px), medium
- **Body:** 1rem (16px), line-height 1.6
- **NO monospace tech tags** (not applicable in minimalist design)

### Layout Principles
- **Single-column layout** throughout
- **Max content width:** 600-800px for text
- **Centered containers** with generous margins
- **No cards, no gradients, no textures**
- **Flat design:** No shadows, no borders (except very subtle if needed)
- **Whitespace:** Generous (4rem desktop, 2rem mobile between sections)

### Responsive Breakpoints
- Mobile: `< 640px` (single column, stacked)
- Tablet: `sm: 640px`, `md: 768px` (still mostly single column)
- Desktop: `lg: 1024px`, `xl: 1280px` (optimized spacing)
- Wide: `2xl: 1536px` (max content width)

### Key Differences from Previous Build
- ❌ NO dark navy backgrounds
- ❌ NO heavy card-based layouts with 10 experience cards
- ❌ NO Playfair Display serif font
- ❌ NO color progression gradients
- ❌ NO texture overlays
- ❌ NO 12 Rules for Business grid
- ✅ Light, airy off-white background
- ✅ Simple single-page scroll
- ✅ 3 achievement highlights (not detailed experience cards)
- ✅ Sans-serif throughout
- ✅ One accent color only
- ✅ Minimal, clean, focused on content

---

## Files to Reference
- **DESIGN_BRIEF.md v2.0** - Complete minimalist design specifications
- **CONTENT.md** - All copy/content for the site
- **CLAUDE.md** - Project documentation

## Notes
- This is a static site with no backend
- Single-page scrolling design with anchor navigation
- Secondary rates.html page for detailed info
- Use Tailwind utility classes throughout
- Keep JavaScript minimal (share button only)
- Git commits should NOT include co-author information
- Focus: Light, clean, minimalist aesthetic
- Emphasis: Content over decoration, readability, whitespace

---

## Content Mapping

### Hero Section
- Portrait: `static/img/profile.jpg`
- Name: "Tom Counsell"
- Title: "CTO & Technical Leader"
- Social links from CONTENT.md lines 25-29

### About Section
- Biography: CONTENT.md lines 216-220 (condensed to 4-5 sentences)

### Key Achievements Section
- Achievement 1: "Leading Dev Teams" (from CONTENT.md header tagline)
- Achievement 2: "Building Software" (from CONTENT.md header tagline)
- Achievement 3: "Millions Served" (from CONTENT.md header tagline)

### Contact Section
- CTA: Links to rates.html

### Rates Page
- Testimonials: CONTENT.md lines 244-257
- Pricing: CONTENT.md lines 265-268
- Services: CONTENT.md lines 277-310
- Terms: CONTENT.md lines 315-334
