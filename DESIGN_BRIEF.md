# Design Brief: Tom Counsell Portfolio Rebrand
## tomcounsell.com

**Date:** October 30, 2025
**Version:** 1.0
**Project Type:** Portfolio Website Rebrand

---

## Brand Positioning

**Tagline (from Cosmos):** *"Stoic strategy future navy CTO app aesthetic"*

Tom Counsell is a strategic technology leader who combines:
- **Stoic Philosophy** - Calm, measured decision-making
- **Strategic Vision** - Seeing patterns others miss ("You call them dreams. I call them maps with many pathways")
- **Technical Excellence** - CTO-level expertise with modern tech, human-centered design, AI-powered
- **Design Thinking** - "With strategy, design transforms aesthetics into powerful ideas"
- **Growth Mindset** - Embracing change, learning, being ambitious, always seeing the next mountain beyond this mountain.
---

## Design Principles

### 1. Clean Layout for Lists (Network Graph Inspiration)
**Reference:** Network diagram patterns showing different organizational structures

**Application:**
- Professional experience cards should show **connections** between roles
- Chronological progression with visual flow (radial convergence, organic connections)
- Each role as a "node" in a larger career network
- Technologies/skills as interconnected dots showing relationships

### 2. Color Progression (Bauhaus Navy Circles)
**Reference:** Concentric circles showing depth through color variation

**Application:**
- Most recent experiences: **Medium navy** (#4A6FA5, #3D5A7A)
- Recent past (2-3 years): **Navy blue-grey** (#354A5F)
- Earlier experiences: **Dark slate** (#2D3B4A, #323B45)
- Archived/legacy work: **Muted dark grey** (#3A3E42, #45494E)
- Creates visual **recency hierarchy** without explicit dates dominating
- Older items recede into darker, desaturated tones

### 3. Organic Texture (Mountain Impression)
**Reference:** Textured embossed surface on STRATEGY book cover

**Application:**
- Subtle background texture on cards (diagonal lines, paper grain)
- Creates **tactile, premium feel** without being busy
- Conveys depth and craftsmanship
- Use as CSS background pattern or SVG overlay at low opacity (5-10%)

---

## Color Palette

### Primary Colors
```
Navy Medium:      #4A6FA5  (Most recent work, primary cards)
Navy Blue:        #3D5A7A  (Recent experiences, headers)
Navy Blue-Grey:   #354A5F  (Mid-period experiences)
Dark Slate:       #2D3B4A  (Earlier work)
Muted Dark Grey:  #3A3E42  (Oldest/archived content)
```

### Secondary/Accent Colors
```
Sage Green:    #8B9B88  (Strategic thinking, growth themes)
Warm Sand:     #E5DCC5  (Background, warmth)
Cream:         #F5F2E8  (Card backgrounds, light sections)
Cool Gray:     #D8DFE3  (Borders, subtle dividers)
```

### Utility Colors
```
Black:         #0A0A0A  (Typography, contrast)
White:         #FEFEFE  (Clean spaces, text on dark)
Error/Alert:   #C84B4B  (Sparingly used)
Success:       #5A8F7B  (CTAs, links)
```

---

## Typography

### Existing Fonts (Retain & Enhance)
- **Playfair Display** - Headings, large display text
  - Serif provides classic, established feel
  - Pairs well with modern sans-serif body

### Recommended Additions
- **System Sans-Serif Stack** for body copy:
  ```css
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI",
               Roboto, "Helvetica Neue", Arial, sans-serif;
  ```
- **Monospace** for technical tags/skills:
  ```css
  font-family: "SF Mono", Monaco, "Cascadia Code", monospace;
  ```

### Typography Scale
```
H1 (Name):          48px / 3rem   (Playfair Display)
H2 (Section):       36px / 2.25rem (Playfair Display)
H3 (Role Title):    24px / 1.5rem  (Playfair Display)
Body Large:         18px / 1.125rem
Body Regular:       16px / 1rem
Body Small:         14px / 0.875rem
Technical Tags:     12px / 0.75rem (Monospace)
```

---

## Visual Elements

### 1. Geometric Patterns
**Inspired by:** Network diagrams, Bauhaus circles

**Elements to Create:**
- **Concentric circle motifs** as section backgrounds/accents
- **Connection lines** between experience cards (Bezier curves)
- **Node/dot patterns** to represent skills/technologies
- **Radial patterns** for visual interest in empty spaces

### 2. Background Textures
**Inspired by:** STRATEGY book embossed texture

**Implementation:**
```css
.card-texture {
  background-image: url('data:image/svg+xml,...'); /* Diagonal lines */
  background-size: 4px 4px;
  opacity: 0.05;
}
```

Options:
- Diagonal line pattern (45deg)
- Paper grain texture
- Subtle noise overlay
- Embossed effect using box-shadow

### 3. Photography Style
- **Deep blue tones** (ocean, contemplative)
- **High contrast** black & white with navy overlay
- **Geometric composition** (rule of thirds, clean lines)
- **Minimal, not busy** - lots of negative space

---

## Layout Structure

### Technical Implementation
**Framework:** Tailwind CSS via CDN (Browser version 4.x)
```html
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
```

**Custom Theme Configuration:**
Tailwind Browser v4 supports custom CSS via `@theme` directive:
```html
<style type="text/tailwindcss">
  @theme {
    --color-navy-medium: #4A6FA5;
    --color-navy-blue: #3D5A7A;
    --color-navy-blue-grey: #354A5F;
    --color-dark-slate: #2D3B4A;
    --color-muted-grey: #3A3E42;
    --color-sage-green: #8B9B88;
    --color-warm-sand: #E5DCC5;
    --color-cream: #F5F2E8;
  }
</style>
```

Then use in HTML as: `bg-navy-medium`, `text-navy-blue`, etc.

**Implementation Notes:**
- Use Tailwind's utility-first classes throughout
- Leverage responsive prefixes (`md:`, `lg:`, `xl:`) for breakpoints
- Define all brand colors in `@theme` block for consistent usage
- Keep HTML semantic and accessible

### Site Structure

**Pages:**
- `index.html` - Main portfolio/about page
- `rates.html` - Services and pricing page

**Key Features:**
- Card-based experience layout
- Responsive 2-column grid (`md:grid-cols-2`)
- Share button with clipboard functionality
- Smooth scrolling navigation
- Mobile-first responsive design

### Page Layout Specifications

#### 1. Header Navigation

**Structure:**
```
┌──────────────────────────────────────────────────────────┐
│  ⊚  Tom Counsell              [index] [rates] [Share]    │
│     Leading Dev Teams                                     │
│     Building Software                                     │
│     Millions Served                                       │
│                                                            │
│  [LinkedIn] [AngelList] [GitHub] [StackOverflow] [Telegram]│
└──────────────────────────────────────────────────────────┘
```

**Elements:**
- **Logo/Icon:** Circular geometric element (⊚) - concentric circles in brand navy, optional
- **Name:** Tom Counsell - Large display heading (Playfair Display)
- **Tagline:** Three-line format as shown in CONTENT.md
- **Navigation Links:**
  - "About" (links to index.html or #about)
  - "Rates" (links to rates.html)
  - "Share" (clipboard copy button)
- **Social Media Icons:** Horizontal row, icon-only buttons
  - LinkedIn, AngelList, GitHub, Stack Overflow, Telegram
  - Font Awesome icons

**Responsive:**
- Desktop: Full horizontal layout
- Tablet: Stacked, centered
- Mobile: Stacked, centered, smaller icons

#### 2. Experience Cards - Progressive Color
```
┌─────────────────────────────────┐
│ ⬤ 2024-Present  [Medium Navy]   │  ← Most recent
│ DeckFusion - CTO                 │
│ • Gen AI, data pipelines         │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│ ⬤ 2022-2023  [Navy Blue-Grey]   │  ← Recent past
│ Bumble/Official - Head of Eng    │
│ • React Native, scaling          │
└─────────────────────────────────┘

┌─────────────────────────────────┐
│ ⬤ 2018-Present  [Dark Slate]    │  ← Older/ongoing
│ Chainstarters - Advisor          │
│ • Blockchain, strategy           │
└─────────────────────────────────┘
```

#### 3. Skills/Tech Tags
**Inspired by:** Network node patterns

Instead of:
```
# Gen AI, prompt engineering, data pipelines
```

Use visual tags:
```
⬢ Gen AI  ⬢ Prompt Engineering  ⬢ Data Pipelines  ⬢ Startup
```

- Hexagon or circle bullets
- Monospace font
- Navy background with white text (pill-shaped)
- Hoverable to show connections

#### 4. Connection Visualization (Optional v2)
Show career progression as an **organic network diagram**:
- Each role = node
- Lines connect related experiences
- Technologies cluster in related groups
- Interactive hover states

---

## Component Specifications

### Card Component (Tailwind Implementation)

**HTML Structure:**
```html
<div class="relative overflow-hidden rounded-lg border-2 border-navy-blue shadow-lg p-6
            bg-gradient-to-br from-navy-medium to-navy-blue-grey">
  <!-- Texture overlay -->
  <div class="absolute inset-0 opacity-5 pointer-events-none"
       style="background-image: url('texture-pattern.svg');"></div>

  <!-- Card content -->
  <div class="relative z-10">
    <!-- Role and period -->
    <p class="text-cream text-sm">
      <strong>CTO</strong> 2024-present
    </p>

    <!-- Company name and logo -->
    <div class="flex items-center gap-4 my-4">
      <img src="static/img/company.png" alt="Logo" class="h-10" />
      <h3 class="text-2xl font-serif">Company Name</h3>
    </div>

    <!-- Description bullets -->
    <ul class="space-y-2 text-cream/90">
      <li>- Description point</li>
    </ul>

    <!-- Tech tags -->
    <div class="flex flex-wrap gap-2 mt-4">
      <span class="px-3 py-1 bg-navy-blue text-cream rounded-full text-xs font-mono">
        Tech Tag
      </span>
    </div>
  </div>
</div>
```

**Color Classes by Year:**
- 2024: `bg-gradient-to-br from-navy-medium to-navy-blue`
- 2023: `bg-gradient-to-br from-navy-blue to-navy-blue-grey`
- 2022: `bg-gradient-to-br from-navy-blue-grey to-dark-slate`
- 2021 & older: `bg-gradient-to-br from-dark-slate to-muted-grey`

### Circular Accent Element
```html
<div class="circle-accent">
  <div class="circle outer"></div>
  <div class="circle middle"></div>
  <div class="circle inner"></div>
</div>
```

Creates Bauhaus-style concentric circles as decorative elements.

### Tech Tag Component (Tailwind Implementation)
```html
<span class="inline-flex items-center gap-1 px-3 py-1 bg-navy-blue text-cream
             rounded-full text-xs font-mono">
  <span class="text-sage-green">⬢</span>
  Gen AI
</span>
```

**Variations:**
- Standard: `bg-navy-blue text-cream`
- Highlighted: `bg-sage-green text-dark-slate`
- Subtle: `bg-muted-grey text-cream/80`

---

## Content Hierarchy

### Page Priority (Visual Weight)
1. **Name & Title** - Largest, most prominent (Navy Blue)
2. **Current Role** (DeckFusion) - Medium navy card, top position
3. **Recent Experience** - Navy blue-grey, strong presence
4. **Skills/Technologies** - Visual tags, easily scannable
5. **About/Philosophy** - Secondary section
6. **Older Experience** - Dark slate/muted grey, recedes visually
7. **Contact/Social** - Accessible but not dominating

### Information Architecture
```
Header
  ├─ Name/Logo (with geometric accent)
  ├─ Tagline
  └─ Navigation (About, Experience, Rates, Contact)

Introduction
  ├─ Brief bio (2-3 sentences)
  └─ Core values visual (12 Rules as geometric pattern?)

Current Work
  └─ Featured card (DeckFusion) - Full width, medium navy

Experience Timeline
  ├─ Recent (2022-2024) - Medium navy/navy blue-grey cards
  ├─ Mid (2018-2021) - Dark slate cards
  └─ Legacy - Muted dark grey, collapsible/expandable section

Skills & Technologies
  ├─ Visual tag cloud
  └─ Grouped by category (AI, Infrastructure, Leadership)

About Section
  ├─ 12 Rules for Business (cleaner presentation)
  └─ Philosophy/approach

Footer
  ├─ Social links (minimal, icon-only)
  └─ Copyright
```

---

## Specific Implementations

### 1. List Layout (Network Graph Style)
For the **12 Rules for Business**, instead of plain list:

```
        1. Challenge status quo
       ╱
    ⬤────⬤ 2. Lead by example
   ╱      ╲
  ⬤        ⬤ 3. Promote curiosity
  │         ╲
  ⬤          ⬤ 4. Admit mistakes
  │           ╲
 ...          ...
```

Or cleaner card-based grid:
```
┌──────────────┐ ┌──────────────┐ ┌──────────────┐
│ ⬤ Rule 1     │ │ ⬤ Rule 2     │ │ ⬤ Rule 3     │
│ Challenge    │ │ Lead by      │ │ Promote      │
│ status quo   │ │ example      │ │ curiosity    │
└──────────────┘ └──────────────┘ └──────────────┘
```

### 2. Color Progression Implementation
Use CSS custom properties for easy theming:

```css
/* Years progress from medium navy to muted dark grey */
.year-2024 { --year-color: #4A6FA5; --year-opacity: 1.0; }
.year-2023 { --year-color: #3D5A7A; --year-opacity: 0.95; }
.year-2022 { --year-color: #354A5F; --year-opacity: 0.90; }
.year-2021 { --year-color: #2D3B4A; --year-opacity: 0.85; }
.year-2020 { --year-color: #323B45; --year-opacity: 0.80; }
.year-older { --year-color: #3A3E42; --year-opacity: 0.75; }
```

### 3. Texture Background
Create SVG pattern for subtle texture:

```html
<svg width="4" height="4" xmlns="http://www.w3.org/2000/svg">
  <line x1="0" y1="0" x2="4" y2="4"
        stroke="#1A3A52"
        stroke-width="0.5"
        opacity="0.1"/>
</svg>
```

Apply to cards as `background-image` at low opacity.

---

## Mobile Considerations

### Responsive Breakpoints (Tailwind)
- **Mobile:** `< 640px` - Single column, stacked cards
- **Tablet:** `sm: 640px` and `md: 768px` - 2-column grid starts
- **Desktop:** `lg: 1024px` and `xl: 1280px` - Full 2-column with optimal spacing
- **Wide:** `2xl: 1536px` - Maximum content width, extra padding

### Mobile-Specific
- Reduce geometric decoration (simpler patterns)
- Maintain color progression (critical for hierarchy)
- Touch-friendly spacing (min 44px tap targets)
- Simplified texture (may disable on very small screens)

---

## Success Metrics

### Visual Goals
✅ Immediate recognition as "strategic tech leader"
✅ Clean, professional, not corporate/sterile
✅ Geometric/Bauhaus aesthetic without being trendy
✅ Clear visual hierarchy (newest → oldest)
✅ Premium feel (textures, spacing, typography)

### User Goals
✅ Understand Tom's current role within 3 seconds
✅ Scan experience timeline effortlessly
✅ Feel the "stoic strategy" brand personality
✅ Easy navigation to rates/contact
✅ Mobile experience equals desktop quality

---

## Implementation Guide

### Build Order

**1. Setup HTML Boilerplate**
- Add Tailwind CDN script
- Define `@theme` colors
- Include Font Awesome CDN
- Add Playfair Display font (Google Fonts)
- Set up semantic HTML structure

**2. Build Header Component**
- Name and tagline
- Navigation links (About, Rates, Share)
- Social media icon row
- Share button with clipboard functionality

**3. Build Experience Cards**
- 2-column responsive grid (`grid md:grid-cols-2`)
- Card component with year-based color progression
- Company logo + name layout
- Tech tag pills
- Implement texture overlay

**4. Build About Section**
- Bio paragraphs
- 12 Rules for Business (grid or list layout)
- Profile image integration

**5. Build Rates Page**
- Testimonials section with quotes
- Pricing table
- Services lists
- Payment terms and discounts

**6. Polish & Testing**
- Add hover states
- Test mobile responsiveness
- Verify all links work
- Check accessibility
- Test share functionality

---

## References

**Inspiration Images:**
- `static/img/branding/01-geometric-patterns.webp` - Network diagrams for list layouts
- `static/img/branding/03-bauhaus-navy.webp` - Color progression (concentric circles)
- `static/img/branding/07-strategic-book.webp` - Texture inspiration (embossed surface)
- `static/img/branding/02-green-quote.webp` - Strategic messaging style
- `static/img/branding/09-neutral-tones.webp` - Quote treatment ("maps" reference)

**Brand Essence:**
"Stoic strategy future navy CTO app aesthetic" - Clean, strategic, technical, timeless.
