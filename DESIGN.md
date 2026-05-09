---
name: Ember & Oak
colors:
  surface: '#fff9ef'
  surface-dim: '#e2d9c5'
  surface-bright: '#fff9ef'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fcf3de'
  surface-container: '#f6edd8'
  surface-container-high: '#f0e7d3'
  surface-container-highest: '#ebe2cd'
  on-surface: '#1f1b0f'
  on-surface-variant: '#4f453f'
  inverse-surface: '#353022'
  inverse-on-surface: '#f9f0db'
  outline: '#81756e'
  outline-variant: '#d3c4bc'
  surface-tint: '#72594a'
  primary: '#0d0300'
  on-primary: '#ffffff'
  primary-container: '#2c1a0e'
  on-primary-container: '#9d806f'
  inverse-primary: '#e1c0ad'
  secondary: '#934a27'
  on-secondary: '#ffffff'
  secondary-container: '#ffa277'
  on-secondary-container: '#783614'
  tertiary: '#0a0400'
  on-tertiary: '#ffffff'
  tertiary-container: '#2c1b00'
  on-tertiary-container: '#b47b00'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#fedcc8'
  primary-fixed-dim: '#e1c0ad'
  on-primary-fixed: '#29170c'
  on-primary-fixed-variant: '#594234'
  secondary-fixed: '#ffdbcd'
  secondary-fixed-dim: '#ffb595'
  on-secondary-fixed: '#351000'
  on-secondary-fixed-variant: '#753311'
  tertiary-fixed: '#ffddaf'
  tertiary-fixed-dim: '#fdba49'
  on-tertiary-fixed: '#281800'
  on-tertiary-fixed-variant: '#614000'
  background: '#fff9ef'
  on-background: '#1f1b0f'
  surface-variant: '#ebe2cd'
typography:
  headline-xl:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Playfair Display
    fontSize: 24px
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
    lineHeight: '1.6'
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1200px
  gutter: 24px
  margin-edge: 32px
  section-gap: 80px
---

## Brand & Style

The brand identity centers on the intersection of rustic warmth and high-end editorial sophistication. This design system aims to evoke the sensory experience of a specialty café: the aroma of roasted beans, the texture of reclaimed oak, and the quiet comfort of a morning ritual. 

The aesthetic style is a blend of **Minimalism** and **Tactile** design. It prioritizes generous whitespace and a rigid, magazine-like layout structure while employing warm colors and soft shadows to prevent the UI from feeling sterile. Every interaction should feel intentional and serene, targeting a discerning audience that values aesthetics as much as quality.

## Colors

The palette is rooted in organic, earthy tones. The primary color, **Deep Espresso**, serves as the anchor for typography and high-contrast dark sections. **Warm Cream** acts as the canvas, providing a softer, more premium alternative to pure white. 

**Muted Terracotta** provides a sophisticated secondary accent for iconography and decorative elements, while **Soft Amber** is reserved strictly for high-priority calls to action and interactive accents, mimicking the glow of a hearth. When applying colors, maintain a high ratio of cream-to-espresso to ensure the editorial "breathability" of the interface.

## Typography

This design system utilizes a high-contrast typographic pairing to reinforce its editorial character. **Playfair Display** is used for headlines to convey elegance and tradition. For these headlines, tight line-heights and slight negative letter-spacing are encouraged to create a "blocky," authoritative look.

**Inter** provides a functional counterpoint for body text and UI labels, ensuring legibility across digital devices. Label styles should frequently use uppercase transforms with increased letter spacing to create a distinct hierarchy between functional UI elements and storytelling content.

## Layout & Spacing

The layout philosophy follows a **Fixed Grid** model to mirror the structured precision of a printed lookbook. Use a 12-column grid for desktop views with generous gutters to allow content to "breathe." 

Vertical rhythm is based on an 8px scale. To achieve the "Instagram-worthy" aesthetic, the design system mandates aggressive whitespace between sections (80px+), preventing the UI from appearing cluttered. Content should be centered or asymmetrically balanced to create visual interest without sacrificing clarity.

## Elevation & Depth

Visual hierarchy is achieved through **Tonal Layers** and **Ambient Shadows**. Surfaces should not rely on stark black shadows; instead, use low-opacity shadows tinted with the primary Espresso color (e.g., `#2C1A0E` at 8-12% opacity) to maintain warmth.

Interactive cards and modal elements should appear to lift slightly off the Cream background. Use subtle inner glows on buttons to simulate a soft, tactile press. Backdrop blurs are permitted on navigation overlays to suggest a glass-like transition over rich photography.

## Shapes

The shape language is characterized by "softened geometry." Standard components like buttons and input fields use a 12px radius, while larger containers and featured image cards utilize a 16px radius.

This roundedness level balances the sharp, modern lines of the grid with the "cozy" brand promise. Icons should feature rounded caps and corners to match this language. Avoid fully circular "pill" shapes for buttons to maintain the sophisticated, high-end architectural feel of the brand.

## Components

### Buttons
Primary buttons are filled with **Soft Amber** and use **Deep Espresso** text for maximum legibility. Secondary buttons use a **Deep Espresso** border and text. Hover states should involve a subtle shift in saturation or a slight upward translation (2px) accompanied by a softened shadow.

### Cards
Cards are the primary vehicle for product displays (e.g., coffee blends, pastries). They feature a **Warm Cream** surface, 16px corner radius, and a 1px border in a faint Espresso tint (5% opacity). Images within cards should always utilize a subtle zoom effect on hover.

### Input Fields
Inputs use a minimal bottom-border style or a very light cream-filled box with 12px corners. Focus states are indicated by a **Muted Terracotta** border, avoiding the standard "blue" focus rings to maintain the brand’s warm palette.

### Menu & Navigation
The navigation should be sparse and elegant. Use the **Label-MD** typography style for menu items. Active states are indicated by a small, terracotta dot beneath the text rather than an underline, preserving whitespace.

### Interactive Accents
Incorporate "Product Chips" for flavor notes (e.g., "Nutty," "Dark Roast") using a **Warm Cream** fill on an **Espresso** background to provide high-contrast focal points within an otherwise light layout.