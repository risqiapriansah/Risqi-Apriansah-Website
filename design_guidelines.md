# Design Portfolio Website Guidelines

## Design Approach
**Reference-Based Approach** - Drawing inspiration from premium design portfolios (Behance, Dribbble, award-winning designer portfolios) while maintaining clean, content-forward aesthetics. This portfolio must demonstrate exceptional design sensibility through its own presentation.

## Core Design Principles
1. **Visual Hierarchy First** - Let the work speak through generous imagery and strategic whitespace
2. **Grid-Based Structure** - Precise alignment and modular layouts
3. **Typography as Design** - Bold use of type to create visual interest without competing with portfolio pieces
4. **Restrained Interaction** - Purposeful micro-interactions that enhance, never distract

## Typography System

**Primary Font**: Inter or Work Sans (Google Fonts)
- Headings: 700 weight
- Body: 400 weight
- Captions: 500 weight

**Scale**:
- Hero/Display: text-6xl to text-8xl (60-96px)
- Project Titles: text-4xl to text-5xl (36-48px)
- Section Headers: text-2xl to text-3xl (24-36px)
- Body Text: text-base to text-lg (16-18px)
- Metadata/Tags: text-sm (14px)

## Layout & Spacing

**Spacing Primitives**: Use Tailwind units of 4, 6, 8, 12, 16, 20, 24 (p-4, m-8, gap-12, etc.)

**Container Strategy**:
- Max width: max-w-7xl for main content areas
- Gallery grids: Full-width with inner padding (px-8 md:px-12 lg:px-16)
- Project content: max-w-4xl for optimal reading

**Vertical Rhythm**: py-16 to py-24 for section spacing

## Component Library

### Navigation
Sticky top navigation with minimal height (h-16 to h-20), logo left, filter/menu right. Simple underline hover states for links.

### Gallery Grid
- Desktop: 3 columns (grid-cols-3)
- Tablet: 2 columns (grid-cols-2)
- Mobile: 1 column (grid-cols-1)
- Gap: gap-6 to gap-8
- Cards: Aspect ratio 4:3, hover state with subtle scale (hover:scale-[1.02])
- Project metadata below thumbnail (title, categories, year)

### Filter System
Horizontal pill-style buttons with gap-3, active state distinguishable through typography weight and subtle background treatment.

### Project Page Structure
1. **Hero**: Full-width project hero image (aspect-[16/9]) with overlay text (project title, role, year)
2. **Overview**: 2-column layout (problem/solution) with max-w-5xl
3. **Process Sections**: Full-width sections alternating between text and visuals
   - Discovery: Text-heavy with supporting images
   - Sketches: Image grid (2-3 columns)
   - Wireframes: Larger images (1-2 columns) 
   - Iterations: Before/after comparisons
4. **Figma Embeds**: Full-width container with 16:9 aspect ratio, responsive iframe scaling
5. **Project Navigation**: Fixed bottom bar or inline next/prev links

### Style Guide Page
Organized sections with clear visual separation:
- **Typography**: Live examples of each scale level
- **Color System**: Swatch grid with hex values and usage context
- **Components**: Interactive component showcase (buttons, cards, inputs)
- **Spacing**: Visual ruler showing token scale

## Images

### Hero Image
Large hero image on homepage (aspect-[21/9] or full viewport height) showcasing selected work or creative composition. Use blur backdrop for any CTAs overlaid on hero.

### Gallery Thumbnails
High-quality project thumbnails for each portfolio piece - mockups, key screens, or hero shots representing the work.

### Process Documentation
Within project pages, include images for:
- Sketches and early concepts
- Wireframe screenshots
- Design iteration comparisons
- Final deliverable mockups
- User testing photos (if applicable)

All images should maintain consistent aspect ratios within their sections for visual harmony.

## Page-Specific Layouts

**Homepage**: 
- Minimal hero with headline + optional CTA
- Filter bar (sticky below nav)
- Project grid gallery
- Simple footer

**Project Pages**:
- Immersive hero
- Structured content sections with clear visual breaks
- Embedded Figma prototypes
- Related projects carousel at bottom

**Style Guide**:
- Sidebar navigation (desktop) listing all sections
- Content area showcasing live examples
- Copy-to-clipboard functionality for color codes and tokens

## Interaction Patterns
- Smooth page transitions
- Filter animations (fade in/out)
- Lazy loading for images
- Scroll-triggered reveal for process sections (subtle fade-up)
- Hover states: Scale (1.02), opacity shifts (0.9), or subtle shadows

**Critical**: Blur backgrounds (backdrop-blur-sm) for any buttons placed over images.