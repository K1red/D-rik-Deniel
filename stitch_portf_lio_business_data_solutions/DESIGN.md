---
name: Precision Engine
colors:
  surface: '#111317'
  surface-dim: '#111317'
  surface-bright: '#37393e'
  surface-container-lowest: '#0c0e12'
  surface-container-low: '#1a1c20'
  surface-container: '#1e2024'
  surface-container-high: '#282a2e'
  surface-container-highest: '#333539'
  on-surface: '#e2e2e8'
  on-surface-variant: '#c2c6d6'
  inverse-surface: '#e2e2e8'
  inverse-on-surface: '#2f3035'
  outline: '#8c909f'
  outline-variant: '#424754'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e6a'
  primary-container: '#4d8eff'
  on-primary-container: '#00285d'
  inverse-primary: '#005ac2'
  secondary: '#4edea3'
  on-secondary: '#003824'
  secondary-container: '#00a572'
  on-secondary-container: '#00311f'
  tertiary: '#ffb95f'
  on-tertiary: '#472a00'
  tertiary-container: '#ca8100'
  on-tertiary-container: '#3e2400'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a42'
  on-primary-fixed-variant: '#004395'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#111317'
  on-background: '#e2e2e8'
  surface-variant: '#333539'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  mono-data:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 20px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style

This design system is engineered for professionals in RevOps, Data Engineering, and IA. The brand personality is **analytical, high-performance, and sophisticated**, designed to convey technical mastery and operational efficiency. 

The aesthetic is a hybrid of **Minimalism** and **Glassmorphism**, specifically optimized for a dark, data-heavy environment. It prioritizes information density without sacrificing clarity, using structured grid patterns and subtle background blurs to create a sense of digital depth. The UI should evoke a "Command Center" emotional response—controlled, intelligent, and focused on actionable insights.

## Colors

The palette is rooted in a "Deep Space" dark mode. The primary background uses a near-black charcoal to minimize eye strain and maximize the pop of data visualizations. 

- **Primary (Vibrant Blue):** Reserved for primary actions, active states, and growth-oriented data trends.
- **Secondary (Emerald Green):** Used for success states, positive deltas, and completed milestones.
- **Tertiary (Amber):** Used for warnings, pending tasks, or middle-tier performance metrics.
- **Surface Strategy:** Layers are defined by hex-value elevation. The canvas is the darkest, while cards and interactive elements use slightly lighter charcoal values with subtle borders to maintain separation.

## Typography

The system utilizes **Inter** for its exceptional legibility in data-dense interfaces and its neutral, technical character. 

- **Data Presentation:** For numeric values and code snippets, the system introduces a secondary monospace font (**JetBrains Mono**) to ensure character alignment and a "data-first" feel.
- **Hierarchy:** High contrast in font weights is used to distinguish between metadata (Labels) and primary insights (Headlines). 
- **Readability:** Line heights are kept slightly tighter for labels and data tables to maintain density, while body text uses a generous 1.5x ratio for long-form case studies.

## Layout & Spacing

The layout utilizes a **12-column fluid grid** for desktop and a **4-column grid** for mobile. 

- **Grid Philosophy:** The design system employs a 4px baseline grid. All margins and paddings must be multiples of 4.
- **Data-Inspired Patterns:** Backgrounds should feature a subtle dot-matrix pattern (1px dots, 24px spacing) to reinforce the engineering theme.
- **Sectioning:** Content is grouped into logical "Modules" or cards. Gutters are kept tight (20px) to maximize the screen real estate for charts and tables.
- **Mobile Reflow:** On mobile, complex data tables should transition to card-based summaries or include horizontal scroll containers with sticky lead columns.

## Elevation & Depth

Visual hierarchy is achieved through a combination of **Tonal Layering** and **Glassmorphism**:

- **Layers:** 
  - Level 0: Canvas (#09090B) with dot-matrix pattern.
  - Level 1: Standard Cards (#18181B) with a 1px solid border (#27272A).
  - Level 2: Overlays/Modals with a 40% opacity blur (Backdrop-filter: blur(12px)).
- **Shadows:** Avoid heavy black shadows. Use "Ambient Glows" for primary cards—a very low-opacity blue or neutral tint (0,0,0, 0.5) with a large spread (24px) to suggest the element is lifting off the surface.
- **Glass Effect:** Interactive states (like hovered table rows) should use a subtle semi-transparent white overlay (5% opacity) to create a "frost" effect over the background.

## Shapes

The shape language is **sharp and professional**. 

- **Radius:** A standard `0.25rem` (4px) radius is used for buttons, input fields, and small UI components to maintain a technical, "hardware" feel. 
- **Large Components:** Larger containers like main dashboard cards use `rounded-lg` (8px) to provide just enough softness to feel modern without losing the precision-engineered look.
- **Graphs:** Data points in line charts should be sharp (square or diamond), while bar charts should have 0px roundedness on the bottom and 2px on the top.

## Components

- **Buttons:** Primary buttons use the vibrant blue with white text. Ghost buttons use a 1px border (#27272A) and transition to a subtle white fill (10% opacity) on hover.
- **Data Chips:** Small, pill-shaped tags used for status (e.g., "In Progress", "Deployed"). Use low-saturation background tints of the accent colors with high-saturation text.
- **Input Fields:** Darker than the card background (#0F1115) with a 1px border. The focus state uses a 1px blue border and a subtle blue outer glow.
- **Data Cards:** Every card must have a "Header" section containing a Label-SM title and optional "View Details" icon.
- **Progress Bars:** Use a thick 8px track with the secondary green for completion. Tracks should be background-neutral with a 10% opacity.
- **KPI Metrics:** Large display numbers should be accompanied by a small "trend" indicator (up/down arrow) using the green/red semantic colors.