# Layout & Visual Hierarchy Reference — UX Movement Corpus

## Visual Hierarchy Fundamentals

### Law of De-Emphasis
"For the most important element to stand out, everything else must fade back."

Process:
1. Identify the single most important element
2. Strip everything else (no shapes, borders, colors)
3. Add back only what serves a clear purpose
4. Use font weight to create contrast without size inflation
5. Group related items; use icons for symbolic recognition

Anti-pattern: every element with equal visual weight → everything shouts, nothing registers.
"The Law of De-Emphasis for Clean UI Design"

### 60/30/10 Color Rule

| Role       | % of UI | Usage |
|------------|---------|-------|
| Neutral    | 60%     | Backgrounds, surfaces, space |
| Primary    | 30%     | Brand identity, sidebar, headings |
| Accent     | 10%     | CTAs, interactive state indicators |

Common failures:
- Primary at 60%+ → saturates, destroys signal-to-noise
- Accent at 20%+ → accent loses its directive power (attention no longer goes to actions)
- Neutral at 90%+ → flat, lifeless, no focal point

"60/30/10: The Color Ratio to Fix Ugly UIs"

### Diagonal Hierarchy Grid
- Users fixate top-left most; fixation rate decreases diagonally toward bottom-right
- Split screen into 3×3 grid
- High priority: top-left blocks (red zone)
- Medium priority: middle diagonal
- Low priority: bottom-right (yellow zone)
- "Diagonal Hierarchy Grid: A Method to Optimize Any Interface Layout"

## Whitespace

### The Design Secret Behind Balanced Whitespace
- Whitespace is not "empty" — it's a design element that creates focus
- Consistent spacing system (4px, 8px, 16px, 24px, 32px, 48px grid)
- Increase whitespace between unrelated elements; decrease between related ones
- "The Design Secret Behind Perfectly Balanced Whitespace"
- "The Sizing and Spacing System for Faster UI Design"

### Padding Ratios for Cards
- Internal padding: content-to-border distance (12–24px typical)
- Corner radius formula: outer radius = inner radius + padding
- "The Formula for Perfect Corners on Cards"

## Cards

**Card design principles**:
- Cards need a clear visual hierarchy: primary data > metadata > actions
- Use footer for metadata (secondary info, timestamps, tags)
- Multiple variants: default, selected, hover, disabled
- "Data Design Tips for Better UI Cards"
- "Why Your Cards Need a Footer for Metadata"
- "Why Your Cards Should Have Multiple Variants"

**Card layouts**:
- Vertical cards (portrait): better for images + text
- Horizontal cards: better for dense data, scannable lists
- "Vertical vs. Horizontal Cards: Which Are Better?"
- "Card Slicing: A Simple Method for Designing Better Grid Layouts"

**Content cards**:
- Cluttered content cards → use card slicing / tiered layout
- "A Better UX Design for Cluttered Content Cards"
- "How to Design Content Cards That Make Users Click"
- "How to Make Cluttered Content Cards Easier to Compare"

**Scan control on cards**:
- Z-pattern scan: image top → title → metadata → CTA
- Place primary info top-left
- "How Scan Control Improves the Readability of Content Cards"

## Grids & Responsive Layout

- Responsive card grids: use min-max column widths, not fixed columns
- "How to Design a Responsive Layout for Your Cards"
- "This 2-Column Grid Will Make Your Form Fields Responsive"

## Dashboards

Three-tier widget hierarchy:
1. Single primary KPI (largest, top, with progress indicator)
2. 3–4 supporting metrics (medium, with trend indicators)
3. Everything else (collapsed, no indicators, expandable)

Goal: users should see the most important number in <3 seconds.
"How to Simplify a 15 Widget Dashboard"

## Progressive Disclosure

- Reveal information on demand, not all at once
- Use "Show more", expandable sections, tabs, or step-by-step flows
- Apply to: optional form fields, long menus, data table columns, nested navigation
- "4 Ways to Apply Progressive Disclosure for Better Task Focus"
- "How to Simplify 6 Optional Fields with Toggle Switches"

## Surface Elevation & Depth

- Use shadows/elevation to indicate layer order (modals above page, tooltips above modals)
- Consistent elevation system: 0dp (flat), 2dp (cards), 4dp (dropdowns), 8dp (modals)
- Elevation signals interactivity: elevated = interactive layer
- "How to Use Surface Elevation to Elevate Your Interface"
- "The Art of User Interface Drop Shadows"

## Boxy vs Rich Interfaces

- Breaking out of "all rectangles" layout creates visual interest
- Use visual metaphors (cards that look like physical objects, progress rings, etc.)
- "How to Break Out of Boxy Interfaces with Visual Metaphors"
- "Primitive UI vs Evolved UI"

## Settings Pages

- Group related settings under section headings
- Use toggle switches for on/off settings
- Prefer a single-column layout for clarity on settings screens
- "Optimal Page Layout for Settings Screens"
- "How to Simplify a Long 15-Option Settings Page"
- "How to Simplify a Settings Screen with 45 Buttons"

## Content Density

- Too much content: apply progressive disclosure, collapse secondary items
- Too little content: don't add filler; whitespace is better than padding
- "6 Ways to Reduce Content Overload on List and Grid Layouts"
- "How to Make Any Information-Heavy Design Look Less Busy"
