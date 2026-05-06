---
name: The Portfolio System
colors:
  surface: '#f9f9f7'
  surface-dim: '#dadad8'
  surface-bright: '#f9f9f7'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f4f2'
  surface-container: '#eeeeec'
  surface-container-high: '#e8e8e6'
  surface-container-highest: '#e2e3e1'
  on-surface: '#1a1c1b'
  on-surface-variant: '#444748'
  inverse-surface: '#2f3130'
  inverse-on-surface: '#f1f1ef'
  outline: '#747878'
  outline-variant: '#c4c7c7'
  surface-tint: '#5f5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1c1b1b'
  on-primary-container: '#858383'
  inverse-primary: '#c8c6c5'
  secondary: '#546257'
  on-secondary: '#ffffff'
  secondary-container: '#d7e7d8'
  on-secondary-container: '#5a685c'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#1a1c19'
  on-tertiary-container: '#838480'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c8c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474746'
  secondary-fixed: '#d7e7d8'
  secondary-fixed-dim: '#bbcabd'
  on-secondary-fixed: '#121e16'
  on-secondary-fixed-variant: '#3c4a3f'
  tertiary-fixed: '#e3e3de'
  tertiary-fixed-dim: '#c6c7c2'
  on-tertiary-fixed: '#1a1c19'
  on-tertiary-fixed-variant: '#464744'
  background: '#f9f9f7'
  on-background: '#1a1c1b'
  surface-variant: '#e2e3e1'
typography:
  display-xl:
    fontFamily: Noto Serif
    fontSize: 80px
    fontWeight: '400'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Noto Serif
    fontSize: 48px
    fontWeight: '400'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Noto Serif
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0.01em
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 32px
  margin-edge: 64px
  section-gap: 160px
---

## Brand & Style

This design system is built on the philosophy of "The Quiet Curator." It prioritizes the content—whether photography, architectural renderings, or case studies—by providing a serene, architectural frame. The brand personality is intentional, sophisticated, and understated, evoking the emotional response of walking into a high-end, contemporary art gallery.

The design style is a pure execution of **Minimalism**. It relies on generous whitespace (negative space as a functional element), high-quality typography, and a restrained color palette. Every element exists for a reason; there is no decoration for the sake of decoration. Transitions are intentional and slow, favoring "fade-and-slide" motions over aggressive spring animations to maintain a sense of calm.

## Colors

The palette is designed to feel organic yet professional. The foundation is **Soft White** (#FDFDFB), which provides a warmer, more premium feel than a clinical pure white. **Deep Charcoal** (#1A1A1A) serves as the primary color for typography and structural elements, offering high contrast without the harshness of pure black.

A sophisticated **Sage Green** (#94A396) is used as the sole accent color. It should be applied sparingly—to call attention to primary actions, signify active states, or highlight subtle brand moments. A tertiary **Stone Gray** (#E8E8E3) is utilized for borders and secondary backgrounds to create soft separation without breaking the minimalist flow.

## Typography

The typographic system relies on a high-contrast pairing that balances classical elegance with modern utility. 

**Noto Serif** is the voice of the system, used for headlines and display text. Its refined serifs and varying stroke widths convey a sense of history and editorial quality. It should be set with generous leading to allow the letterforms to breathe.

**Manrope** provides a functional, balanced counterpoint for body copy and metadata. As a modern sans-serif, it maintains exceptional readability at smaller sizes. Labels and small navigational elements should be set in Manrope with increased letter spacing and uppercase styling to create a clear visual hierarchy against the more fluid serif headlines.

## Layout & Spacing

The layout follows a **Fixed Grid** model centered within the viewport. A 12-column system is utilized for content organization, but the defining characteristic is the "internal margin." Large-scale sections are separated by significant vertical gaps (160px+) to ensure each piece of content is viewed in isolation.

Spacing follows an 8px rhythmic scale. However, for layout purposes, priority is given to asymmetric compositions—for example, a headline spanning 5 columns with a 1-column offset, leaving the remaining space empty. This creates the "gallery" feel where the void is as important as the content.

## Elevation & Depth

Depth in this design system is subtle and atmospheric. We avoid heavy dropshadows in favor of **Tonal Layers** and **Ambient Shadows**. 

Surfaces that require elevation (like cards or floating navigation) use a two-part shadow: a very soft, high-blur ambient occlusion shadow (15% opacity of the Sage Green mixed with Charcoal) and a subtle 1px border in the tertiary Stone Gray. This makes elements appear to lift slightly off the page rather than hover aggressively. 

Interactions should utilize background blurs (12px to 20px) on navigation bars and overlays to maintain a sense of spatial context, allowing the colors of the underlying portfolio imagery to bleed through softly.

## Shapes

The shape language is **Soft** and architectural. While the layout is driven by a rigid grid, the corners of UI elements are slightly eased with a 0.25rem (4px) radius. This prevents the design from feeling overly sharp or clinical, adding a touch of "tactile paper" quality to the digital interface.

Buttons and input fields maintain this consistent radius. Imagery should remain sharp (0px) to feel like professional prints, unless they are used as interactive tiles, in which case they adopt the system's standard soft radius.

## Components

### Buttons
Primary buttons are solid Deep Charcoal with Soft White text. Secondary buttons are "Ghost" style—a Sage Green border with a subtle background tint on hover. All button transitions must be timed at 300ms with a linear-out-slow-in easing profile.

### Cards
Portfolio cards are the centerpiece. They should be borderless by default, using the Soft White background. On hover, the image should scale slightly (1.05x) within its container, and the caption (set in Noto Serif) should shift upwards by 8px.

### Inputs
Text inputs are minimalist: a single 1px bottom border in Stone Gray that transitions to Sage Green on focus. Labels should always be visible, using the uppercase Label-SM typography.

### Navigation
The main navigation should be "sticky" but minimalist, using a Backdrop Blur effect. Use Manrope for nav links, ensuring they have a generous 32px horizontal padding to maintain the open, airy aesthetic of the design system.

### Gallery Lightbox
When viewing assets, the background should transition to a Deep Charcoal at 98% opacity, completely removing distractions and shifting the focus entirely to the work.