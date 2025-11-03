# Design Brief: Tom Counsell Portfolio Website
## tomcounsell.com

**Date:** October 30, 2025
**Version:** 2.1
**Project Type:** Modern Professional Portfolio

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

### Long-Scrolling Portfolio Layout
The site consists of one long-scrolling page with anchor-linked sections: Hero, About, Professional Experience, and Contact. The top navigation menu uses these anchors to smoothly scroll to each section.

**Pages:**
- `index.html` - Main portfolio with professional experience cards
- `rates.html` - Secondary page for detailed rates, testimonials, and contact information

**Anchor Navigation:** A simple header nav bar at the top of the page contains Tom's name or logo (linked to the top/hero) and short text links to "About", "Experience", and "Contact." This allows quick jumps to each section.

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

### Balance in Layout
- Vertical stack of content blocks with visual interest
- Single-column for experience cards, grid layouts for other sections where appropriate
- Visual elements (company logos, icons) used to enhance credibility and scannability
- Consistent structure across sections with variation to maintain interest
- Fast load times, professional appearance

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
Soft teal (#52796F) as the primary accent color for highlights and interactive elements:
- Used for:
  - Contact/CTA button backgrounds
  - Social media icon highlights
  - Hover states for links
  - Company name/role headers in experience cards
  - Section dividers or decorative elements
  - Tag/label backgrounds for technologies
- Applied consistently throughout to create cohesion

### Secondary Colors
Additional subtle colors for visual interest:
- Light teal background for alternating sections (#F0F5F4)
- Soft borders and dividers using gray tones
- Technology tags can use muted color variations

### Usage Notes
- Primary accent + subtle secondary colors create visual interest without overwhelming
- All colors meet WCAG AA contrast standards
- Color used meaningfully, not just decoration

---

## Typography

### Font System
**"Tom Counsell" Name Display:** Display serif - balanced, readable, authoritative
```css
font-family: "Playfair Display", "Libre Baskerville", "Lora", Georgia, serif;
```
Use one of: Playfair Display, Libre Baskerville, or Lora for the name "Tom Counsell" wherever it appears (H1, navigation, footer, etc.)

**Headings (H2-H4):** Serif font for elegance and distinction
```css
font-family: "Playfair Display", "Libre Baskerville", "Lora", Georgia, serif;
```

**Body & UI:** Modern sans-serif for readability
```css
font-family: -apple-system, BlinkMacSystemFont, "Segoe UI",
             Roboto, "Helvetica Neue", Arial, sans-serif;
```

### Heading Hierarchy
- **H1 (Hero name):** 3rem (48px) on desktop, serif, bold/extra-bold weight
- **H2 (Section titles):** 1.75rem to 2.25rem (28px-36px), serif, semibold
- **H3 (Experience roles, sub-sections):** 1.25rem (20px), serif, medium weight
- **H4 (Company names):** 1rem (16px), serif or sans-serif, semibold, accent color
- **Body text:** 1rem (16px), sans-serif, line-height 1.6 for readability
- **Small text (dates, tags):** 0.875rem (14px), sans-serif

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
The first screenful of content, communicating who Tom is. **This section should make a strong first impression.**

**Elements:**
- **Portrait Image:** Tom's professional photo as a large circle
  - **Primary visual anchor of the page** - make it prominent
  - Centered above name on all screen sizes
  - As large as the design allows while maintaining balance (160px+ mobile, 320px+ desktop)
  - Tom's professional appearance (handsome, well-dressed) conveys trust and leadership
  - High-quality image with subtle shadow for polish
- **Name and Title:**
  - "Tom Counsell" in large, bold serif font (Playfair Display)
  - Subtitle: "CTO & Technical Leader" beneath in smaller text
- **Social Links:** Icons linking to professional profiles
  - LinkedIn, AngelList, GitHub, Stack Overflow, Telegram (all 5)
  - Simple glyphs in accent color or gray
  - Horizontal row with hover states
  - Generous sizing and spacing

**Layout:** Central alignment, generous padding above and below, extra vertical space to let the portrait breathe

**Visual Hierarchy:** Large Photo (hero element) → Name (largest text) → Title → Social icons

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

### 3. Professional Experience Section
Showcase Tom's career history with detailed experience cards for each role.

**Elements:**
- **Section Heading:** "Professional Experience" or "Experience"
- **Experience Cards:** One card per role/company (8-10 cards from CONTENT.md)
  - Company logos (42px height, maintaining aspect ratio)
  - Role title (H3, serif, prominent)
  - Company name (H4, accent color, linked)
  - Date range (small text, gray)
  - 3-5 bullet points describing responsibilities and impact
  - Technology tags (small rounded badges with light backgrounds)
  - Cards can use subtle borders, light shadows, or alternating background colors

**Layout:**
- Single-column layout for readability
- Each card has generous padding (1.5-2rem)
- Consistent spacing between cards
- Mobile: Full width stacked
- Desktop: Centered with max-width for readability

**Visual Style:**
- Clean card-based design with subtle depth
- Logos add visual interest and credibility
- Technology tags provide scannable information
- Professional but not corporate

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

### Subtle Depth & Separation
- Light borders (1px, subtle gray) for card definition
- Gentle shadows (shadow-sm, shadow-md) for depth and hierarchy
- Alternating background colors for section variation
- Not flat, but not heavy - balanced approach

---

## Imagery & Iconography

### Photography & Logos
- **Portrait:** Tom's professional photo in Hero section
  - High-quality photo showcasing Tom's professional presence
  - Tom is handsome and well-dressed, evoking trust and strength
  - **Make the image as large as possible while keeping the design clean**
  - Cropped as circle (border-radius: 50%)
  - Suggested sizes: 160px mobile, 240px tablet, 320px desktop (or larger if layout permits)
  - Prominent placement - this image builds immediate credibility
  - Subtle shadow for depth and polish
  - The portrait should be a hero element, not an afterthought
- **Company Logos:** In experience cards
  - 42px height, maintaining aspect ratio
  - Positioned near company name/role
  - Adds credibility and visual interest
- No decorative background images or illustrations

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
    --color-bg-secondary: #F0F5F4;
    --color-text-primary: #111111;
    --color-text-secondary: #555555;
    --color-accent: #52796F;
    --color-accent-light: #6B9B8F;
  }
</style>
```

### Display Serif Font (Choose One)
**Option 1: Playfair Display** (elegant, classic)
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&display=swap" rel="stylesheet">
```

**Option 2: Libre Baskerville** (traditional, readable)
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Libre+Baskerville:wght@400;700&display=swap" rel="stylesheet">
```

**Option 3: Lora** (modern, balanced)
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Lora:wght@400;600;700&display=swap" rel="stylesheet">
```

**Font Stack:** Use one primary font with fallbacks
```css
/* Apply to "Tom Counsell" name and all headings */
font-family: "Playfair Display", "Libre Baskerville", "Lora", Georgia, serif;
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

    <!-- Professional Experience Section -->
    <section id="experience" role="region">
      <h2>Professional Experience</h2>
      <div><!-- Experience cards from CONTENT.md --></div>
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

**4. Build Professional Experience Section**
- Section heading
- Experience cards for each role (8-10 from CONTENT.md)
- Include: company logo, role, dates, description bullets, technology tags
- Single-column stacked layout
- Subtle borders/shadows for card definition

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

"Modern, professional portfolio for a strategic CTO" - Clean and well-designed with substantive content. Balances visual appeal with information density. Showcases Tom's impressive career trajectory with elegance and credibility. Professional without being corporate, modern without being trendy.

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
