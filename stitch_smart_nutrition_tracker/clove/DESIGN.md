---
name: Clove Modern Culinary
colors:
  surface: '#fbf9f9'
  surface-dim: '#dbdad9'
  surface-bright: '#fbf9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f3f3'
  surface-container: '#efeded'
  surface-container-high: '#e9e8e7'
  surface-container-highest: '#e3e2e2'
  on-surface: '#1b1c1c'
  on-surface-variant: '#414942'
  inverse-surface: '#303031'
  inverse-on-surface: '#f2f0f0'
  outline: '#717971'
  outline-variant: '#c1c9bf'
  surface-tint: '#43664d'
  primary: '#00230f'
  on-primary: '#ffffff'
  primary-container: '#063a1f'
  on-primary-container: '#7ea386'
  inverse-primary: '#a9d0b1'
  secondary: '#556158'
  on-secondary: '#ffffff'
  secondary-container: '#d9e6da'
  on-secondary-container: '#5b675e'
  tertiary: '#1f1b24'
  on-tertiary: '#ffffff'
  tertiary-container: '#35303a'
  on-tertiary-container: '#9f97a3'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#bbefc7'
  primary-fixed-dim: '#a9d0b1'
  on-primary-fixed: '#00210e'
  on-primary-fixed-variant: '#2c4e36'
  secondary-fixed: '#d9e6da'
  secondary-fixed-dim: '#bdcabf'
  on-secondary-fixed: '#131e17'
  on-secondary-fixed-variant: '#3e4a41'
  tertiary-fixed: '#e8dfec'
  tertiary-fixed-dim: '#ccc4d0'
  on-tertiary-fixed: '#1e1a23'
  on-tertiary-fixed-variant: '#4a454f'
  background: '#fbf9f9'
  on-background: '#1b1c1c'
  surface-variant: '#e3e2e2'
typography:
  headline-xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '700'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  body-sm:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
  label-md:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.01em
  caption-xs:
    fontFamily: Manrope
    fontSize: 10px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  gutter: 16px
  container-padding: 20px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 40px
---

## Brand & Style

Clove is a premium culinary lifestyle brand that blends modern wellness with editorial sophistication. The design style is **Editorial Minimalism**—it prioritizes high-fidelity food photography and generous white space to create a calm, aspirational user experience. 

The aesthetic is inspired by high-end boutique cookbooks: clean, structured, and trustworthy. It uses subtle tonal layering and soft shadows to provide depth without clutter, ensuring the vibrant colors of fresh ingredients remain the focal point. The interface should feel like a breathable digital magazine—inviting, organized, and effortlessly professional.

## Colors

The palette is anchored by "Deep Forest Green" (#00230f), evoking freshness and culinary expertise. This is supported by a range of sophisticated neutrals that lean slightly warm (off-whites and soft greys) to maintain an organic, approachable feel.

- **Primary:** Used for brand identity, core actions, and high-level headings.
- **Surface Tones:** A tiered system of off-whites (FBF9F9 to F5F3F3) provides subtle containment for UI elements without the harshness of pure white.
- **Accents:** High-chroma photography provides the "pop," while UI accents like `primary-fixed` (#BBEFC7) are used for subtle highlights and container backgrounds.

## Typography

The system uses a pairing of **Plus Jakarta Sans** for headlines to provide a modern, welcoming personality, and **Manrope** for body and label text to ensure high legibility and a refined technical feel.

Headlines use tight letter spacing and heavy weights (Bold/Extrabold) to command attention. Body text is optimized for readability with generous line heights. Labels often utilize "Semi-Bold" or "Bold" weights even at small sizes to maintain hierarchy within dense information layouts.

## Layout & Spacing

The system follows a **Fixed Grid** philosophy for desktop (max-width: 1280px) and a **Fluid Fluid** approach for mobile. 

- **Vertical Rhythm:** A stack-based spacing scale is used to separate sections. Use `stack-lg` (40px) between major content sections and `stack-sm` (12px) for internal component spacing.
- **Safe Areas:** Mobile views utilize a 20px horizontal container margin. 
- **Horizontal Scroll:** Multi-card sections (like Meal Plans) should bleed into the container padding and use a "peek" affordance to indicate further content.

## Elevation & Depth

Hierarchy is established through **Ambient Shadows** and **Tonal Layering**:

- **Soft Elevation:** Primary cards use a very subtle, diffused shadow (`0 4px 20px 0 rgba(0, 0, 0, 0.04)`) to lift them off the background without appearing heavy.
- **Glassmorphism:** Navigation bars (top and bottom) use an 80-90% opacity surface color with a `backdrop-blur-md` effect. This maintains a sense of place as the user scrolls.
- **Contrast Depth:** Interaction states (like the floating feedback button or FAB) use higher-intensity shadows (`shadow-lg`) to denote immediate accessibility.

## Shapes

The shape language is **Rounded and Organic**, reflecting the natural forms of food and ingredients.

- **Standard Containers:** Cards and major sections use a 1.5rem (`rounded-3xl`) or 1rem (`rounded-2xl`) corner radius.
- **Interactive Elements:** Input fields and buttons use 0.75rem (`rounded-xl`).
- **Circular Elements:** Profile avatars, icons buttons, and the Floating Action Button (FAB) are always fully rounded (`rounded-full`).

## Components

- **Cards:** Use a "Bento" style for collections, grouping multiple images in a grid with a single caption area. Images within cards should have a `rounded-xl` radius and use `object-cover`.
- **Buttons:**
    - **Primary FAB:** Large, circular, high-contrast (Primary background, White icon).
    - **Ghost/Icon Buttons:** Circular with a `surface-container` hover state.
- **Inputs:** Search bars should be borderless, using `surface-container-low` as a background and `rounded-xl` corners for a soft, integrated look.
- **Chips/Badges:** Small, high-contrast labels (e.g., "6 MEALS") use a `backdrop-blur` background when placed over images, with uppercase bold text for maximum visibility.
- **Navigation:** The bottom bar uses a fixed-height layout with a central "bulge" for the Primary FAB, creating a distinct visual anchor.