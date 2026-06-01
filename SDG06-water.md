---
version: alpha
name: SDG.design — 06 Clean Water
description: Design system for SDG 6 — Clean Water and Sanitation. Two variants: a community monitoring tool and a policy advocacy platform. Pure, vital, trusted.

colors:
  primary: "#0A3D52"
  secondary: "#2D7A9A"
  tertiary: "#6DB8CE"
  background: "#F0FAFE"
  surface: "#FFFFFF"
  surface-subtle: "#E3F5FB"
  accent: "#29BFE0"
  accent-deep: "#0A7A99"
  neutral: "#4A6572"
  success: "#2E9E6B"
  warning: "#E8A020"
  error: "#D94F3D"

typography:
  headline:
    fontFamily: "Helvetica Neue"
    fontSize: 40px
    fontWeight: 500
    lineHeight: 1.1
    letterSpacing: -0.03em
  title:
    fontFamily: "Helvetica Neue"
    fontSize: 20px
    fontWeight: 500
    lineHeight: 1.25
    letterSpacing: -0.02em
  body:
    fontFamily: "Helvetica Neue"
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.7
    letterSpacing: -0.01em
  label:
    fontFamily: "JetBrains Mono"
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.05em
  data:
    fontFamily: "JetBrains Mono"
    fontSize: 24px
    fontWeight: 500
    lineHeight: 1.0
    letterSpacing: -0.02em

rounded:
  sm: 4px
  md: 8px
  lg: 12px
  xl: 20px
  full: 9999px

spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  2xl: 80px

components:
  button-primary:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
    padding: 20px
  button-primary-hover:
    backgroundColor: "{colors.accent-deep}"
    textColor: "#FFFFFF"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
    padding: 20px
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-data:
    backgroundColor: "{colors.surface-subtle}"
    rounded: "{rounded.lg}"
    padding: 20px
  status-safe:
    backgroundColor: "#E6F7F1"
    textColor: "{colors.success}"
    rounded: "{rounded.full}"
    padding: 8px
  status-warning:
    backgroundColor: "#FEF5E7"
    textColor: "{colors.warning}"
    rounded: "{rounded.full}"
    padding: 8px
  status-alert:
    backgroundColor: "#FDECEA"
    textColor: "{colors.error}"
    rounded: "{rounded.full}"
    padding: 8px
  nav:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFF"
    padding: 16px
---

# SDG.design — 06 Clean Water

## Overview

SDG 6 calls for clean water and sanitation for all by 2030. Design for this goal must convey trust, clarity, and urgency without panic. Water is essential and precious — the visual language should reflect both its purity and its criticality.

This system serves two distinct builder contexts. The first is community-level tools — apps used by local water committees, field workers, and residents to monitor boreholes, report problems, and track usage. These need to work on low-end devices, in low-literacy contexts, and often offline. The second is policy and advocacy platforms — tools used by NGOs, journalists, and governments to communicate water access data and drive systemic change.

Both variants share the same color foundation but diverge in typographic weight and information density. Community tools favour large touch targets, icon-supported navigation, and calm status indicators. Advocacy platforms favour data-dense layouts, strong typographic hierarchy, and shareable chart components.

The palette draws from clear water and deep ocean — cyan accent against deep teal, on a near-white background with the faintest blue tint. Status colors are essential: safe (green), warning (amber), and critical (red) must be immediately legible in field conditions, including bright sunlight.

## Colors

The palette is built on deep teal for authority and trust, with a bright cyan accent for interactive moments and data highlights.

- **Primary (#0A3D52):** Deep ocean teal. Headlines, primary text, dark nav backgrounds.
- **Secondary (#2D7A9A):** Mid teal. Section headers, active states, link text.
- **Tertiary (#6DB8CE):** Light teal. Decorative borders, chart fills, secondary data.
- **Background (#F0FAFE):** Barely-blue white. The page canvas — suggests clean water without being heavy.
- **Surface (#FFFFFF):** Card backgrounds. Pure white for maximum contrast with data.
- **Surface Subtle (#E3F5FB):** Data card backgrounds, input fields, recessed panels.
- **Accent (#29BFE0):** Bright cyan. Primary CTAs, interactive highlights, live data indicators.
- **Accent Deep (#0A7A99):** Pressed/hover state for accent. Also used for chart emphasis.
- **Neutral (#4A6572):** Body text, metadata, secondary labels.
- **Success (#2E9E6B):** Safe water status. Used consistently for positive readings.
- **Warning (#E8A020):** Caution status. Elevated contamination, low pressure, maintenance needed.
- **Error (#D94F3D):** Critical status. Unsafe water, system failure, urgent action required.

## Typography

Inter throughout — clean, legible at small sizes, and widely available on low-end devices.

Headlines set tight at -0.03em tracking — authoritative without being heavy. Body text at 15px with generous 1.7 line height for low-literacy readability.

Inter Mono is essential for two contexts: data labels (pump readings, contamination levels, flow rates) and technical field labels. Numbers must be monospace so they align in tables and dashboards.

The `data` type scale is the defining typographic moment — 24px monospace numerals for live sensor readings. Large enough to read from a meter away, clear enough to read in bright outdoor conditions.

## Layout

**Community tool variant:** Single-column mobile layout. Maximum 400px content width. Large touch targets minimum 48px. Bottom navigation with icon + label. Map view as primary screen. Status indicators visible above the fold at all times.

**Advocacy platform variant:** Desktop-first, two-column layout. Maximum 1200px. Left column: navigation and filters. Right column: data visualisations and narrative content. Designed for sharing — every chart has a built-in export button.

Spacing is generous throughout — 24px card padding minimum to prevent content feeling cramped on small screens.

## Elevation & Depth

Cards float on the barely-blue background with a subtle 0.5px border in surface-subtle. No drop shadows — they create ambiguity on low-quality screens. Status cards use background color fills (green/amber/red tints) to signal state — no border required.

Data cards (sensor readings, stats) use surface-subtle background to distinguish them from content cards.

## Shapes

12px radius for cards and panels. Full radius for status pills, buttons, and tags. The rounded language signals approachability — this tool is for communities, not bureaucracies.

Input fields: 8px radius. Tab navigation: 4px radius top only.

## Components

**Status Pill:** The most critical component. Three states — safe (green), warning (amber), critical (red). Always visible. Used in map markers, list items, and dashboard headers. Icon + label + timestamp.

**Data Card:** Monospace large number, unit label below in small caps, trend indicator (arrow + percentage). Used for pump pressure, pH level, flow rate, days since last test.

**Map Marker:** Circle with status color fill. Tap expands to card with full readings. Critical markers pulse with a subtle animation.

**Report Button:** Prominent, always accessible. "Report a problem" — accent background, full width on mobile. The single most important action for community users.

**Nav (Community):** Bottom bar, 5 items maximum. Icon + label. Active state: accent color. Inactive: neutral.

**Nav (Advocacy):** Left sidebar, desktop. Section headers in primary. Active link: accent-deep with left border indicator.

## Do's and Don'ts

- Do use status colors consistently — safe is always green, warning always amber, critical always red. Never repurpose these colors decoratively.
- Do make the Report button impossible to miss on community tool screens
- Don't use more than three data cards above the fold — information overload causes inaction
- Do support offline states gracefully — show last-known data with a clear timestamp
- Don't use light text on the accent cyan — contrast is insufficient. Use primary dark text instead.
- Do design for glanceability — a field worker should understand a screen's meaning in under 2 seconds
- Don't hide critical alerts behind tabs or menus — they must be immediately visible
- Do use Inter Mono for all numerical data — proportional numerals misalign in tables

## Field Conditions

This design system is used outdoors. Most water monitoring tools fail in the field because they were designed indoors on calibrated monitors. These constraints are non-negotiable:

**Sunlight legibility:** Minimum contrast ratio 7:1 for all data displays — not the WCAG standard 4.5:1. Field workers read phones in direct sunlight at arm's length. The accent cyan (#29BFE0) on white fails at 2.1:1 — never use it as text. Always use primary dark (#0A3D52) on light backgrounds for any critical reading.

**The 3-tap rule:** Any critical action (report contamination, flag pump failure, request maintenance) must be completable in 3 taps from the home screen. Field workers often have wet or gloved hands. No action that matters should require navigation deeper than 3 levels.

**Glanceability test:** Cover the screen labels. Can a field worker understand the status of every monitored site from icons and colors alone in under 2 seconds? If not, the information hierarchy is wrong. Status must be visible before text is readable.

**Battery and data:** The average community field worker in a low-income region has less than 40% battery when they reach a remote site. Every screen should load in under 2 seconds on a 3G connection. Avoid loading states for primary data — cache aggressively.
