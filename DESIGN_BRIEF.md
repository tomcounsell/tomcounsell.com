# Design Brief: Tom Counsell Portfolio Website
## tomcounsell.com

**Date:** October 30, 2025
**Version:** 2.0
**Project Type:** Minimalist Personal Website

---

## Brand Positioning

Tom Counsell is a strategic technology leader who combines:
- **Stoic Philosophy** - Calm, measured decision-making
- **Strategic Vision** - Seeing patterns others miss ("You call them dreams. I call them maps with many pathways")
- **Technical Excellence** - CTO-level expertise with modern tech, human-centered design, AI-powered
- **Design Thinking** - "With strategy, design transforms aesthetics into powerful ideas"
- **Growth Mindset** - Embracing change, learning, being ambitious, always seeing the next mountain beyond this mountain

---

## Site Structure

### Single-Page Layout
The site consists of one long-scrolling page with anchor-linked sections: Hero, About, Key Achievements, and Contact. The top navigation menu uses these anchors to smoothly scroll to each section.

**Pages:**
- `index.html` - Main single-page portfolio with all sections
- `rates.html` - Secondary page for detailed rates, testimonials, and contact information

**Anchor Navigation:** A simple header nav bar at the top of the page contains Tom's name or logo (linked to the top/hero) and short text links to "About", "Achievements", and "Contact." This allows quick jumps to each section.

**Mobile-First Approach:** The structure is planned mobile-first, meaning on small screens the content stacks vertically in one column (no side-by-side elements), and on larger screens it simply expands or centers within the available space.

---

## Design Constraints

### Light Theme Only
The site uses a light, airy color scheme:
- **Background:** Off-white (#FAFAFA) to avoid starkness and give a modern, soft feel
- **Text:** Dark charcoal (#111111 or similar) for maximum readability
- **High contrast** (dark text on light background) is critical for legibility
- The off-white background provides a subtle, contemporary finish and avoids eye strain

### No Animation or Gimmicks
- Static and calm design – no parallax, sliders, or animated effects
- Sections appear as the user scrolls without motion-based transitions
- Simple interactivity only (e.g., slight color change on hover)
- Keeps focus on content, aligns with minimalist philosophy

### Visual Hierarchy & Clarity
- Strong visual hierarchy guides user's eyes through the page in order of importance
- Achieved through typography (larger/bolder text for key info) and spacing
- Tom's name in Hero is largest text, immediately grabbing attention
- Section headings are smaller, body text is modest
- Plenty of whitespace, no clutter
- Easy to scan – main points visible in seconds

### Simplicity in Layout
- Straightforward vertical stack of content blocks
- No multiple columns or complex grids
- Visual elements (images, icons) used sparingly
- Consistent structure across sections (heading, then text or icons)
- Fast load times, clean look

### Responsive & Mobile-Friendly
- All elements sized and positioned with small screens in mind
- Buttons large enough to tap with finger
- Text legible on phone (no tiny font sizes)
- Images scale to screen width
- On desktop: sensible max-widths, use extra space as padding/margin

---

## Color Palette

### Primary Colors
```
Background:       #FAFAFA  (Off-white, light and airy)
Text Primary:     #111111  (Dark charcoal, nearly black)
Text Secondary:   #555555  (Medium gray for subtitles)
```

### Accent Color
Choose ONE muted accent color for highlights and interactive elements:
- Options: Soft teal (#52796F), dusty blue, or similar muted professional tone
- Low saturation to fit subdued aesthetic
- Used for:
  - Contact Me button background
  - Social media icon highlights
  - Hover states for links
  - Achievement icons (optional)
- Applied sparingly to draw attention where needed

### Usage Notes
- Monochromatic + accent scheme keeps design minimalist and cohesive
- All colors meet WCAG AA contrast standards
- No additional colors beyond grayscale and the single accent

---

## Typography

### Font System
**Primary Font:** Modern sans-serif throughout for clean, professional appearance
```css
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI",
             Roboto, "Helvetica Neue", Arial, sans-serif;
```

### Heading Hierarchy
- **H1 (Hero name):** 3rem (48px) on desktop, smaller on mobile, bold/extra-bold weight
- **H2 (Section titles):** 1.5rem to 2rem (24px-32px), medium/semi-bold weight
- **H3 (Sub-points):** 1.125rem (18px), medium weight
- **Body text:** 1rem (16px), line-height 1.6 for readability

### Font Weights & Styles
- Heavy weight for name
- Semibold for headings
- Regular for paragraphs
- Minimal use of italic (only for emphasis)

### Text Alignment
- Hero: center-aligned
- About: left-aligned (paragraph readability)
- Achievements: center-aligned under each icon
- Contact: center-aligned (CTA)

---

## Core Sections

### 1. Hero Section
The first screenful of content, communicating who Tom is.

**Elements:**
- **Portrait Image:** Tom's profile photo as a circle (~100px diameter mobile, larger on desktop)
  - Centered above name on all screen sizes
  - Friendly, modern look
- **Name and Title:**
  - "Tom Counsell" in large, bold font
  - Subtitle: "CTO & Technical Leader" (or similar) beneath in smaller text
- **Social Links:** Icons linking to professional profiles
  - LinkedIn, AngelList, GitHub, Stack Overflow, Telegram
  - Simple glyphs (~24px) in accent color or gray
  - Horizontal row with hover states
  - Limit to 3-4 most important networks

**Layout:** Central alignment, generous padding above and below

**Visual Hierarchy:** Photo → Name (largest text) → Title → Social icons

### 2. About Section
Concise introduction providing context about Tom's background and values.

**Elements:**
- **Section Heading:** "About" or "About Tom" (~2rem, bold)
- **Paragraph Content:** 4-5 sentences (~60-80 words)
  - Professional biography and personal qualities
  - Leadership, vision, technical authority in approachable tone
  - Example: "Tom bootstrapped his first successful startup, growing it to a multi-million-dollar enterprise..."
  - Focus on high-impact points that establish credibility

**Tone:** Confident but humble

**Format:** Normal paragraph, ~16px font size, left-aligned, centered within single column

**Visuals:** Minimal – no additional images (portrait already in Hero), possibly small decorative horizontal line

### 3. Key Achievements Section
Showcase Tom's notable accomplishments in visually engaging, quick-to-read format.

**Elements:**
- **Section Heading:** "Key Achievements" or "What I've Done"
- **Achievement Items:** 3-4 key points, each with icon and brief text
  - Example points: "Leading Dev Teams", "Building Software", "Millions Served"
  - Simple line icons or duotone icons in consistent style
  - Icons in accent color or gray (~32px)
  - Text: 1 line each, slightly larger or bold

**Layout:**
- Mobile: Stack vertically (one per line)
- Desktop: Horizontal row or grid (3 items in row, or 2x2 for 4 items)
- Centered within grid cells, consistent spacing between items
- Plenty of padding separating from sections above/below

**Visual Style:** Light, minimal, possibly uniform icon background shapes (circles)

### 4. Contact Section
Final section acting as call-to-action for getting in touch.

**Elements:**
- **Intro Text:** Short prompt (1-2 lines)
  - Example: "Interested in working with Tom? Let's get in touch."
- **Contact Button (CTA):** Prominent button in accent color
  - Text: "Contact Me" or "View Rates & Contact"
  - White text on accent background
  - Large size (0.75-1rem vertical padding, 2rem horizontal)
  - Links to `/rates.html` page
  - Simple hover effect (darker shade)

**Additional Info:**
- Could list email or social link for direct contact
- Or funnel all contact through button to rates page

**Layout:** Centered, padded, extra bottom padding to signify end of page

---

## Spacing & Layout Principles

### Vertical Rhythm
- Ample padding on top and bottom of each section
- Desktop: 4rem top/bottom, Mobile: 2rem
- Prevents cramped feel, enhances scanning

### Content Width
- Single-column layout
- Max width for paragraphs: 600-800px
- Centered in viewport, generous left/right margins on desktop

### Grid System
- Simple grids/flexbox inside sections:
  - Nav links: horizontal flex layout
  - Achievements: grid (1x3 desktop, 1xN mobile)

### Mobile Adaptation
- All elements stack vertically with full width
- Nav may collapse to hamburger menu
- Hero image centered, full width up to max size
- Achievements: one item per row
- Slightly reduced padding on mobile (but not cramped)

### Whitespace
- More spacing rather than less
- Consistent spacing scale (multiples of 4 or 8px)
- Tailwind spacing utilities: 4, 8, 16, 24, 32px

### No Borders or Shadows
- Separation via spacing rather than lines
- Very light 1px divider only if absolutely needed
- Flat design, no card-like shadows

---

## Imagery & Iconography

### Photography
- Only photograph: Tom's portrait in Hero
- Good-quality, friendly photo
- Cropped as circle (border-radius: 50%)
- Responsive size: ~8rem mobile, ~10rem desktop
- No background images or illustrations

### Icons
- Social links: Standard brand icons
- Achievements: Simple outline style icons
- Consistent style throughout (Material Design outlined or Font Awesome line)
- Rendered in accent color or dark gray
- Sizes: Social ~24px, Achievement ~32px
- Alt text for accessibility

### Logo/Branding
- Plain text for name preferred (strong font as "logo")
- If logo exists, should be simple and monochrome

### Favicon
- Simple favicon (maybe "T" or "TC" in accent color)

---

## Technical Implementation

### Framework
**Tailwind CSS via CDN (Browser version 4.x)**
```html
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
```

### Custom Theme Configuration
```html
<style type="text/tailwindcss">
  @theme {
    --color-bg-primary: #FAFAFA;
    --color-text-primary: #111111;
    --color-text-secondary: #555555;
    --color-accent: #52796F;  /* Muted teal - adjust as needed */
  }
</style>
```

### Implementation Notes
- Use Tailwind utility-first classes throughout
- Leverage responsive prefixes (`sm:`, `md:`, `lg:`)
- Keep HTML semantic and accessible
- No custom CSS beyond theme colors

---

## Semantic HTML Structure

```html
<body>
  <!-- Header with navigation -->
  <header>
    <nav>
      <!-- Site name/logo and anchor links -->
    </nav>
  </header>

  <!-- Main content wrapper -->
  <main>
    <!-- Hero Section -->
    <section id="hero" role="region">
      <img src="portrait.jpg" alt="Tom Counsell">
      <h1>Tom Counsell</h1>
      <p>CTO & Technical Leader</p>
      <!-- Social links -->
    </section>

    <!-- About Section -->
    <section id="about" role="region">
      <h2>About</h2>
      <p><!-- Biography --></p>
    </section>

    <!-- Achievements Section -->
    <section id="achievements" role="region">
      <h2>Key Achievements</h2>
      <ul><!-- Achievement items as list --></ul>
    </section>

    <!-- Contact Section -->
    <section id="contact" role="region">
      <h2>Get in Touch</h2>
      <p><!-- CTA text --></p>
      <a href="/rates.html">Contact Me</a>
    </section>
  </main>

  <!-- Footer (optional) -->
  <footer>
    <p>&copy; 2025 Tom Counsell</p>
  </footer>
</body>
```

---

## Secondary Page: rates.html

The rates page provides detailed information and maintains consistent styling with the main page.

**Content Sections:**
1. **Header** - Same navigation as index.html
2. **Hero/Intro** - Portrait, tagline, social links (consistent branding)
3. **Testimonials** - 5 quotes with attribution, clean blockquote styling
4. **Pricing Table** - Base Rate ($324/hr), FinTech ($486/hr), Consultancy ($648/hr)
5. **Services** - Core Services, Data & Analytics, Specialized Technologies, Integrations & Content
6. **Payment Terms** - Deposit, invoicing schedule
7. **Discounts** - Referral discounts, non-profit rates
8. **Additional Assurances** - Confidentiality, IP ownership, flexibility
9. **Footer** - Consistent with index.html

**Design Approach:**
- Light background (#FAFAFA)
- Clean typography, sans-serif throughout
- Minimal use of Bootstrap (from legacy implementation)
- Or full rebuild with Tailwind matching index.html aesthetic
- Generous spacing between sections
- Simple table for rates
- Service items in clean card/list format

---

## Accessibility & UX Considerations

- High contrast design inherently helps accessibility
- Proper heading structure (H1, H2s in order)
- Alt text on all images
- Sufficient color contrast (WCAG AA compliance)
- Mobile-first, no-animation approach good for performance
- Reduced motion preferences respected
- Anchor navigation obvious, possibly fixed nav bar
- No content relies on color alone
- Clear form labels (if contact form included)

---

## Responsive Breakpoints (Tailwind)

- **Mobile:** `< 640px` - Single column, stacked content
- **Tablet:** `sm: 640px`, `md: 768px` - Slight expansion, still mostly single column
- **Desktop:** `lg: 1024px`, `xl: 1280px` - Full layout with optimal spacing
- **Wide:** `2xl: 1536px` - Maximum content width, extra padding

---

## Success Metrics

### Visual Goals
✅ Immediate recognition as strategic tech leader
✅ Clean, professional, not corporate/sterile
✅ Minimalist aesthetic without being trendy
✅ Clear visual hierarchy
✅ Light, airy feel with excellent readability

### User Goals
✅ Understand who Tom is within 3 seconds
✅ Scan key achievements effortlessly
✅ Feel the "stoic strategy" brand personality
✅ Easy navigation to rates/contact
✅ Mobile experience equals desktop quality

---

## Implementation Guide

### Build Order

**1. Setup HTML Boilerplate**
- Add Tailwind CDN script
- Define `@theme` colors (off-white, charcoal, accent)
- Include Font Awesome CDN for icons
- Set up semantic HTML structure

**2. Build Hero Section**
- Circular portrait image
- Name and title (large, bold typography)
- Social media icon row
- Central alignment, generous padding

**3. Build About Section**
- Section heading
- 4-5 sentence biography paragraph
- Single column, left-aligned text
- Max width constraint for readability

**4. Build Key Achievements Section**
- Section heading
- 3 achievement items with icons and short text
- Responsive grid (1 column mobile, 3 columns desktop)
- Center-aligned content

**5. Build Contact Section**
- Section heading and intro text
- Large CTA button linking to rates.html
- Center-aligned, prominent accent color

**6. Build Header Navigation**
- Simple nav bar with anchor links
- Mobile hamburger menu (optional)
- Share button functionality

**7. Style rates.html**
- Maintain consistent header/footer
- Clean presentation of testimonials
- Simple pricing table
- Service lists with clear formatting

**8. Polish & Testing**
- Test all anchor links
- Verify mobile responsiveness at all breakpoints
- Check accessibility (semantic HTML, alt text, contrast)
- Test share button clipboard functionality
- Verify all external links work

---

## Brand Essence

"Clean, strategic, minimalist personal website for a stoic CTO" - Light, airy, focused on content over decoration, emphasizing Tom's leadership and technical excellence through simplicity and clarity.

---

## References

**Design Inspiration:**
- Minimalist single-page portfolio sites
- Modern SaaS landing pages (clean, light aesthetic)
- Professional personal brands in tech

**Content Sources:**
- `CONTENT.md` - All copy and biographical information
- `CLAUDE.md` - Project documentation and technical notes
- Tom's existing site at tomcounsell.com for legacy reference
