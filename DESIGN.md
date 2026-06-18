---
name: Syntactic Flux
colors:
  surface: '#fdf7ff'
  surface-dim: '#ded8e0'
  surface-bright: '#fdf7ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f8f2fa'
  surface-container: '#f2ecf4'
  surface-container-high: '#ece6ee'
  surface-container-highest: '#e6e0e9'
  on-surface: '#1d1b20'
  on-surface-variant: '#494551'
  inverse-surface: '#322f35'
  inverse-on-surface: '#f5eff7'
  outline: '#7a7582'
  outline-variant: '#cbc4d2'
  surface-tint: '#6750a4'
  primary: '#4f378a'
  on-primary: '#ffffff'
  primary-container: '#6750a4'
  on-primary-container: '#e0d2ff'
  inverse-primary: '#cfbcff'
  secondary: '#63597c'
  on-secondary: '#ffffff'
  secondary-container: '#e1d4fd'
  on-secondary-container: '#645a7d'
  tertiary: '#765b00'
  on-tertiary: '#ffffff'
  tertiary-container: '#c9a74d'
  on-tertiary-container: '#503d00'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#cfbcff'
  on-primary-fixed: '#22005d'
  on-primary-fixed-variant: '#4f378a'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#cdc0e9'
  on-secondary-fixed: '#1f1635'
  on-secondary-fixed-variant: '#4b4263'
  tertiary-fixed: '#ffdf93'
  tertiary-fixed-dim: '#e7c365'
  on-tertiary-fixed: '#241a00'
  on-tertiary-fixed-variant: '#594400'
  background: '#fdf7ff'
  on-background: '#1d1b20'
  surface-variant: '#e6e0e9'
typography:
  display-xl:
    fontFamily: Outfit
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-xl-mobile:
    fontFamily: Outfit
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-lg:
    fontFamily: Outfit
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  mono-label:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
  metric-num:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  section-gap: 120px
  section-gap-mobile: 64px
---

## Brand & Style

The design system is engineered for a Data Engineering portfolio, focusing on the intersection of raw computational power and refined architectural precision. The brand personality is technical, transparent, and authoritative. It targets hiring managers and technical leads who value clarity in complex data pipelines.

The visual style is **High-Contrast Minimalism with a Developer-Centric edge**. It utilizes expansive whitespace (or "blackspace" in dark mode) to allow technical documentation and metrics to breathe. The aesthetic balances a clean, professional SaaS interface with the "terminal" feel favored by engineers, achieved through the strategic use of monospaced accents and high-chroma primary colors.

## Colors

The palette is bifurcated to provide two distinct emotional responses:
- **Light Mode:** Professional, academic, and accessible. Uses a deep "Google Blue" (#1A73E8) to signify reliability and trust.
- **Dark Mode:** High-energy, technical, and reminiscent of IDE environments. Uses a vibrant "Matrix Green" (#00FF41) to highlight active data flows and terminal outputs.

Both modes rely on absolute backgrounds (#FFFFFF and #000000) to maximize contrast ratios for accessibility. Accent colors should be used sparingly for primary actions, metrics, and syntax highlighting in code blocks.

## Typography

Typography distinguishes between narrative content and technical data.
- **Outfit** is used for large displays and headlines. Its geometric construction feels modern and approachable.
- **Inter** handles all body copy, ensuring maximum readability for long-form project descriptions.
- **Geist** (Monospace) is utilized for "metadata"—labels, technology tags, code snippets, and metrics.

In Dark Mode, the font weight of Inter should be slightly reduced (e.g., 400 to 300) or letter spacing increased by 0.01em to prevent visual "glow" or blurring on high-contrast screens.

## Layout & Spacing

This design system employs a **Fluid Grid** model with high internal padding. 
- **Desktop:** 12-column grid with 24px gutters. Content is centered within a 1280px max-width container.
- **Mobile:** 4-column grid with 16px margins. 

The vertical rhythm is defined by a 120px "Section Gap," creating the "Spacious" feel requested. This encourages focus on one project or experience at a time. Project cards should use an internal padding of `40px` (5 units) to maintain the minimalist aesthetic.

## Elevation & Depth

To maintain the minimalist and high-contrast aesthetic, this design system avoids heavy drop shadows. Instead, it uses **Tonal Layers and Subtle Borders**:

- **Level 0 (Background):** Absolute #FFFFFF or #000000.
- **Level 1 (Cards/Surfaces):** A subtle fill (#F3F4F6 in Light / #111111 in Dark) with a 1px solid border.
- **Borders:** In Light Mode, use `rgba(0,0,0,0.08)`. In Dark Mode, use `rgba(255,255,255,0.15)`.
- **Hover States:** Instead of lifting an element with a shadow, the border color should shift to the `primary_color` to indicate interactivity.

A "Glassmorphism" effect is reserved exclusively for the Navigation Bar, using a 12px backdrop blur and semi-transparent background to maintain context while scrolling.

## Shapes

The design system uses a **Rounded (Level 2)** language with specific overrides for large components to achieve the "XL" feel:
- **Small Components (Pills/Tags):** Fully rounded (height / 2).
- **Standard Cards:** 1rem (16px) radius.
- **Large Sections/Containers:** 1.5rem (24px) radius.

Buttons and Inputs follow the 16px standard, creating a soft contrast against the rigid, high-contrast grid.

## Components

### Navigation Bar
A fixed top-bar with a `blur(12px)` backdrop. It features a logo on the left, centered navigation links using `mono-label` typography, and a "Mode Toggle" on the right. The toggle should be a simple icon-only button (Sun/Moon).

### Hero Section
The Hero uses `display-xl` typography. It should be left-aligned with a maximum width of 800px. A "Custom Cursor" (a 20px circle with a `difference` blend mode) should be active here, expanding when hovering over the primary CTA.

### Horizontal Sliding Cards (Education)
Education entries are displayed in a non-breaking horizontal row. Each card has a fixed width (e.g., 400px). Use a subtle scroll-snap behavior to ensure cards lock into place.

### Timeline (Experience)
A vertical 2px line in `primary_color`. Each entry has a `primary_color` dot. The layout is asymmetrical: Date/Company on the left, Job Description/Tech Stack on the right.

### Technology Tags (Pills)
Use `mono-label` font. Background is a 10% opacity version of the `primary_color`, with a 1px solid border of the same color. 

### Project Cards with Metrics
The card footer includes a "Metric Bar." Use `metric-num` for data points (e.g., "99.9% Uptime" or "2TB/day"). These metrics should be the highest contrast element in the card.

### Simple Contact Form
Inputs use a "bottom-border only" style to maintain minimalism. On focus, the bottom border transitions from `border_color` to `primary_color` with a 200ms ease. The submit button is a full-width `rounded-xl` element using the `primary_color` fill.