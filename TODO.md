# TODO: Portfolio Site Rebuild (Modern Professional)

**Branch:** `rebuild-tailwind-v4`
**Status:** Ready to rebuild from scratch following updated design brief
**Design Version:** 2.1 - Modern professional portfolio with substantive content

---

## Build Plan

### Phase 1: Setup & Foundation
- [ ] Create HTML boilerplate for index.html
  - [ ] Add Tailwind CSS Browser v4 CDN script
  - [ ] Add Display Serif Google Font (choose one: Playfair Display, Libre Baskerville, or Lora)
  - [ ] Define @theme colors (off-white bg, secondary bg, text colors, accent, accent-light)
  - [ ] Include Font Awesome CDN for icons
  - [ ] Set up CSS for serif headings/name and sans-serif body
  - [ ] Apply serif font to "Tom Counsell" name wherever it appears (H1, nav, footer)
  - [ ] Set up semantic HTML structure (header, main with sections, footer)

### Phase 2: Header Navigation
- [ ] Build sticky header/nav bar
  - [ ] Site name/logo: "Tom Counsell" (left side, serif font)
  - [ ] Navigation links (right side): About, Experience, Contact (anchor links)
  - [ ] Share button with clipboard functionality
  - [ ] Sticky positioning with light background and subtle border
  - [ ] Mobile: Responsive layout (consider stacking if needed)

### Phase 3: Hero Section
- [ ] Build hero section (make a strong first impression)
  - [ ] **Large circular portrait image (160px mobile, 240px tablet, 320px+ desktop)**
  - [ ] Portrait is primary visual anchor - as big as layout allows
  - [ ] Subtle shadow on portrait for polish
  - [ ] Center-aligned above name with generous breathing room
  - [ ] H1: "Tom Counsell" (large, bold, serif, 3rem+ desktop)
  - [ ] Subtitle: "CTO & Technical Leader" (serif, gray)
  - [ ] Social media icon row (5 icons with generous sizing)
    - [ ] LinkedIn, AngelList, GitHub, Stack Overflow, Telegram
    - [ ] Icons in accent color with hover states
  - [ ] Extra vertical padding to let portrait breathe

### Phase 4: About Section
- [ ] Build about section
  - [ ] Section heading H2: "About" (serif, large)
  - [ ] Three-paragraph biography from CONTENT.md lines 216-220
  - [ ] Max width 800px, left-aligned text
  - [ ] Centered container
  - [ ] Alternating background color for visual interest

### Phase 5: Professional Experience Section
- [ ] Build experience section with cards
  - [ ] Section heading H2: "Professional Experience" (serif, large)
  - [ ] Create experience cards for all roles from CONTENT.md:
    - [ ] Fuse (DeckFusion) - CTO (Jun 2024-present)
    - [ ] Bumble/Official - Head of Engineering (Oct 2022-Dec 2023)
    - [ ] Chainstarters - Strategic Advisor (May 2018-present)
    - [ ] Yudame - Owner (Mar 2019-present)
    - [ ] SIMPLENIGHT - Cache Architect (2021-2024)
    - [ ] Blockchain Hub Prague - Executive Director (Sep 2017-Oct 2019)
    - [ ] Intelligent Trading Foundation - CTO (Jan 2017-Aug 2020)
    - [ ] Agoda (Booking Group) - Senior Team Lead (Jan 2016-Sep 2016)
    - [ ] Anou - Cofounder, Technical Director (Dec 2012-Jul 2015)
  - [ ] Each card includes:
    - [ ] Company logo (42px height, from static/img/)
    - [ ] Role title (H3, serif, prominent)
    - [ ] Company name (H4, accent color, linked)
    - [ ] Date range (small text, gray)
    - [ ] 3-5 bullet points from CONTENT.md
    - [ ] Technology tags (rounded badges, colored backgrounds)
  - [ ] Card styling:
    - [ ] Light border or subtle shadow
    - [ ] Padding: 1.5-2rem
    - [ ] Single-column stacked layout
    - [ ] Alternating backgrounds or consistent white cards
    - [ ] Generous spacing between cards

### Phase 6: Contact Section
- [ ] Build contact section (CTA)
  - [ ] Section heading H2: "Get in Touch" (serif)
  - [ ] Intro text: "Interested in working with Tom? Let's get in touch."
  - [ ] Large CTA button linking to rates.html
  - [ ] Button text: "View Rates & Contact"
  - [ ] Button in accent color with white text
  - [ ] Center-aligned
  - [ ] Extra bottom padding

### Phase 7: Footer
- [ ] Build footer
  - [ ] Copyright: "© 2025 Tom Counsell"
  - [ ] GitHub source link
  - [ ] "Back to top" link
  - [ ] Small text, centered
  - [ ] Light border on top

### Phase 8: Rates.html (Secondary Page)
- [ ] Build rates.html with consistent styling
  - [ ] Reuse header/nav from index.html (update links to point to index.html#sections)
  - [ ] Hero section (large portrait, name, tagline, social links - unified with index.html)
  - [ ] Testimonials section
    - [ ] Section heading H2: "What People Say"
    - [ ] 5 quotes with attribution from CONTENT.md
    - [ ] Clean blockquote styling with accent left border
    - [ ] Generous spacing
  - [ ] Pricing section
    - [ ] Section heading H2: "2024 Rates"
    - [ ] Table with 3 rates:
      - [ ] Base Rate: $324/hr
      - [ ] FinTech: $486/hr
      - [ ] Consultancy: $648/hr
  - [ ] Services sections (grid layouts)
    - [ ] Core Services (4 items in 2-column grid)
    - [ ] Data & Analytics (2 items)
    - [ ] Specialized Technologies (3 items in 3-column grid)
    - [ ] Integrations & Content (3 items in 3-column grid)
    - [ ] Each with icon, title, description
  - [ ] Payment Terms section
  - [ ] Discounts section
  - [ ] Additional Assurances section
  - [ ] CTA section with email contact button
  - [ ] Reuse footer from index.html

### Phase 9: Polish & Testing
- [ ] Test anchor navigation on index.html
- [ ] Test share button clipboard functionality
- [ ] Verify all external links work (social, company links, rates page)
- [ ] Test mobile responsiveness at all breakpoints
  - [ ] < 640px (mobile - single column)
  - [ ] 640-768px (tablet)
  - [ ] 1024px+ (desktop - larger portrait, optimal spacing)
- [ ] Check accessibility
  - [ ] Semantic HTML (proper heading hierarchy H1→H2→H3→H4)
  - [ ] Alt text on all images (portrait, company logos)
  - [ ] Color contrast (WCAG AA)
  - [ ] Keyboard navigation
- [ ] Test on different browsers (Chrome, Safari, Firefox)
- [ ] Verify smooth scrolling behavior
- [ ] Check all spacing/padding is consistent
- [ ] Verify typography hierarchy (serif headings, sans-serif body)
- [ ] Check that colors are used throughout (not just black/white)

---

## Design System Reference (v2.1)

### Colors (Tailwind @theme)
```
--color-bg-primary: #FAFAFA       (Off-white background)
--color-bg-secondary: #F0F5F4     (Light teal for alternating sections)
--color-text-primary: #111111     (Dark charcoal text)
--color-text-secondary: #555555   (Gray for subtitles, dates)
--color-accent: #52796F           (Muted teal for CTAs, links, company names)
--color-accent-light: #6B9B8F     (Lighter teal for hover states)
```

### Typography
- **"Tom Counsell" Name:** Display serif (Playfair Display, Libre Baskerville, or Lora)
  - Balanced, readable, authoritative
  - Used in H1, navigation, footer - wherever the name appears
- **Headings (H2-H4):** Same display serif font
  - H1 (Name): 3rem (48px), bold, serif
  - H2 (Sections): 1.75-2.25rem (28-36px), semibold, serif
  - H3 (Roles): 1.25rem (20px), medium, serif
  - H4 (Companies): 1rem (16px), semibold, accent color
- **Body text:** System sans-serif stack
  - Body: 1rem (16px), line-height 1.6
  - Small (dates, tags): 0.875rem (14px)
- **Technology tags:** Sans-serif, small, rounded badges with colored backgrounds

### Layout Principles
- **Single-column layout** for experience cards
- **Max content width:** 800-1000px for readability
- **Centered containers** with generous margins
- **Card-based design:** Subtle borders, shadows, or alternating backgrounds
- **Visual hierarchy:** Large portrait → Name → Experience cards with logos
- **Whitespace:** Generous (4rem desktop, 2rem mobile between sections)
- **Color throughout:** Not just black/white - use accent colors meaningfully

### Key Features (v2.1)
- ✅ Display serif font for "Tom Counsell" name and headings (Playfair Display, Libre Baskerville, or Lora)
- ✅ Professional experience cards with company logos
- ✅ Technology tags with colored backgrounds
- ✅ Accent colors used throughout (teal: #52796F)
- ✅ Alternating section backgrounds for visual interest
- ✅ Large portrait photo (160px-320px+) as hero element
- ✅ Subtle shadows and borders for depth
- ✅ Information-rich content (8-10 experience cards)
- ✅ Clean, modern, professional - not sterile or corporate

---

## Files to Reference
- **DESIGN_BRIEF.md v2.1** - Complete modern professional design specifications
- **CONTENT.md** - All copy/content for the site (experience details, testimonials, services)
- **CLAUDE.md** - Project documentation

## Notes
- This is a static site with no backend
- Long-scrolling portfolio with anchor navigation
- Secondary rates.html page for detailed info
- Use Tailwind utility classes throughout
- Keep JavaScript minimal (share button only)
- Git commits should NOT include co-author information
- Focus: Modern, professional, content-rich
- Emphasis: Substantive content with elegant design

---

## Content Mapping

### Hero Section
- Portrait: `static/img/profile.jpg` (LARGE - 320px+ desktop)
- Name: "Tom Counsell"
- Title: "CTO & Technical Leader"
- Social links from CONTENT.md lines 25-29

### About Section
- Biography: CONTENT.md lines 216-220 (three paragraphs)

### Professional Experience Section
- Fuse: CONTENT.md lines 40-52
- Bumble/Official: CONTENT.md lines 56-72
- Chainstarters: CONTENT.md lines 76-90
- Yudame: CONTENT.md lines 94-103
- SIMPLENIGHT: CONTENT.md lines 107-118
- Blockchain Hub: CONTENT.md lines 121-142
- ITF: CONTENT.md lines 145-163
- Agoda: CONTENT.md lines 166-184
- Anou: CONTENT.md lines 187-209

### Contact Section
- CTA: Links to rates.html

### Rates Page
- Testimonials: CONTENT.md lines 244-257
- Pricing: CONTENT.md lines 265-268
- Services: CONTENT.md lines 277-310
- Terms: CONTENT.md lines 315-334

### Company Logos (42px height)
All located in `static/img/`:
- deckfusion.jpeg (Fuse)
- bumble.png, official.jpg (Bumble/Official)
- chainstarters.jpg
- yudame.png
- simplenight.jpg
- bhub.png (Blockchain Hub)
- ITF.png
- agoda.png, booking.png (Agoda/Booking)
- anou.png
