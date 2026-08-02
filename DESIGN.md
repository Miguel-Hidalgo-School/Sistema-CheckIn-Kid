---
name: Academic Pillar
colors:
  surface: '#fff8f2'
  surface-dim: '#e0d9d0'
  surface-bright: '#fff8f2'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#faf2e9'
  surface-container: '#f4ede4'
  surface-container-high: '#efe7de'
  surface-container-highest: '#e9e1d9'
  on-surface: '#1e1b16'
  on-surface-variant: '#504441'
  inverse-surface: '#33302a'
  inverse-on-surface: '#f7f0e7'
  outline: '#827470'
  outline-variant: '#d3c3be'
  surface-tint: '#74584e'
  primary: '#231009'
  on-primary: '#ffffff'
  primary-container: '#3a241c'
  on-primary-container: '#aa897e'
  inverse-primary: '#e3bfb2'
  secondary: '#a53c08'
  on-secondary: '#ffffff'
  secondary-container: '#ff7e49'
  on-secondary-container: '#692100'
  tertiary: '#1e1300'
  on-tertiary: '#ffffff'
  tertiary-container: '#382600'
  on-tertiary-container: '#bb8708'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbcf'
  primary-fixed-dim: '#e3bfb2'
  on-primary-fixed: '#2a160f'
  on-primary-fixed-variant: '#5a4138'
  secondary-fixed: '#ffdbce'
  secondary-fixed-dim: '#ffb599'
  on-secondary-fixed: '#370e00'
  on-secondary-fixed-variant: '#802a00'
  tertiary-fixed: '#ffdea7'
  tertiary-fixed-dim: '#f8bd45'
  on-tertiary-fixed: '#271900'
  on-tertiary-fixed-variant: '#5e4200'
  background: '#fff8f2'
  on-background: '#1e1b16'
  surface-variant: '#e9e1d9'
  surface-white: '#FFFFFF'
  text-high-contrast: '#1A100C'
  status-safe: '#2D5A27'
  status-warning: '#F4B942'
typography:
  display-lg:
    fontFamily: Fraunces
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Fraunces
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Fraunces
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
  headline-md:
    fontFamily: Fraunces
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
  label-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.04em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-margin: 24px
  gutter: 16px
  section-gap: 40px
  mobile-margin: 16px
---

## Brand & Style

The design system is engineered for a school management environment where reliability, safety, and clarity are paramount. The brand personality is **authoritative yet accessible**, bridging the gap between institutional security and the warmth of a community-focused educational setting.

The chosen style is **Corporate Modern with a Minimalist focus**. It utilizes generous whitespace to reduce cognitive load for administrators and parents, while employing structured layouts that suggest order and efficiency. Visual interest is generated through precise typography and a sophisticated use of brand accents against a clean, neutral backdrop, avoiding unnecessary decorative elements that could distract from critical student data.

## Colors

The color palette is anchored by a deep, scholarly brown (`#3A241C`) which provides a grounded alternative to standard navy or black, evoking a sense of heritage and stability. 

- **Primary:** The dark chocolate tone is used for core branding, primary headers, and high-importance navigation to establish authority.
- **Secondary & Tertiary:** The sunset orange and amber tones are used sparingly for actionable elements (buttons, notifications) to ensure they stand out against the neutral backgrounds.
- **Neutral:** The parchment-inspired cream (`#FFF7EE`) is the primary background color, providing a softer, more professional reading experience than pure white, though pure white is reserved for content cards to create subtle depth.

## Typography

This design system uses a sophisticated pairing of **Fraunces** for editorial impact and **Inter** for functional clarity.

- **Fraunces** (Serif): Reserved for headlines and "Check-in" titles. It provides a literary, academic feel that differentiates the app from generic SaaS products.
- **Inter** (Sans-Serif): Used for all body text, data tables, and input labels. It is highly legible at small sizes, which is critical for mobile management tasks and schedule viewing.
- **Contrast:** All text intended for reading is set to the `text-high-contrast` token to meet accessibility standards against the parchment background.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy on desktop to maintain a structured "dashboard" feel, while transitioning to a fluid single-column layout on mobile.

- **Desktop:** 12-column grid with a max-width of 1280px. Content is organized into modular cards.
- **Mobile:** Single column with 16px side margins. Emphasis is placed on vertical stacking for easy one-handed scrolling during student drop-off/pick-up.
- **Spacing Rhythm:** An 8px base unit governs all padding and margins. Vertical rhythm should be consistent, using `section-gap` between major functional blocks (e.g., student list vs. attendance summary).

## Elevation & Depth

To maintain a professional and clean aesthetic, depth is communicated through **Tonal Layers** and **Low-Contrast Outlines** rather than heavy shadows.

- **Surface Tiers:** The main background is the Neutral Parchment. Interaction areas (cards, lists) are Pure White. This subtle shift provides enough separation without visual clutter.
- **Borders:** Use 1px solid borders in a slightly darker version of the neutral tone (`#E5DED5`) to define data cells and input fields.
- **Active State:** A soft, diffused shadow (10% opacity of the primary brown) may be used on "Active" or "Selected" cards to provide a tactile sense of focus.

## Shapes

The design system uses **Rounded (level 2)** corners (8px base) to strike a balance between professional rigor and student-friendly approachability.

- **Standard Elements:** Buttons, input fields, and cards utilize the 8px radius.
- **Large Components:** Hero sections or large modal containers may use the `rounded-lg` (16px) token to soften the overall UI.
- **Interactive Triggers:** Small utility buttons (e.g., "Add Student") should maintain consistent rounding to signify clickability.

## Components

- **Buttons:** Primary buttons use the secondary orange (`#F0733F`) with white text for maximum visibility. Secondary buttons use an outline of the primary brown.
- **Chips:** Used for student status (e.g., "Checked In", "Late"). These should have a background tint of the status color with high-contrast text.
- **Input Fields:** Use a white background with a 1px border. Labels must always be visible (no floating labels that disappear) to ensure clarity for busy staff.
- **Cards:** The primary container for student profiles. Cards feature a white background and a subtle 8px corner radius. On mobile, cards should be full-width with a bottom border for separation.
- **Lists:** Attendance lists should use alternating row tints or clear dividers to assist in horizontal scanning of data points like time-stamps and guardian names.