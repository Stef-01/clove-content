---
name: Clove Refined
colors:
  surface: '#fafaf4'
  surface-dim: '#dadad5'
  surface-bright: '#fafaf4'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f4ee'
  surface-container: '#eeeee9'
  surface-container-high: '#e8e8e3'
  surface-container-highest: '#e3e3de'
  on-surface: '#1a1c19'
  on-surface-variant: '#424844'
  inverse-surface: '#2f312e'
  inverse-on-surface: '#f1f1ec'
  outline: '#727974'
  outline-variant: '#c1c8c3'
  surface-tint: '#476558'
  primary: '#163328'
  on-primary: '#ffffff'
  primary-container: '#2d4a3e'
  on-primary-container: '#99b9a9'
  inverse-primary: '#adcebe'
  secondary: '#4a654e'
  on-secondary: '#ffffff'
  secondary-container: '#c9e8cb'
  on-secondary-container: '#4e6952'
  tertiary: '#2c2f2c'
  on-tertiary: '#ffffff'
  tertiary-container: '#424542'
  on-tertiary-container: '#b0b2af'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#c9ead9'
  primary-fixed-dim: '#adcebe'
  on-primary-fixed: '#022016'
  on-primary-fixed-variant: '#304d40'
  secondary-fixed: '#cceace'
  secondary-fixed-dim: '#b0ceb2'
  on-secondary-fixed: '#07200f'
  on-secondary-fixed-variant: '#334d38'
  tertiary-fixed: '#e1e3df'
  tertiary-fixed-dim: '#c5c7c3'
  on-tertiary-fixed: '#191c1a'
  on-tertiary-fixed-variant: '#444845'
  background: '#fafaf4'
  on-background: '#1a1c19'
  surface-variant: '#e3e3de'
typography:
  headline-lg:
    fontFamily: Manrope
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  insight-title:
    fontFamily: Manrope
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Source Serif 4
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 30px
  body-md:
    fontFamily: Source Serif 4
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 26px
  label-caps:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-padding-desktop: 40px
  container-padding-mobile: 20px
  stack-gap-lg: 32px
  stack-gap-md: 16px
  insight-padding: 24px
---

## Brand & Style

The design system is engineered for a coaching-focused interface that bridges the gap between clinical authority and personal growth. The brand personality is empathetic, intentional, and grounded, aiming to evoke a sense of calm clarity and professional support. 

The aesthetic is a hybrid of **Minimalism** and **Tactile Modernism**. It prioritizes heavy white space and a restricted palette to reduce cognitive load, while using subtle physical metaphors—like soft depth and organic "coach-surface" layers—to make expert feedback feel tangible and approachable. The goal is to move away from cold, analytical data visualization toward a "human-in-the-loop" experience where system data feels automated but coaching feels curated.

## Colors

The palette is rooted in a sophisticated "Evergreen" spectrum. The **Primary Color** (#2D4A3E) is a deep, authoritative forest green used for navigation and key actions. The **Secondary Color** (#8BA88E) acts as a bridge for supportive UI elements.

A specialized **Coach-Surface** color (#E9EDDE) is introduced as a functional "warm sage" background. This specific token must be used exclusively for areas containing expert feedback, clinical insights, or direct coach communication. This visual distinction ensures that users can instantly differentiate between system-generated metrics (on white or neutral-tertiary surfaces) and human-vetted guidance.

## Typography

Typography in this design system follows a dual-path strategy to balance technical precision with long-form readability. 

- **Manrope** is used for headlines and UI navigation, providing a modern, balanced, and professional structure.
- **Source Serif 4** is the primary typeface for body content and insights. Its literary, authoritative, and warm characteristics are optimized for reading clinical reports and lengthy coach feedback without eye strain.
- **Hanken Grotesk** handles functional labels and metadata, offering a sharp, contemporary feel for data points.

Line heights are intentionally generous (1.6x for body text) to ensure that dense information remains digestible and non-threatening.

## Layout & Spacing

The layout utilizes a **Fixed Grid** on desktop (1200px max width) and a **Fluid Grid** on mobile. The spacing rhythm is based on an 8px base unit.

- **Desktop:** 12-column grid with 32px gutters. Insights cards typically span 6 to 8 columns to maintain an optimal line length for the serif body text (approx. 60-75 characters).
- **Mobile:** 4-column grid with 16px gutters and 20px side margins. 

Large vertical gaps (stack-gap-lg) are used to separate system data blocks from coaching blocks, creating a clear "breathing room" between automated stats and human advice.

## Elevation & Depth

This design system uses **Tonal Layers** combined with **Ambient Shadows** to create a soft, non-intimidating hierarchy.

- **Level 0 (Base):** Neutral white or Tertiary Light Grey (#F2F4F0).
- **Level 1 (Cards):** Standard cards use a subtle 1px border (#E0E0E0) with no shadow to maintain a flat, clean look.
- **Level 2 (Insight Cards):** These use the "Coach-Surface" background with a deep, ultra-diffused shadow (Color: Primary with 5% opacity, Y: 8, Blur: 24) to make them feel elevated and significant.
- **Level 3 (Interactive/Pop-overs):** Crisp shadows with a tighter blur to indicate immediate proximity and focus.

## Shapes

The shape language is consistently **Rounded**, reflecting the approachable and organic nature of coaching. 

Standard components (buttons, inputs) utilize a 0.5rem (8px) radius. Larger containers, specifically **Insight Cards**, should utilize the `rounded-xl` (1.5rem / 24px) setting to appear softer and more like a contained "thought" or "module." Avatars for coaches must be perfectly circular to contrast against the architectural geometry of the UI.

## Components

### Insight Cards
The flagship component of the design system. 
- **Surface:** Uses the `coach_surface_hex` background.
- **Avatar:** 48px circular coach portrait positioned at the top-left or top-right.
- **Clinical Badge:** A small, pill-shaped label using the primary color with white text (using `label-caps` typography), anchored to the avatar or card header to signify "Verified Expert."
- **Content:** Headline in `insight-title` and body in `body-md` (Source Serif 4).

### Buttons
- **Primary:** Solid `primary_color_hex` with white text. High contrast, 8px radius.
- **Supportive:** Ghost style with a 1.5px border of the primary color, used for secondary actions within coach surfaces.

### Lists & Inputs
- **Lists:** Use subtle dividers (1px, Tertiary color) with 16px vertical padding. 
- **Inputs:** Soft-filled backgrounds (#F9F9F9) that transition to a 2px primary-colored border on focus.

### Feedback Chips
Small, rounded-pill indicators used within insights to highlight "Key Takeaways." These should use a slightly darker tint of the coach-surface to remain harmonious but legible.