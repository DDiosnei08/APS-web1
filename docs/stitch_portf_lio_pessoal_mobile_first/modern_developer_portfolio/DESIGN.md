---
name: Modern Developer Portfolio
colors:
  surface: '#150c34'
  surface-dim: '#150c34'
  surface-bright: '#3b335d'
  surface-container-lowest: '#0f062f'
  surface-container-low: '#1d153d'
  surface-container: '#211941'
  surface-container-high: '#2c244c'
  surface-container-highest: '#372f58'
  on-surface: '#e7deff'
  on-surface-variant: '#ccc3d8'
  inverse-surface: '#e7deff'
  inverse-on-surface: '#322a53'
  outline: '#958da1'
  outline-variant: '#4a4455'
  surface-tint: '#d2bbff'
  primary: '#d2bbff'
  on-primary: '#3f008e'
  primary-container: '#7c3aed'
  on-primary-container: '#ede0ff'
  inverse-primary: '#732ee4'
  secondary: '#d2c5ae'
  on-secondary: '#37301f'
  secondary-container: '#4e4634'
  on-secondary-container: '#c0b49d'
  tertiary: '#ffb784'
  on-tertiary: '#4f2500'
  tertiary-container: '#a15100'
  on-tertiary-container: '#ffe0cd'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#eaddff'
  primary-fixed-dim: '#d2bbff'
  on-primary-fixed: '#25005a'
  on-primary-fixed-variant: '#5a00c6'
  secondary-fixed: '#efe1c9'
  secondary-fixed-dim: '#d2c5ae'
  on-secondary-fixed: '#211b0c'
  on-secondary-fixed-variant: '#4e4634'
  tertiary-fixed: '#ffdcc6'
  tertiary-fixed-dim: '#ffb784'
  on-tertiary-fixed: '#301400'
  on-tertiary-fixed-variant: '#713700'
  background: '#150c34'
  on-background: '#e7deff'
  surface-variant: '#372f58'
  surface-dark: '#1a1629'
  surface-light: '#F8F9FA'
  text-main: '#FFFFFF'
  text-muted: '#B8AC96'
  border-subtle: rgba(184, 172, 150, 0.15)
typography:
  headline-xl:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-xl-mobile:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-lg:
    fontFamily: Geist
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: 0.02em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.4'
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
  margin-mobile: 16px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style

This design system is engineered for the modern software engineer—balancing technical precision with a sophisticated, editorial aesthetic. The brand personality is **authoritative yet approachable**, prioritizing clarity of information and the showcase of craft. 

The visual style follows a **Corporate Modern** approach with **Glassmorphism** accents. It utilizes high-quality typography and a card-based architecture to organize diverse content types (code snippets, project galleries, and technical blogs). The interface relies on subtle depth, precise geometry, and a deliberate use of whitespace to convey a sense of "premium engineering." The emotional response should be one of trust, competence, and obsessive attention to detail.

## Colors

The palette is anchored by a deep, purple-tinted neutral (`#342C55`) that provides more character than a standard grey-scale dark mode. The primary brand color is a **vibrant violet**, used sparingly for interactive elements and key brand moments to maintain a high-signal environment.

The **Sand accent** acts as a sophisticated counterpoint to the cool-toned background, used for secondary text, metadata, and decorative strokes. In light mode, the primary violet remains the anchor, while the background shifts to a clean off-white (`#F8F9FA`), and the deep purple is repurposed for high-contrast typography.

## Typography

This design system employs a dual-font strategy. **Geist** is used for all UI and prose elements to provide a clean, technical, and highly legible experience. Its geometric nature aligns with the developer-centric brand.

**JetBrains Mono** is reserved for labels, metadata, and code blocks. This monospaced font provides a visual "context switch" for the user, signaling technical data or system-level information. Large headlines use tighter letter spacing and heavy weights to create a strong visual hierarchy, while body text maintains a generous line height for long-form readability.

## Layout & Spacing

The layout utilizes a **12-column fixed grid** on desktop, centered within the viewport. Spacing is strictly governed by an **8px base unit**, ensuring mathematical harmony across all components.

- **Desktop:** 1200px max-width, 24px gutters, and 48px-64px section padding.
- **Tablet:** Fluid width with 32px side margins; columns collapse to 6 or 4 depending on content density.
- **Mobile:** Single column layout with 16px horizontal safe areas. 

Vertical rhythm is maintained by using the `stack` variables to define consistent gaps between related elements (e.g., 8px between a label and input, 16px between a headline and body text).

## Elevation & Depth

Visual hierarchy is achieved through **tonal layers** and **ambient shadows**. In dark mode, surfaces that are closer to the user are rendered in slightly lighter shades of the neutral purple base. 

The design system avoids heavy, pitch-black shadows. Instead, it uses **low-opacity tinted shadows** (using the primary purple hue) to create a subtle glow effect around floating cards. Interactive elements like buttons use a "soft lift" on hover—transitioning from a flat state to a slight shadow-induced elevation. Glassmorphism is applied to navigation bars and floating overlays, using a backdrop blur (12px) and a 1px semi-transparent sand border to maintain edge definition against complex backgrounds.

## Shapes

The shape language is defined by **rounded containers** that soften the technicality of the typography. A standard **8px (0.5rem) corner radius** is applied to primary UI components like buttons, input fields, and small cards. 

Large containers and feature sections use `rounded-lg` (16px) to create a clear nested relationship with internal elements. Decorative elements, such as tag chips or avatars, may utilize a pill-shape (full radius) to provide visual variety and distinguish them from structural components.

## Components

### Buttons
- **Primary:** Solid `#7c3aed` background with white text. High-contrast, 8px radius.
- **Secondary:** Transparent background with a 1px `#B8AC96` border (Ghost style). 
- **Active State:** A subtle scale-down (0.98) and increased shadow spread.

### Cards
Cards are the primary container for portfolio projects. They should feature a 1px border (`border-subtle`) and a background color one step lighter than the page background. Hovering over a card should trigger a transition to a more prominent sand-tinted border.

### Chips & Tags
Used for tech stacks (e.g., "React", "TypeScript"). Use `label-sm` typography in a pill-shaped container with a low-opacity primary purple background.

### Input Fields
Inputs use the `surface-dark` background with a subtle inset shadow to indicate "emptiness." The focus state must clearly highlight the field with a 2px primary purple border and a soft outer glow.

### Code Snippets
Code blocks should use a custom dark theme that highlights the Accent Sand and Primary Purple hues, housed in a card with a "Copy" utility button in the top right corner.