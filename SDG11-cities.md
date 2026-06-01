---
version: alpha
name: SDG.design — 11 Sustainable Cities
description: Design system for SDG 11 — Sustainable Cities and Communities. Two variants: a civic reporting tool and an urban planning dashboard. Connected, dynamic, communal.

colors:
  primary: "#1A1508"
  secondary: "#7A4E08"
  tertiary: "#F4B85A"
  background: "#FFFAF4"
  surface: "#FFFFFF"
  surface-subtle: "#FFF4E6"
  accent: "#FD9D24"
  accent-deep: "#C87810"
  neutral: "#4A4030"
  civic: "#2D5986"
  civic-soft: "#EAF0F8"
  success: "#2E7D4F"
  alert: "#C53030"

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
    lineHeight: 1.65
    letterSpacing: -0.01em
  label:
    fontFamily: "JetBrains Mono"
    fontSize: 11px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0.05em
  stat:
    fontFamily: "Helvetica Neue"
    fontSize: 36px
    fontWeight: 500
    lineHeight: 1.0
    letterSpacing: -0.03em
  map-label:
    fontFamily: "JetBrains Mono"
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0.04em

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
  button-civic:
    backgroundColor: "{colors.civic}"
    textColor: "#FFFFFF"
    rounded: "{rounded.full}"
    padding: 20px
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.neutral}"
    rounded: "{rounded.full}"
    padding: 20px
  card:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
    padding: 24px
  card-civic:
    backgroundColor: "{colors.civic-soft}"
    rounded: "{rounded.lg}"
    padding: 20px
  card-stat:
    backgroundColor: "{colors.surface-subtle}"
    rounded: "{rounded.lg}"
    padding: 20px
  report-button:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.primary}"
    rounded: "{rounded.xl}"
    padding: 24px
  status-open:
    backgroundColor: "{colors.surface-subtle}"
    textColor: "{colors.accent-deep}"
    rounded: "{rounded.full}"
    padding: 8px
  status-in-progress:
    backgroundColor: "{colors.civic-soft}"
    textColor: "{colors.civic}"
    rounded: "{rounded.full}"
    padding: 8px
  status-resolved:
    backgroundColor: "#E6F4ED"
    textColor: "{colors.success}"
    rounded: "{rounded.full}"
    padding: 8px
  nav:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.neutral}"
    padding: 16px
---

# SDG.design — 11 Sustainable Cities

## Overview

SDG 11 calls for inclusive, safe, resilient, and sustainable cities and human settlements. Design for this goal must bridge two worlds: the everyday experience of residents navigating their city, and the complex systems of planners, officials, and civic technologists managing it.

This system serves two builder contexts. The first is civic reporting tools — apps used by residents to report infrastructure problems (potholes, broken lights, flooding), vote on local priorities, and track whether their reports are being acted on. These must be fast, frictionless, and trustworthy. The second is urban planning dashboards — tools used by city planners, NGOs, and civic technologists to visualise urban data, model interventions, and communicate findings to stakeholders.

Civic tools live or die on perceived responsiveness. If residents report problems and never see them resolved, they stop reporting. The design must make both the act of reporting and the act of following up feel worthwhile.

The palette draws from the official SDG 11 amber-orange — warm, urban, energetic. This is the color of street lights and construction signs — visible, actionable, civic. A secondary civic blue handles official and institutional content, creating a natural two-role palette.

## Colors

Warm amber for civic action, deep blue for institutional information. Two distinct visual roles that never compete.

- **Primary (#1A1508):** Deep warm black. Headlines and body text.
- **Secondary (#7A4E08):** Deep amber. Active states and emphasis.
- **Tertiary (#F4B85A):** Light amber. Chart fills, decorative accents.
- **Background (#FFFAF4):** Barely-warm white. Urban warmth.
- **Surface (#FFFFFF):** Cards and panels.
- **Surface Subtle (#FFF4E6):** Stat cards, input backgrounds, recessed panels.
- **Accent (#FD9D24):** Amber orange. Primary CTAs, report buttons, active map markers.
- **Accent Deep (#C87810):** Hover and pressed states for accent.
- **Neutral (#4A4030):** Warm body text.
- **Civic (#2D5986):** Official blue. Used for government-sourced data, verified information, institutional cards. Never for CTAs — that role belongs to amber.
- **Civic Soft (#EAF0F8):** Background for civic/official content cards.

## Typography

The `stat` scale (36px, weight 500) handles the key numbers that define urban dashboards — incident counts, resolution rates, resident satisfaction scores. Large enough to read across a meeting room screen.

`map-label` (10px Inter Mono) is used for map overlays — neighbourhood names, zone labels, data point annotations. Tight, readable, non-intrusive on map backgrounds.

## Layout

**Civic reporting variant:** Map as primary interface — the city is the context. Report button always visible, floating above the map. Issue list accessible via bottom sheet. Status tracking is the key retention feature — every submitted report shows a visible timeline.

**Planning dashboard variant:** Desktop-first. Left panel: filters and layer controls. Center: map or primary visualisation. Right panel: detail and data cards for selected elements. Designed for collaborative use — multiple people viewing the same screen in a meeting.

## Elevation & Depth

Map interfaces require clear visual hierarchy — interactive elements must be obviously distinguishable from map content. Cards that float above the map use white background with a visible border and subtle shadow (exception to the no-shadow rule — map context requires it for legibility).

Status cards use color fills rather than borders to quickly communicate state across a long list.

## Shapes

Standard 12px for most cards. Report button uses `xl` (20px) — it is the single most important action and deserves generous treatment. Map markers are circular — 32px for standard, 40px for selected state.

## Components

**Report Button:** Full-width on mobile, floating action on map view. Amber background. Camera icon + "Report a problem" label. Tapping opens a 3-step flow: category → location confirm → photo/description.

**Issue Card:** Category icon, title, street address, submission date, status pill, vote count ("14 residents agree"), resolution timeline. The vote count is social proof that makes individual reporting feel collective.

**Status Timeline:** Vertical timeline of report lifecycle — Submitted → Reviewed → In Progress → Resolved. Each step has a timestamp and a brief note. The most important component for building resident trust.

**Stat Card:** Large number (stat scale), label below, trend arrow and percentage, time period. Used in planning dashboard for KPIs.

**Map Layer Toggle:** Pill-style toggles for data layers — Infrastructure, Green Space, Transport, Population. Civic-blue active state.

**Zone Card:** Planning dashboard card for a selected urban zone. Name, area, population estimate, active issues count, key indicators. Civic-blue header strip.

## Do's and Don'ts

- Do show report status updates proactively — push notifications when status changes are the single biggest driver of re-engagement
- Do use amber for resident-facing actions and civic blue for official/government information — never mix the roles
- Don't require an account to submit a basic report — anonymous reporting increases volume significantly
- Do design the map marker cluster states — reports cluster at zoom-out, individual at zoom-in
- Don't show more than 5 active data layers simultaneously — map becomes unreadable
- Do localise category labels — "pothole" means different things in different cities
- Don't use amber for error states — it is an action color, not a warning color. Use standard error red.
- Do provide an offline submission queue — residents in areas with poor infrastructure may have poor connectivity

## The Trust Gap

Civic reporting tools fail not because of bad design — they fail because residents don't believe reporting works. In most cities, fewer than 20% of residents who see a problem report it. The primary reason is not laziness: it is learned helplessness from past reports that were ignored.

**Show resolution rates prominently.** Before a resident submits their first report, show them: "In your neighbourhood, 73% of reports are resolved within 14 days." If the rate is low, show it anyway — honesty builds more trust than silence. A tool that hides poor performance data will be abandoned when residents discover the truth.

**The accountability loop is the product.** The report submission is not the valuable action — the follow-up is. Every status change must trigger a notification. "Your report about the broken streetlight on Keizersgracht has been assigned to a crew" is more valuable than any feature. Design the notification as carefully as the submission form.

**Anonymous reporting increases volume 3x.** Research consistently shows that requiring identity verification reduces civic reporting dramatically, especially in communities with low trust in government. Anonymous reporting with optional identity disclosure always outperforms mandatory registration. Make it the default.

**Design for the sceptic, not the activist.** The person most likely to use this app is not a civic-minded activist — they are someone who nearly tripped on a broken pavement and is mildly annoyed. Design the first-use experience for that person: fast, low-effort, immediate confirmation, no account required. Convert them to a repeat user through demonstrated results, not onboarding flows.
