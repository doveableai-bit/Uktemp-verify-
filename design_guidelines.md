# UK Temp Numbers - Design Guidelines

## Design Approach

**Selected Approach:** Design System-based with Material Design influence, prioritizing utility and trust for a verification service.

**Rationale:** This is a utility-focused tool where users need to quickly find numbers, copy them, and receive verification codes. The design must establish trust and credibility while maintaining excellent usability and clarity.

---

## Core Design Elements

### A. Typography

**Font Family:** 
- Primary: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif (system fonts for optimal performance and familiarity)

**Typography Scale:**
- Hero Heading: 2.5rem (40px) / Font Weight: 600
- Section Titles: 2.2rem (35px) / Font Weight: 600
- Card Headers: 1.3rem (21px) / Font Weight: 600
- Phone Numbers: 1.5rem (24px) / Font Weight: 700
- Body Text: 1rem (16px) / Font Weight: 400 / Line Height: 1.6
- Small Text: 0.85rem (14px) / Font Weight: 400

**Hierarchy:**
- Use bold weights (600-700) for critical information like phone numbers and verification codes
- Maintain consistent heading sizes across sections
- Keep body text at comfortable reading size with generous line-height

### B. Color Palette

**Primary Colors:**
- Primary Blue: #2a5298
- Deep Blue: #1e3c72
- Gradient: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%)

**Accent Colors:**
- Action Red: #ff6b6b (CTA buttons)
- Success Green: #28a745 (available status, phone icons)
- Alert Red: #c62828 (in-use status)

**Neutral Colors:**
- Background: #f5f7fa
- Card White: #ffffff
- Light Gray: #f8f9fa
- Border Gray: #ddd, #eee
- Text Primary: #333
- Text Secondary: #666
- Text Tertiary: #999

**Status Colors:**
- Available: Background #e8f5e9 / Text #2e7d32
- In Use: Background #ffebee / Text #c62828
- Code Highlight: Background #e3f2fd / Text #1565c0

### C. Layout System

**Spacing Units:** Use Tailwind-equivalent spacing of 2, 4, 8, 12, 15, 20, 25, 30 for consistent rhythm.

**Container:**
- Max-width: 1200px
- Horizontal padding: 20px
- Center-aligned

**Grid System:**
- Number Cards: CSS Grid with auto-fill, minmax(300px, 1fr)
- Footer Columns: Flexbox with equal flex distribution
- Steps Section: Flexbox with equal distribution

**Section Spacing:**
- Section padding: 3rem vertical (48px)
- Element margins: 1rem to 2rem between major elements
- Card gaps: 25px in grid layouts

### D. Component Library

**Navigation:**
- Fixed header with gradient background
- Horizontal navigation with 25px gaps
- Links with subtle hover state (light blue #a8d0ff)
- Logo with icon + text combination

**Hero Section:**
- Full-width gradient overlay on background image
- Center-aligned content
- Large heading with descriptive subtext
- Single prominent CTA button
- Padding: 4rem vertical

**Number Cards:**
- White background with subtle shadow
- Rounded corners: 10px
- Header section with colored background (primary blue)
- Body with phone number as primary element
- Footer with action buttons
- Hover effect: lift (-5px translateY) with enhanced shadow
- Status badges with rounded corners (20px)

**Phone Number Display:**
- Large, bold display (1.5rem, weight 700)
- Icon prefix (mobile phone)
- Primary blue color
- Flex layout with gap

**Buttons:**
- Primary CTA: Red background (#ff6b6b), white text, rounded (30px), padding 12px 30px
- Secondary: Blue background (#2a5298), white text, rounded (5px), padding 8px 15px
- Ghost: Light background (#f8f9fa), border, rounded (30px or 5px)
- Hover states: Slight color darkening + translateY(-3px) for CTA
- Active state for filter buttons: filled with primary color

**Message Cards:**
- White background container with rounded corners
- Each message as bordered row
- Sender name bold
- Verification code highlighted with colored background
- Timestamp in light gray
- Scrollable container (max-height: 400px)

**Status Badges:**
- Small, rounded pills (border-radius: 20px)
- Colored backgrounds with matching text
- Padding: 5px 12px
- Font size: 0.85rem, weight 600

**Steps/Features:**
- Equal-width columns with minimum 250px
- Light gray background (#f8f9fa)
- Large icons (2.5rem) in primary blue
- Center-aligned text
- Rounded containers (10px)

**Footer:**
- Dark background (#1a1a2e)
- Multi-column layout with flex
- Light text with subtle accent color (#a8d0ff) for headings
- Border-top separator for copyright
- Links with hover transition to accent color

### E. Interactive Elements

**Hover States:**
- Cards: Lift with shadow enhancement
- Links: Color change to #a8d0ff
- Buttons: Background darkening + optional lift
- Filter buttons: Background color change

**Transitions:**
- Standard: 0.3s ease for all transitions
- Consistent timing across all interactive elements

**Icons:**
- Font Awesome 6.4.0 via CDN
- Icon sizes: 2rem for logo, 2.5rem for step icons, standard sizes for inline usage
- Colors match context (green for success, blue for primary actions)

### F. Responsive Behavior

**Breakpoint: 768px (mobile/tablet)**
- Header: Stack logo and navigation vertically
- Navigation gaps: Reduce to 15px
- Hero heading: Reduce to 2rem
- Number grid: Single column layout
- Steps: Stack vertically
- Footer: Allow natural wrapping of columns

**Mobile-First Considerations:**
- All text remains readable at base sizes
- Touch targets minimum 44x44px
- No horizontal scrolling
- Generous padding maintained

---

## Images

**Hero Background:**
- Source: London cityscape/phone technology themed image (currently using London phone booth)
- Treatment: Dark gradient overlay (rgba(30, 60, 114, 0.9), rgba(42, 82, 152, 0.9))
- Coverage: Full-width, background-size: cover
- Position: Center

**Purpose:** Establishes UK identity and technical credibility while maintaining text readability through gradient overlay.

---

## Key Design Principles

1. **Trust Through Clarity:** Large, readable phone numbers with clear status indicators build confidence
2. **Immediate Access:** Critical actions (copy, use number) prominently placed and easily accessible
3. **Visual Hierarchy:** Phone numbers and verification codes are the most prominent elements
4. **Consistent Feedback:** Clear status states for numbers (available vs in-use) and instant copy feedback
5. **Credibility:** Professional gradient theme, clean cards, and structured layout establish service reliability
6. **Scannability:** Grid layout allows quick browsing of available numbers with filtering options
7. **Functional Beauty:** Design serves the utility purpose while maintaining modern, polished aesthetics