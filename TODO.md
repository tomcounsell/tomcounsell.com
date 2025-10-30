# TODO: Portfolio Site Rebuild

**Branch:** `rebuild-tailwind-v4`
**Status:** Ready to build from scratch

---

## Build Plan

### Phase 1: Setup & Foundation
- [ ] Create HTML boilerplate for index.html
  - [ ] Add Tailwind CSS Browser v4 CDN script
  - [ ] Define @theme colors (all brand colors)
  - [ ] Include Font Awesome CDN for icons
  - [ ] Add Playfair Display font from Google Fonts
  - [ ] Set up semantic HTML structure (header, main, footer)

### Phase 2: Header Component (Both Pages)
- [ ] Build header navigation
  - [ ] Name: "Tom Counsell" (Playfair Display, large)
  - [ ] Tagline (3 lines): Leading Dev Teams / Building Software / Millions Served
  - [ ] Navigation links: About (index.html), Rates (rates.html)
  - [ ] Share button with clipboard functionality
- [ ] Build social media icon row
  - [ ] LinkedIn, AngelList, GitHub, Stack Overflow, Telegram
  - [ ] Use Font Awesome icons
  - [ ] Horizontal layout on desktop, responsive on mobile

### Phase 3: Index.html - Experience Cards
- [ ] Create 2-column responsive grid (grid md:grid-cols-2)
- [ ] Build experience card component with:
  - [ ] Year-based color progression (2024 = navy-medium → older = muted-grey)
  - [ ] Company logo (42px height) + name
  - [ ] Role and period
  - [ ] Description bullets
  - [ ] Tech tag pills (rounded, monospace font)
  - [ ] Texture overlay (diagonal lines, 5% opacity)
- [ ] Implement cards for all 10 companies from CONTENT.md:
  - [ ] Fuse (2024-present)
  - [ ] Bumble/Official (2022-2023)
  - [ ] Chainstarters (2018-present)
  - [ ] Yudame (2019-present)
  - [ ] SIMPLENIGHT (2021-2024)
  - [ ] Blockchain Hub Prague (2017-2019)
  - [ ] Intelligent Trading Foundation (2017-2020)
  - [ ] Agoda (2016)
  - [ ] Anou (2012-2015)
  - [ ] Add Peace Corps volunteer experience if space permits

### Phase 4: Index.html - About Section
- [ ] Add profile image (static/img/profile.jpg, 150px circular)
- [ ] Bio paragraphs (3 paragraphs from CONTENT.md)
- [ ] 12 Rules for Business
  - [ ] Consider grid layout (3x4 or 4x3)
  - [ ] Each rule with keyword in parentheses
  - [ ] Geometric/clean presentation

### Phase 5: Rates.html
- [ ] Reuse header component from index.html
- [ ] Build testimonials section
  - [ ] 5 quotes with attribution from CONTENT.md
  - [ ] Clean blockquote styling
  - [ ] Spaced layout
- [ ] Pricing table
  - [ ] Base Rate: $324/hr
  - [ ] FinTech: $486/hr
  - [ ] Consultancy: $648/hr
- [ ] Services sections
  - [ ] Core Services (4 items)
  - [ ] Data & Analytics (2 items)
  - [ ] Specialized Technologies (3 items)
  - [ ] Integrations & Content (3 items)
- [ ] Payment Terms
- [ ] Discounts
- [ ] Additional Assurances

### Phase 6: Footer (Both Pages)
- [ ] GitHub source link
- [ ] "Back to top" link
- [ ] Simple, minimal design

### Phase 7: Polish & Testing
- [ ] Add hover states to cards
- [ ] Test share button clipboard functionality
- [ ] Verify all external links work
- [ ] Test mobile responsiveness at all breakpoints
- [ ] Check accessibility (semantic HTML, alt text)
- [ ] Test on different browsers
- [ ] Optimize images if needed

---

## Design System Reference

### Colors (Tailwind @theme)
```
--color-navy-medium: #4A6FA5       (2024 - newest)
--color-navy-blue: #3D5A7A         (2023)
--color-navy-blue-grey: #354A5F    (2022)
--color-dark-slate: #2D3B4A        (2021)
--color-muted-grey: #3A3E42        (older)
--color-sage-green: #8B9B88
--color-warm-sand: #E5DCC5
--color-cream: #F5F2E8
```

### Typography
- **Headings:** Playfair Display (serif)
- **Body:** System sans-serif stack
- **Tech Tags:** Monospace

### Responsive Breakpoints
- Mobile: `< 640px`
- Tablet: `sm: 640px`, `md: 768px`
- Desktop: `lg: 1024px`, `xl: 1280px`
- Wide: `2xl: 1536px`

### Card Color Progression
- 2024: `bg-gradient-to-br from-navy-medium to-navy-blue`
- 2023: `bg-gradient-to-br from-navy-blue to-navy-blue-grey`
- 2022: `bg-gradient-to-br from-navy-blue-grey to-dark-slate`
- 2021+: `bg-gradient-to-br from-dark-slate to-muted-grey`

---

## Files to Reference
- **CONTENT.md** - All copy/content for the site
- **DESIGN_BRIEF.md** - Complete design specifications
- **CLAUDE.md** - Project documentation

## Notes
- This is a static site with no backend
- All content is in CONTENT.md
- Use Tailwind utility classes throughout
- Keep JavaScript minimal (share button only)
- Company logos are all 42px height
- Git commits should NOT include co-author information
