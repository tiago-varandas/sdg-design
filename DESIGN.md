---
version: alpha
name: SDG.design
description: Editorial design system for SDG.design — a magazine-style library of DESIGN.md files for SDG builders. White canvas, bold color blocks, extreme typographic contrast. Each SDG card is a designed object. Feels like a design publication, not a tool directory.

colors:
  background: "#FFFFFF"
  surface: "#FFFFFF"
  surface-ink: "#F2F0EB"
  primary: "#0D0D0B"
  secondary: "#5C5C58"
  tertiary: "#ADADAA"
  rule: "#E8E6E1"
  sdg-water: "#29BFE0"
  sdg-health: "#4C9B47"
  sdg-education: "#C5192D"
  sdg-equality: "#FF3A21"
  sdg-cities: "#FD9D24"
  sdg-climate: "#3F7E44"
  sdg-poverty: "#E5243B"
  sdg-hunger: "#DDA63A"
  sdg-energy: "#FCC30B"
  sdg-work: "#A21942"
  sdg-industry: "#FD6925"
  sdg-inequality: "#DD1367"
  sdg-consumption: "#BF8B2E"
  sdg-ocean: "#0A97D9"
  sdg-land: "#56C02B"
  sdg-peace: "#00689D"
  sdg-partnership: "#19486A"

typography:
  display:
    fontFamily: "Helvetica Neue"
    fontSize: 96px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.04em
  display-sm:
    fontFamily: "Helvetica Neue"
    fontSize: 64px
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: -0.04em
  sdg-number:
    fontFamily: "Helvetica Neue"
    fontSize: 120px
    fontWeight: 700
    lineHeight: 1.0
    letterSpacing: -0.05em
  headline:
    fontFamily: "Helvetica Neue"
    fontSize: 18px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: -0.02em
  body:
    fontFamily: "Helvetica Neue"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: -0.005em
  meta:
    fontFamily: "Helvetica Neue Condensed"
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0.1em
  code:
    fontFamily: "JetBrains Mono"
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: 0.02em

rounded:
  none: 0px
  sm: 2px
  md: 4px
  lg: 6px
  full: 9999px

spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 64px
  2xl: 128px
  3xl: 200px

components:
  sdg-card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.none}"
    padding: 0px
  sdg-card-hover:
    backgroundColor: "{colors.surface-ink}"
  sdg-color-block:
    rounded: "{rounded.none}"
    height: 160px
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.background}"
    rounded: "{rounded.none}"
    padding: 16px
  button-primary-hover:
    backgroundColor: "{colors.sdg-water}"
    textColor: "{colors.primary}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.secondary}"
    rounded: "{rounded.none}"
    padding: 16px
  tag:
    backgroundColor: "transparent"
    textColor: "{colors.tertiary}"
    rounded: "{rounded.none}"
    padding: 0px
  rule:
    backgroundColor: "{colors.rule}"
    height: 1px
  nav:
    backgroundColor: "{colors.background}"
    textColor: "{colors.secondary}"
    padding: 24px
  code-block:
    backgroundColor: "{colors.surface-ink}"
    textColor: "{colors.primary}"
    rounded: "{rounded.none}"
    padding: 20px
---

# SDG.design

## Overview

SDG.design is an editorial library of DESIGN.md starter kits for the 17 Sustainable Development Goals. The visual identity is a design magazine — bold, authoritative, and typographically confident. It does not look like a sustainability website. It looks like something a design director would create.

The primary reference is editorial graphic design — think Emigre, Dot Dot Dot, Eye Magazine. Large type. Extreme scale contrast. Color as identity block, not tint. White space used with intention, not as padding.

Each SDG card is a designed object. The SDG number is set at 120px — it is the dominant visual element of every card. Below it, a color block in the SDG's identity color occupies the full card width at 160px height. This creates the L'Autre Soie effect — photography (or in our case, a pure color field) interrupted by a bold typographic layer.

The overall page reads like an issue of a design publication — a hero section that makes a statement, a grid of cards that reward close reading, and a demo section that tells a story in three acts.

No rounded corners anywhere on the main interface. Sharp edges signal precision and editorial authority. Full radius is reserved only for pill tags inside the SDG-specific design systems — never on the gallery UI itself.

## Colors

Pure white canvas. The SDG identity colors are the only color on the page. They appear as solid blocks within cards — full saturation, full opacity. Never as tints, gradients, or backgrounds.

- **Background (#FFFFFF):** Pure white. The page is a sheet of paper.
- **Surface Ink (#F2F0EB):** Warm paper tint. Used only for hover states and code blocks.
- **Primary (#0D0D0B):** Near-black. All headlines, body text, primary buttons.
- **Secondary (#5C5C58):** Mid grey. Metadata, nav links, secondary text.
- **Tertiary (#ADADAA):** Light grey. Tags, captions, timestamps.
- **Rule (#E8E6E1):** Hairline rule. Section dividers, card borders.

Each of the 17 SDG identity colors is used only within its card's color block and as the dominant color in that SDG's own DESIGN.md system. They never bleed into the global navigation or typography.

## Typography

Helvetica Neue is the only typeface. It is used at extreme scale contrast — the SDG number at 120px sits next to metadata at 10px. This is the Nitsa Club typographic principle: the contrast between scales is the design.

The `display` scale (96px, weight 700) is for the hero headline only. One appearance per page. No other element competes with it.

`sdg-number` (120px, weight 700) is the typographic identity of every card. It bleeds into the color block beneath it — the number visually interrupts the color, creating tension between text and image exactly as in the L'Autre poster series.

`meta` uses Helvetica Neue Condensed at 10px, all caps, wide tracking — the editorial label style. Used for SDG category labels, download counts, variant labels. Never for body text.

`code` uses JetBrains Mono — the only non-Helvetica typeface, used exclusively for DESIGN.md code previews.

Weight 700 for display and numbers. Weight 500 for headlines. Weight 400 for body. Never any other weights.

## Layout

Maximum width 1500px, centered. Side margins 64px desktop, 24px mobile.

**Navigation:** Pure typographic. Wordmark left (sdg.design, 14px, weight 500). Nav links center (Browse, About, GitHub) in secondary color. CTA right (Download all) as a text link with arrow, not a button. A single 1px rule below the nav. No background color — the nav sits on the white page.

**Hero:** Full-width typographic section. Display headline ("Design for what matters.") at 96px, bleeding to the left margin. Below: a single rule, then a two-column layout — left column: subheadline and CTA, right column: the stat line and a short editorial paragraph about the project.

**Card grid:** Asymmetric masonry, 4 columns desktop. No gutters between cards — they butt up against each other with only a hairline rule. Each card: color block at top (full width, 160px, SDG identity color), large number overlapping the color block bottom edge, SDG name in headline scale, descriptor in body, meta tags, download link. No card shadows. No card backgrounds beyond the color block.

**Demo section:** Full bleed. Title at display-sm scale. Three product screens at large scale side by side, each labeled in meta style below.

## Elevation & Depth

None. This is a flat, ink-on-paper system. No shadows, no elevation, no gradients. Depth is created entirely through typographic scale contrast and the color blocks within cards.

## Shapes

Zero border radius on all containers, cards, and buttons. The sharpness is intentional — it signals editorial precision. The only exception is pill-style tags within individual SDG DESIGN.md files where the rounded language supports approachability for that specific goal.

## Components

**SDG Card:** Color block (160px tall, full SDG identity color, sharp edges). SDG number (120px, primary color, overlapping the bottom edge of the color block by 40px — creating the poster tension). SDG name (headline scale, below). One-line descriptor (body, secondary). Two meta tags (10px condensed, tertiary). Download link (body, primary, with →).

**Color Block:** The visual signature of every card. A flat rectangle of pure SDG identity color. No gradients, no images, no texture. The number bleeds into it from below.

**Rule:** 1px horizontal line in #E8E6E1. Used between nav and hero, between sections, and as the invisible border between cards in the grid.

**Code Block:** Surface-ink background (#F2F0EB). JetBrains Mono, 11px. No border radius. Left rule in SDG identity color, 3px. The one moment of color in an otherwise monochrome code panel.

**Nav:** Pure text. No background, no shadow, no border — just the single rule below. The wordmark in primary. Links in secondary. CTA as underlined text link.

**Meta Tag:** 10px Helvetica Neue Condensed, all caps, wide tracking, tertiary color. No pill background — the text sits naked on the white surface. Multiple tags separated by a thin slash or em dash.

## Do's and Don'ts

- Do let the SDG number bleed into the color block — the overlap creates the editorial tension that makes each card feel designed
- Do use Helvetica Neue exclusively — introducing a second typeface breaks the typographic system
- Don't add rounded corners to any container on the main gallery — sharpness is the identity
- Do maintain extreme scale contrast — the 120px number next to 10px metadata is the design
- Don't use SDG identity colors as backgrounds on the main page — only as the card color block
- Do use hairline rules (1px) as structural elements — they replace borders and shadows
- Don't centre-align text — everything is left-aligned. Centre alignment is decorative; this system is editorial
- Do keep the nav purely typographic — no button shapes, no background fills in the nav
- Don't add more than two meta tags per card — white space is information
- Do let cards touch each other with only a hairline rule between — no gutters, no padding between cards in the grid
