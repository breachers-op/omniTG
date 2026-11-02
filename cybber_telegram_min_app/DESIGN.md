---
name: Cyber Telegram Mini App
colors:
  surface: '#10131a'
  surface-dim: '#10131a'
  surface-bright: '#363940'
  surface-container-lowest: '#0b0e14'
  surface-container-low: '#191c22'
  surface-container: '#1d2026'
  surface-container-high: '#272a31'
  surface-container-highest: '#32353c'
  on-surface: '#e1e2eb'
  on-surface-variant: '#bec8d1'
  inverse-surface: '#e1e2eb'
  inverse-on-surface: '#2e3037'
  outline: '#88929b'
  outline-variant: '#3e4850'
  surface-tint: '#86cfff'
  primary: '#86cfff'
  on-primary: '#00344c'
  primary-container: '#24a1de'
  on-primary-container: '#00344c'
  inverse-primary: '#00658f'
  secondary: '#d0bcff'
  on-secondary: '#3c0091'
  secondary-container: '#571bc1'
  on-secondary-container: '#c4abff'
  tertiary: '#4cd7f6'
  on-tertiary: '#003640'
  tertiary-container: '#00a6c2'
  on-tertiary-container: '#003540'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c8e6ff'
  primary-fixed-dim: '#86cfff'
  on-primary-fixed: '#001e2e'
  on-primary-fixed-variant: '#004c6d'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d0bcff'
  on-secondary-fixed: '#23005c'
  on-secondary-fixed-variant: '#5516be'
  tertiary-fixed: '#acedff'
  tertiary-fixed-dim: '#4cd7f6'
  on-tertiary-fixed: '#001f26'
  on-tertiary-fixed-variant: '#004e5c'
  background: '#10131a'
  on-background: '#e1e2eb'
  surface-variant: '#32353c'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '800'
    lineHeight: 38px
  display-lg-mobile:
    fontFamily: Inter
    fontSize: 26px
    fontWeight: '800'
    lineHeight: 32px
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 30px
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 26px
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-code:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  label-badge:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 14px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 0.75rem
  margin: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.75rem
  space-lg: 1rem
  space-xl: 1.5rem
---

## Brand & Style

This design system establishes a high-performance, dark cyberpunk aesthetic tailored explicitly for Telegram Mini Apps (TMA). It unites Telegram's native brand clarity with an immersive, high-energy neon interface suited for Web3 mini-games, AI agent interfaces, live social audio channels, and bot ecosystems.

The visual direction combines **Sleek Cyberpunk** and **Frosted Glassmorphism**:
- Ultra-deep dark backgrounds (#0B0E14) prevent visual fatigue inside the Telegram client wrapper and conserve battery on mobile OLED screens.
- Controlled atmospheric neon glows and vibrant accent cues indicate real-time activities (voice streams, AI computing states, moderation flags, and gaming events).
- Interaction states deliver hyper-responsive tactile feedback, matching native Telegram WebApp standards (safe-area aware, gesture-friendly, and haptic-aligned).

## Colors

The palette operates on a strict functional token structure in a dark-only mode:

### Base Canvas & Surfaces
- **Canvas Base**: `#0B0E14` (Deep Midnight Void)
- **Surface Elevation 1 (Card/Containers)**: `#121824`
- **Surface Elevation 2 (Elevated Sheets/Modals)**: `#1A2234`
- **Surface Elevation Glass**: `rgba(18, 24, 36, 0.72)` with 16px backdrop-filter blur
- **Hairline Borders**: `rgba(255, 255, 255, 0.08)`
- **Hairline Borders Active/Hover**: `rgba(36, 161, 222, 0.35)`

### Primary & Functional Accents
- **Primary (Telegram Electric Blue)**: `#24A1DE` (Interactive actions, verified badges, primary buttons)
- **Primary Glow**: `rgba(36, 161, 222, 0.25)`
- **Secondary (Neon Violet)**: `#8B5CF6` (AI processing nodes, generative features, Web3 utilities)
- **Tertiary (Cyber Cyan)**: `#06B6D4` (Music frequency visualizers, telemetry streams, speed boosts)
- **Success / Live (Emerald Green)**: `#10B981` (Active voice chat rooms, ping latency, player connected)
- **Warning / Moderation (Neon Amber)**: `#F59E0B` (Telegram bot warnings, rate limits, moderation actions)
- **Danger (Cyber Crimson)**: `#EF4444` (Disconnect, kick, purge, destructive flows)

### Typography & Content Neutrals
- **Text High-Contrast**: `#F8FAFC` (Titles, values, primary labels)
- **Text Medium-Contrast**: `#94A3B8` (Descriptions, secondary headers)
- **Text Low-Contrast / Disabled**: `#475569` (Placeholders, inactive tabs)

## Typography

The typography system relies on **Inter** for crisp, scalable legibility across density screens, paired with **JetBrains Mono** for status codes, bot commands, numeric rewards, and token tallies.

### Scaling & Legibility Rules
- Numerical meters (game scores, wallet balances, mining counters) utilize tabular figures (`font-variant-numeric: tabular-nums`) to prevent layout shifts during live increments.
- Letter spacing is tightened on large display headlines (`letter-spacing: -0.02em`) for a solid, commanding presence.
- Badges and monospaced telemetry tokens enforce uppercase formatting with `letter-spacing: 0.05em` to preserve scannability at small sizes within Telegram's in-app viewport.

## Layout & Spacing

The layout is built mobile-first, engineered specifically for Telegram's WebApp frame constraint (`window.Telegram.WebApp`).

### Viewport & Telegram Chrome Accommodation
- **Top Safe Area**: A dynamic padding offset accommodates Telegram’s native header buttons (`Close`, `More Options`, expandable navigation).
- **Bottom Safe Area**: 16px base padding plus the mobile device's home indicator safe-area-inset. Fixed primary buttons ("MainButton") rest with a persistent floating gap of `1rem`.
- **Canvas Width Constraint**: On desktop Telegram clients, the canvas restricts to a maximum width of `480px`, auto-centering with ambient side drop-glows to preserve the focused mobile app feel.

### Layout Grid
- Content utilizes a continuous fluid column layout with `1rem` outer margins (`margin-mobile: 16px`, `margin-desktop: 24px`) and `0.75rem` (12px) component spacing gaps to optimize vertical screen efficiency.

## Elevation & Depth

Visual hierarchy uses frosted glassmorphism over dark surfaces paired with spectral neon back-glows.

### Layer Stack
1. **Canvas Level 0**: `#0B0E14` base background, with subtle, fixed-position radial gradients of electric cyan (`#06B6D410`) and violet (`#8B5CF60F`) at the screen corners.
2. **Surface Level 1 (Panels & Feed Cards)**: Background `rgba(18, 24, 36, 0.75)` with `backdrop-filter: blur(14px)` and a single outline border of `1px solid rgba(255, 255, 255, 0.08)`.
3. **Surface Level 2 (Sheets, Drawers, Flyouts)**: Background `rgba(26, 34, 52, 0.92)` with `backdrop-filter: blur(20px)` and outer box-shadow: `0 8px 32px -4px rgba(0, 0, 0, 0.65)`.
4. **Neon Atmospheric Glows**: Key interactives apply localized soft neon drop-shadows:
   - Telegram Blue Action: `0 4px 18px rgba(36, 161, 222, 0.35)`
   - Emerald Voice Active: `0 0 14px rgba(16, 185, 129, 0.40)`
   - Violet AI Pulsing: `0 0 20px rgba(139, 92, 246, 0.35)`

## Shapes

The design system maintains a balanced curved geometry (`roundedness: 2`):

- **Cards and Panels**: `1rem` (16px) corner radius creates a modern handheld feel that mirrors Telegram’s rounded UI surfaces.
- **Modals and Action Sheets**: `1.5rem` (24px) for upper sheet corners.
- **Pill Elements**: Full-pill `9999px` radius is reserved for interactive filters, chips, game item tags, and Telegram user avatars.
- **Form Controls & Micro Inputs**: `0.75rem` (12px) for structured tactile tap areas.

## Components

### Buttons
- **Primary CTA**: Electric Telegram Blue (`#24A1DE`), crisp white typography (`Inter` 600), subtle cyan top-inset highlight line, and an active state that scales to `0.98` with enhanced glow.
- **Neon Glass (Secondary)**: Background `rgba(255, 255, 255, 0.05)`, border `1px solid rgba(255, 255, 255, 0.12)`, text `#F8FAFC`.
- **Destructive**: Background `rgba(239, 68, 68, 0.15)`, border `1px solid rgba(239, 68, 68, 0.4)`, text `#EF4444`.

### Chips & Pill Tags
- **Filter Pills**: Semi-translucent dark background with uppercase `label-code` typography. Selected state turns Telegram Blue with a matching `0 0 10px rgba(36, 161, 222, 0.3)` glow.
- **Status Badges**: Full-pill containers housing a pulsing 6px colored dot:
  - Voice active: `#10B981` (pulsing)
  - AI thinking: `#8B5CF6` (breathing animation)
  - Bot Warning: `#F59E0B` (static high contrast)

### Cards
- **Cyber Glass Card**: Background `rgba(18, 24, 36, 0.7)`, border `1px solid rgba(255, 255, 255, 0.08)`, border-radius `16px`. Provides clean separation without visual weight.
- **Game / Action Module**: Same as Cyber Glass Card, but with an active gradient accent border (e.g., cyan-to-violet linear-gradient border on hover or focus).

### Lists & Activity Rows
- Borderless rows separated by `8px` vertical spacing.
- Left-aligned icon/avatar container with rounded-full pill status pip.
- Title in high-contrast text (`#F8FAFC`) with trailing metadata rendered in `JetBrains Mono` (`#94A3B8`).

### Input Fields
- Height `48px` to guarantee zero miss-clicks in mobile Telegram.
- Background `rgba(11, 14, 20, 0.85)` inset with `1px solid rgba(255, 255, 255, 0.1)`.
- Focused state: Border transitions to `#24A1DE` with `0 0 12px rgba(36, 161, 222, 0.25)` drop-glow.

### Checkboxes & Switches
- **Switches**: Track size `48px x 28px`, background `rgba(255, 255, 255, 0.1)`. Active track fills with `#24A1DE` or `#10B981`, thumb is solid white with ambient neon halo.
- **Checkboxes**: Rounded `6px` square with border `rgba(255, 255, 255, 0.25)`. Checked state delivers instant electric cyan fill with a high-contrast check icon.

### Telegram Specific: Floating Bottom Nav & Haptic Indicators
- **Navigation Dock**: Floating glass bar at the bottom with 5 navigation anchors, 12px elevated from bottom safe margin, active tab highlighted with a neon indicator line.