---
name: VIP Glamour
colors:
  surface: '#151316'
  surface-dim: '#151316'
  surface-bright: '#3b383c'
  surface-container-lowest: '#0f0d10'
  surface-container-low: '#1d1b1e'
  surface-container: '#211f22'
  surface-container-high: '#2c292c'
  surface-container-highest: '#373437'
  on-surface: '#e7e1e5'
  on-surface-variant: '#d1c5ac'
  inverse-surface: '#e7e1e5'
  inverse-on-surface: '#322f33'
  outline: '#9a9078'
  outline-variant: '#4e4633'
  surface-tint: '#f0c110'
  primary: '#ffe5a0'
  on-primary: '#3d2f00'
  primary-container: '#f5c518'
  on-primary-container: '#695200'
  inverse-primary: '#745b00'
  secondary: '#ffb1c3'
  on-secondary: '#66002c'
  secondary-container: '#ff4b89'
  on-secondary-container: '#590026'
  tertiary: '#f2e1ff'
  on-tertiary: '#470083'
  tertiary-container: '#debeff'
  on-tertiary-container: '#7623c7'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffe08b'
  primary-fixed-dim: '#f0c110'
  on-primary-fixed: '#241a00'
  on-primary-fixed-variant: '#584400'
  secondary-fixed: '#ffd9e0'
  secondary-fixed-dim: '#ffb1c3'
  on-secondary-fixed: '#3f0019'
  on-secondary-fixed-variant: '#8f0041'
  tertiary-fixed: '#efdbff'
  tertiary-fixed-dim: '#dbb8ff'
  on-tertiary-fixed: '#2b0052'
  on-tertiary-fixed-variant: '#6600b7'
  background: '#151316'
  on-background: '#e7e1e5'
  surface-variant: '#373437'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 56px
    fontWeight: '700'
    lineHeight: 64px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 38px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 26px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 22px
    fontWeight: '600'
    lineHeight: 28px
  title-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '700'
    lineHeight: 24px
    letterSpacing: 0.01em
  title-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 22px
  body-lg:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: Manrope
    fontSize: 13px
    fontWeight: '700'
    lineHeight: 18px
    letterSpacing: 0.08em
  label-md:
    fontFamily: Manrope
    fontSize: 11px
    fontWeight: '800'
    lineHeight: 14px
    letterSpacing: 0.1em
  label-sm:
    fontFamily: Manrope
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-mobile: 0.75rem
  gutter-desktop: 1.5rem
  margin: 1.25rem
  margin-mobile: 1rem
  margin-desktop: 3rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2.5rem
---

## Brand & Style

The design system embodies an unapologetic, high-octane luxury aesthetic: high-fashion editorial polish merged with viral social-media celebrity bravado. It treats VIP status, influencer allure, and conspicuous luxury not as subtle undertones, but as front-row spectacles. 

The visual language draws inspiration from high-jewelry spreads, exclusive backstage passes, and luminous mobile-first content drops. It delivers sensory impact through pitch-black obsidian canvases, ultra-refined serif headlines, high-saturation magenta bursts, and champagne gold metallic trims. The interface evokes exclusivity, hype, and celebratory indulgence—engineered for high-conversion lifestyle feeds, live drops, and aspirational curation.

## Colors

The palette operates in strict dark mode, anchored by deep, obsidian-violet background tiers that allow chromatic accents to radiate:

- **Surface Grounds:**
  - Base canvas (`#0D0B0E`): Deepest velvety black-purple, grounding the entire interface.
  - Surface Container Low (`#18141B`): Secondary surfaces, list rows, and structural divisions.
  - Surface Container High (`#221C27`): Interactive cards, elevated panels, and sheet backgrounds.
  - Surface Rim (`#32283A`): Subtle boundary definition for elevated layers.

- **Precious Metals & Accents:**
  - Primary (`#F5C518`): Champagne 24k gold, reserved for primary achievements, VIP badges, verified seals, and monetary triggers.
  - Secondary (`#FF007A` / `#FF2E93`): Magenta Glam and electric pink, applied to live badges, viral action items, and assertive call-to-actions.
  - Tertiary (`#7928CA`): Deep amethyst, balancing high-contrast glows and providing ambient gradient bridges between obsidian and magenta.
  - High-Contrast Text (`#FFFFFF`): Crisp pure white for maximum legibility on dark luxury surfaces.
  - Subdued Text (`#A39BA8`): Lavender-tinted muted gray for secondary labels and metadata.

## Typography

Typography establishes an intentional contrast between aristocratic editorial elegance and modern social ergonomics. 

- **Playfair Display:** Employed exclusively for large-scale editorial statements, drop titles, numbers, prices, and hero banners. High stroke contrast reinforces an haute-couture atmosphere.
- **Manrope:** Serves as the functional counterweight. Its geometric precision and wide aperture provide razor-sharp clarity for high-density mobile interfaces, fast-scrolling feeds, micro-labels, and interactive controls.
- **Letter Spacing:** All uppercase micro-labels (`label-lg`, `label-md`) strictly utilize expanded tracking (`0.08em` to `0.1em`) to mimic luxury fragrance and jewelry packaging.

## Layout & Spacing

The layout model adapts across three primary device viewports:

- **Mobile (< 768px):** 4-column fluid layout with `1rem` margins and `0.75rem` gutters. Content runs edge-to-edge with generous vertical breathing room (`space-lg`) between content capsules.
- **Tablet (768px - 1024px):** 8-column fluid layout with `1.5rem` margins and `1rem` gutters.
- **Desktop (> 1024px):** 12-column fixed-max layout (capped at `1280px`) with `3rem` outer margins and `1.5rem` gutters, centering content with theatrical presentation borders.

Vertical cadence follows strict multiples of `0.25rem` (4px base unit). Dense interactive modules rely on `space-sm` (8px) internal gaps, while editorial sections maintain luxury presence using `space-xl` (40px) thematic separation.

## Elevation & Depth

Visual hierarchy abandons flat gray drop shadows in favor of tinted luminescence and luminous containment:

- **Surface Tiers:** Layering relies primarily on tonal shifts between `#0D0B0E`, `#18141B`, and `#221C27`.
- **Gold Ambient Glow:** High-priority cards, VIP status items, and floating checkout controls project a dual ambient aura: `0 8px 32px -4px rgba(245, 197, 24, 0.18)` paired with an inner top hairline reflection `inset 0 1px 0 0 rgba(255, 215, 0, 0.35)`.
- **Glam Neon Cast:** Live drops, flash notifications, and urgent engagement triggers project a vibrant magenta aura: `0 8px 28px -2px rgba(255, 0, 122, 0.28)`.
- **Structural Outlines:** Inactive containers avoid drop shadows entirely, maintaining crisp structural clarity through hairline borders (`1px solid rgba(255, 255, 255, 0.08)` or `1px solid rgba(245, 197, 24, 0.2)`).

## Shapes

The interface balances sharp editorial discipline with tactile luxury. A base level of `2` (`0.5rem` / `8px`) governs standard inputs, badges, and thumbnail frames.

- **Standard Containers:** Cards, modals, and dropdown overlays use `rounded-lg` (`1rem` / `16px`) to soften visual bulk while maintaining premium architecture.
- **Hero Drawers & Bottom Sheets:** Employ `rounded-xl` (`1.5rem` / `24px`) on top edges to produce a pillowed, lounge-like feel.
- **Interactive Badges & Chips:** Systematically use fully rounded pill profiles (`9999px`) to create tactile, gem-like interactive touchpoints.

## Components

### Buttons
- **Primary Glam Action:** Background utilizes a directional linear gradient (`135deg, #FF007A 0%, #F5C518 100%`) with pure white bold text (`Manrope 700`), subtle text shadow, and `0.5rem` border radius. On hover/active, the button expands its outer golden-magenta bloom.
- **Secondary VIP Gold:** Dark background (`#18141B`) bordered by a `1px` gradient of `#F5C518` to `#E5A93C`, with metallic gold typography and a top inner highlight line.
- **Tertiary Ghost:** Transparent background with high-contrast white text, shifting to a translucent magenta sheen (`rgba(255, 0, 122, 0.1)`) upon hover.

### Chips & Tags
- **VIP Status Chips:** Pill-shaped (`rounded-full`), padded with `0.25rem 0.75rem`. Outlined with a metallic champagne stroke (`rgba(245, 197, 24, 0.4)`), featuring gold tracking typography (`label-md`) and an optional sparkling star icon prefix.
- **Live / Trending Badges:** Magenta background (`#FF007A`) with white bold text, pulsing with a synchronized ambient glow.

### Cards
- **Editorial Showcases:** Background set to `#221C27` with a fine perimeter stroke (`1px solid rgba(245, 197, 24, 0.2)`). Images inside cards occupy edge-to-edge upper positioning with a dark gradient scrim at the bottom to guarantee readability for `Playfair Display` titles.
- **Interactive Focus:** Elevates by `2px` with the border brightening to solid `#F5C518` and cast shadows deepening.

### Inputs & Form Fields
- **Text Inputs:** Dark base (`#18141B`), border `1px solid rgba(255, 255, 255, 0.12)`, height `48px`, `rounded-md` (`0.5rem`). Text renders in pure white with placeholder in muted `#A39BA8`.
- **Focus State:** Border shifts instantaneously to `#FF007A` backed by an outer blur of `0 0 0 3px rgba(255, 0, 122, 0.2)`.

### Checkboxes & Radios
- **Controls:** Size `20px x 20px`, dark base with a refined champagne border (`#F5C518`). When checked, fills with the magenta-to-gold gradient, displaying a crisp white micro checkmark.

### Modals & VIP Bottom Sheets
- **Surfaces:** Floating obsidian panels (`#18141B`) crowned with a `2px` top border gradient (`#F5C518` to `#FF007A`). Backdrop utilizes frosted obsidian glass (`backdrop-filter: blur(16px)` over `rgba(13, 11, 14, 0.85)`).