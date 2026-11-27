---
name: "Hiraya Bay Coastal Sanctuary"
description: "Warm sand surfaces, deep bay teal, and editorial serif-sans typography inspired by Hiraya Bay Resort in Biliran."
---

## Overview

Hiraya Bay Coastal Sanctuary is a calm, warm, hospitality-first design system built for managing resort operations, reservations, and guest experiences at Hiraya Bay Resort (Sitio Anyog, Brgy. Looc, Cabucgayan, Biliran). The interface pairs sunlit sand-and-shell surfaces with deep coastal bay teal and natural bamboo-wood accents, evoking barefoot island tranquility while keeping operational metrics, kubo availability, and guest feedback immediately scannable on desktop.

## Colors

The palette is anchored in the resort's signature coastal teal (`#0D7C8A` / `#00626D`) over warm shell-cream surfaces (`#FFF8F4`) and soft sand containers (`#FFF1E4`), with warm bamboo amber (`#834A14`) reserved for campfire, wood, and hospitality highlights. Status colors (`success`, `warning`, `error`) are used strictly for booking states, occupancy alerts, and operational statuses.

```yaml
colors:
  success: "#1F6E43"
  on-success: "#FFFFFF"
  success-container: "#D6F5E3"
  on-success-container: "#0B4627"
  warning: "#9A5B00"
  on-warning: "#FFFFFF"
  warning-container: "#FFEDD5"
  on-warning-container: "#6B3D00"
  light:
    primary: "#00626D"
    on-primary: "#FFFFFF"
    primary-container: "#0D7C8A"
    on-primary-container: "#E2FAFF"
    secondary: "#456369"
    on-secondary: "#FFFFFF"
    secondary-container: "#C7E8EF"
    on-secondary-container: "#4B696F"
    tertiary: "#834A14"
    on-tertiary: "#FFFFFF"
    tertiary-container: "#A0622B"
    on-tertiary-container: "#FFF4EE"
    error: "#BA1A1A"
    on-error: "#FFFFFF"
    error-container: "#FFDAD6"
    on-error-container: "#93000A"
    background: "#FFF8F4"
    on-background: "#211B12"
    surface: "#FFF8F4"
    surface-dim: "#E5D8CB"
    surface-bright: "#FFF8F4"
    surface-container-lowest: "#FFFFFF"
    surface-container-low: "#FFF1E4"
    surface-container: "#F9ECDE"
    surface-container-high: "#F3E6D9"
    surface-container-highest: "#EEE0D3"
    on-surface: "#211B12"
    surface-variant: "#D9E4E7"
    on-surface-variant: "#3E494B"
    outline: "#6E797B"
    outline-variant: "#BDC8CB"
    inverse-surface: "#372F26"
    inverse-on-surface: "#FCEFE1"
    inverse-primary: "#7CD4E3"
  dark:
    primary: "#7CD4E3"
    on-primary: "#00363D"
    primary-container: "#0D7C8A"
    on-primary-container: "#E2FAFF"
    secondary: "#ACCCD3"
    on-secondary: "#15353A"
    secondary-container: "#2F4E53"
    on-secondary-container: "#9EBEC4"
    tertiary: "#FFB77E"
    on-tertiary: "#4D2600"
    tertiary-container: "#A0622B"
    on-tertiary-container: "#FFF4EE"
    error: "#FFB4AB"
    on-error: "#690005"
    error-container: "#93000A"
    on-error-container: "#FFDAD6"
    background: "#18120B"
    on-background: "#EEE0D3"
    surface: "#18120B"
    surface-dim: "#18120B"
    surface-bright: "#40382F"
    surface-container-lowest: "#130D06"
    surface-container-low: "#211B12"
    surface-container: "#251F16"
    surface-container-high: "#302920"
    surface-container-highest: "#3B342A"
    on-surface: "#EEE0D3"
    surface-variant: "#3E494B"
    on-surface-variant: "#BDC8CB"
    outline: "#889395"
    outline-variant: "#3E494B"
    inverse-surface: "#EEE0D3"
    inverse-on-surface: "#372F26"
    inverse-primary: "#006875"
```

## Typography

**Noto Serif** brings editorial coastal warmth to page titles, KPI figures, and section headings. **Plus Jakarta Sans** handles navigation, table cells, badges, and body copy with clean geometric legibility. **Source Code Pro** formats booking reference IDs, timestamps, and tabular currency figures.

```yaml
typography:
  display-lg:
    fontFamily: "Noto Serif"
    fontSize: 40px
    fontWeight: 600
    lineHeight: 48px
    letterSpacing: -0.5px
  display-lg-mobile:
    fontFamily: "Noto Serif"
    fontSize: 30px
    fontWeight: 600
    lineHeight: 36px
    letterSpacing: -0.25px
  headline-lg:
    fontFamily: "Noto Serif"
    fontSize: 28px
    fontWeight: 600
    lineHeight: 34px
    letterSpacing: -0.25px
  headline-md:
    fontFamily: "Noto Serif"
    fontSize: 22px
    fontWeight: 600
    lineHeight: 28px
    letterSpacing: -0.1px
  title-lg:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 18px
    fontWeight: 600
    lineHeight: 24px
    letterSpacing: 0px
  title-md:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 16px
    fontWeight: 600
    lineHeight: 22px
    letterSpacing: 0px
  body-lg:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 15px
    fontWeight: 400
    lineHeight: 22px
    letterSpacing: 0px
  body-md:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
    letterSpacing: 0px
  body-sm:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 12px
    fontWeight: 400
    lineHeight: 18px
    letterSpacing: 0.1px
  label-lg:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 14px
    fontWeight: 600
    lineHeight: 20px
    letterSpacing: 0.1px
  label-md:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 12px
    fontWeight: 600
    lineHeight: 16px
    letterSpacing: 0.3px
  label-sm:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 12px
    fontWeight: 500
    lineHeight: 16px
    letterSpacing: 0.4px
  mono-md:
    fontFamily: "Source Code Pro"
    fontSize: 13px
    fontWeight: 500
    lineHeight: 18px
    letterSpacing: 0px
```

## Layout & Spacing

Desktop dashboards use a fixed 240px left navigation rail paired with a fluid main workspace constrained to a comfortable max-width of 1280px, built on a 12-column CSS grid with 20px–24px gutters. On tablet and mobile viewports, multi-column KPI and widget grids collapse cleanly to 2 or 1 columns and the sidebar tucks behind a header toggle. Spacing follows a strict 4px/8px grid.

```yaml
spacing:
  gutter-xs: 4px
  gutter-sm: 8px
  gutter-md: 16px
  gutter-lg: 24px
  gutter-xl: 32px
  section: 40px
  page-margin: 24px
```

## Elevation & Depth

Depth is conveyed primarily through **tonal surface layering** rather than heavy drop shadows: the warm shell canvas (`surface`) holds crisp white cards (`surface-container-lowest`) and soft sand highlight panels (`surface-container-low`), separated by subtle `outline-variant` hairline borders at low opacity. Interactive cards lift gently on hover with an ambient warm-tinted shadow.

## Shapes

Cards, accommodation tiles, and dashboard widgets use generous, approachable rounded corners (`16px` / `20px`) reminiscent of woven bamboo and smooth coastal stone, while buttons, filter chips, and status pills use `9999px` pill or `12px` soft-rect shapes.

```yaml
rounded:
  sm: 8px
  DEFAULT: 12px
  md: 16px
  lg: 20px
  xl: 24px
  full: 9999px
```

## Motion & Micro-interaction

Transitions feel unhurried and tactile, matching the calm coastal pace. State changes on buttons, tabs, and filter pills resolve in 150ms, while drawer or panel reveals decelerate smoothly over 250ms. No decorative looping animations are used.

```yaml
motion:
  state-change:
    duration: 150ms
    delay: 0ms
    timingFunction: ease-out
  surface-enter:
    duration: 250ms
    delay: 0ms
    timingFunction: cubic-bezier(0.2, 0, 0, 1)
  surface-exit:
    duration: 150ms
    delay: 0ms
    timingFunction: cubic-bezier(0.3, 0, 1, 1)
```

## Voice & Content Strategy

Copy is **warm, clear, and hospitality-minded**—friendly without being chatty, and precise on rates, guest counts, and check-in/check-out times. Use sentence case for headings and labels, verb-led action labels ("New Reservation", "Check In Guest", "Export Summary"), Philippine Peso (`₱`) formatting with `tabular-nums` for all rates and revenue, and authentic Hiraya Bay Resort terms (`Native Kubo`, `Day Tour Cottage`, `Grand Gazebo`, `Cliff Bayview Suite`, `Cliffside Pool`, `Starlit Campfire`).

## Components

Component implementations live as individual HTML sticker sheet files in
`components/`. Each file contains the canonical, styled HTML components with
`<!-- COMPONENT: name -->` comment markers. Read each file before use.

- **Badge** → `@components/badge.html` — `badge-numeric`, `badge-dot`
- **Button** → `@components/button.html` — `button-primary`, `button-icon`, `button-with-icon`
- **Card** → `@components/card.html` — `card-elevated`, `card-action`, `card-interactive`, `card-interactive-2`
- **Table** → `@components/table.html` — `table-standard`, `table-interactive`, `table-selectable`
